---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# Generator für bekannte Probleme - Substance 3D Painter

Automatisiert das Generieren des Markdown-Dokuments für bekannte Probleme für Substance 3D Painter, das unter folgender Adresse veröffentlicht wird:
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

Probleme stammen aus dem Jira-Epos `SBSFOUR-6267`. Das Skript ruft alle Probleme ab, filtert alle bereits in der Zielversion behobenen Elemente heraus und gibt eine formatierte Markdown-Datei aus, die zum Commit bereit ist.

---

## Schnellstart

Bei diesen Schritten wird davon ausgegangen, dass Sie die einmalige Einrichtung unten bereits abgeschlossen haben.

1. Verbindung mit **GlobalProtect VPN** herstellen
2. Legen Sie `TARGET_VERSION` in der Datei `.env` auf die Version fest, für die Sie Dokumente generieren (z. B. `12.0.3`)
3. Führen Sie das Skript im Verzeichnis &quot;`scripts/known-issues-automation/`&quot; aus:

   ```
   python fetch_known_issues.py
   ```
4. Überprüfen Sie die Ausgabebeschreibung. Sie zeigt an, wie viele Probleme abgerufen und wie viele davon ausgeschlossen wurden.
5. Generierte `known-issues.md` in `help/release-notes/known-issues.md` kopieren

> Wenn Probleme fehlen oder unerwartet auftreten, überprüfen Sie `raw_issues.json`, um genau zu sehen, was Jira zurückgegeben hat, bevor die Filterung angewendet wurde.

---

## Einmalige Einrichtung

### &#x200B;1. Abhängigkeiten installieren

```bash
pip install requests python-dotenv
```

### &#x200B;2. `.env`-Datei erstellen

```bash
cp .env.example .env
```

### &#x200B;3. Abrufen eines persönlichen Jira-Zugriffstokens

1. Anmelden bei `https://jira.corp.adobe.com`
2. Gehen Sie auf der linken Seitenleiste zu Ihrem Profil → **Persönliche Zugriffstoken**
3. Klicken Sie auf **Token erstellen**, geben Sie ihm einen Namen, und kopieren Sie den generierten Wert.

> PATs laufen nicht ab, wenn Ihre Browsersitzung endet, was sie zuverlässiger als Sitzungs-Cookies für den skriptbasierten API-Zugriff macht.

### &#x200B;4. `.env`-Datei ausfüllen

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION` ist die Version von Substance 3D Painter, für die Sie die Seite mit bekannten Problemen generieren. Es steuert, welche behobenen Probleme ausgeschlossen werden — siehe [Filtering Logic](#filtering-logic) weiter unten.

---

## Repository-Struktur

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

---

## Jira Reference

| Feld | Value |
|---|---|
| Jira-Instanz | `https://jira.corp.adobe.com` |
| Projektschlüssel | `SBSFOUR` |
| Bekannte Probleme epic | `SBSFOUR-6267` |

Alle bekannten Probleme müssen mit diesem Epos verknüpft sein, damit es im generierten Dokument angezeigt wird. Wenn ein Problem hinzugefügt oder von der Seite entfernt werden muss, aktualisieren Sie das Epos in Jira, anstatt das Markdown manuell zu bearbeiten.

---

## Funktionsweise des Skripts

### Schritt 1 - Abrufen

Das Skript fragt die Jira REST API mithilfe von JQL ab:

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

Die Ergebnisse werden bei 50 Ausgaben pro Seite paginiert. Die folgenden Felder werden für jedes Problem abgerufen: `summary`, `issuetype`, `status`, `affectedVersions`, `fixVersions`, `labels`

Die Authentifizierung verwendet ein Bearer-Token von `JIRA_PAT`. Die Jira-Instanz des Unternehmens verwendet ein internes SSL-Zertifikat, daher ist die Zertifikatüberprüfung für diese Anforderungen deaktiviert. Dies ist ein erwartetes Verhalten im Adobe-Netzwerk.

### Schritt 2 - Raw-Dump

Vor jeder Filterung oder Formatierung schreibt das Skript `raw_issues.json`. Dies ist eine vereinfachte Momentaufnahme jedes Problems, das Jira zurückgab, und wird immer generiert, unabhängig davon, was als Nächstes passiert. Wenn die Ausgabe falsch aussieht, überprüfen Sie zuerst diese Datei. Sie zeigt genau an, welche Daten Jira bereitgestellt hat.

### Schritt 3 - Filter

Probleme werden anhand zweier gemeinsam angewendeter Regeln gefiltert:

1. **Statusfilter** — nur `Backlog` und `Dev In Progress` Probleme sind aktive bekannte Probleme. Probleme mit dem Status &quot;`Fixed`&quot; sind Ausschlusskandidaten, die der unten stehenden Versionsprüfung unterliegen.

2. **Versionsfilter** — Ein `Fixed`-Problem ist nur ausgeschlossen, wenn eine der Fixversionen kleiner oder gleich `TARGET_VERSION` ist. Wenn die Fix-Version höher als `TARGET_VERSION` ist, ist das Problem weiterhin enthalten, da der Fix für die zu dokumentierende Version nicht ausgeliefert wurde.

Dies gilt für den Fall, dass zwei Versionen gleichzeitig entwickelt werden: Ein in `12.1.0` behobenes Problem bleibt ein bekanntes Problem für `12.0.3`.

Die vollständige Entscheidungstabelle finden Sie unter [Filtering Logic](#filtering-logic).

### Schritt 4 - Kategorien analysieren

Jede Problemzusammenfassung wird nach Kategorie-Tags am Anfang der Zeichenfolge analysiert:

- `[Shader] Some description` →: 1, Beschreibung: 2`["Shader"]``"Some description"`
- `[Crash][Engine] Some description` →: 1, Beschreibung: 2`["Crash", "Engine"]``"Some description"`
- `No brackets here` → keine Kategorien, behandelt als nicht kategorisiert

Die **primäre Kategorie** ist immer das erste Tag. Sie bestimmt die Gruppierung und die Abschnittsplatzierung.

### Schritt 5 - Gruppieren und Sortieren

Die Themen sind wie folgt organisiert:

- Probleme sind nach Primärkategorie gruppiert
- Gruppen werden nach Problemanzahl sortiert, absteigend (größte Gruppen zuerst)
- Gruppen mit mehreren Problemen werden oben im Dokument angezeigt
- Gruppen mit nur einem Problem sowie alle nicht kategorisierten Probleme werden nach den Gruppen mit mehreren Problemen ohne Abschnittsüberschrift angezeigt
- Probleme mit `[Crash]` als primäre Kategorie werden immer als letztes in einem Abschnitt `## Stability` platziert.

### Schritt 6 - Formatieren und Schreiben

Das Skript gibt `known-issues.md` aus mit:

- YAML-Titelblatt (helpx-Metadaten)
- Eine `# Known issues`-Überschrift mit einem Intro-Absatz, der die Zielversion benennt
- Probleme formatiert als: `` * `[Category]` Description ``
- Probleme mit mehreren Kategorien: `` * `[Category1]` `[Category2]` Description ``
- Leere Linien zwischen Kategoriegruppen
- Ein `## Stability`-Abschnitt am Ende für Absturzprobleme

---

## Filterlogik

| Status | Versionssatz beheben? | Version und Ziel korrigieren | Enthalten? |
|---|---|---|---|
| `Backlog` | — | — | Ja |
| `Dev In Progress` | — | — | Ja |
| `Fixed` | Nein | — | Nein (konservativ ausgeschlossen) |
| `Fixed` | Ja | Version ≤ Ziel korrigieren | Nein (bereits ausgeliefert) |
| `Fixed` | Ja | Version korrigieren > Ziel | Ja (Korrektur erfolgt in einer zukünftigen Version) |

---

## Ausgabeformat

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**Die Formatierungshinweise:** Kategorie-Tags verwenden einen einzelnen Backtick-Wrapping — `` `[Category]` `` — nicht doppelte Backtick-Wrapping. Das ältere manuell verwaltete Dokument enthielt Fehler mit doppeltem Backtick. das Skript immer das richtige Format erzeugt.

---

## Fehlerbehebung

**401 Nicht autorisiert**
- Bestätigen Sie, dass Sie mit **GlobalProtect VPN** verbunden sind.
- Ihr PAT ist möglicherweise abgelaufen oder wurde widerrufen. Generieren Sie einen neuen bei `https://jira.corp.adobe.com/secure/ViewProfile.jspa`, und aktualisieren Sie `.env`.

**`JIRA_PAT is not set`Fehler**
- Stellen Sie sicher, dass Sie eine `.env`-Datei aus `.env.example` erstellt und Ihr Token ausgefüllt haben.
- Bestätigen Sie, dass Sie das Skript im Verzeichnis &quot;`scripts/known-issues-automation/`&quot; ausführen, damit `python-dotenv` die Datei &quot;`.env`&quot; finden kann.

**Probleme in der Ausgabe fehlen**
- Überprüfen Sie `raw_issues.json` — wenn das Problem nicht vorhanden ist, ist es nicht mit dem Epic `SBSFOUR-6267` in Jira verknüpft.
- Wenn das Problem in `raw_issues.json`, aber nicht in der Ausgabe vorliegt, wurde es durch den Filter ausgeschlossen. Überprüfen Sie seinen Status, und korrigieren Sie die Version anhand Ihrer `TARGET_VERSION`.

**`TARGET_VERSION`Warnung zur Laufzeit**
- Das Skript wird ausgeführt, schließt jedoch alle `Fixed` Probleme konservativ aus, wenn `TARGET_VERSION` nicht festgelegt ist. Legen Sie dies immer fest, bevor Sie das endgültige Dokument generieren.
