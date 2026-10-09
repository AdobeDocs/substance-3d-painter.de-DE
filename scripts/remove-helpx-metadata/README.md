---
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%
---
# Ältere HelpX-Metadaten entfernen

Führen Sie in Python 3.10 oder höher die folgenden Befehle aus dem Repository-Stammordner aus:

```shell
python remove_helpx_metadta.py 1 <path>
python remove_helpx_metadta.py 2 <path>
```

Modus &quot;`1`&quot; ist ein trockener Run: Es listet übereinstimmende Dateien auf und meldet die Anzahl der Dateien.
gescannte Dateien, Dateien mit Übereinstimmungen und übereinstimmende Metadatenfelder, ohne Dateien zu ändern.
Modus `2` entfernt diese Felder und meldet die Anzahl der Entfernungen. `<path>` auslassen auf
den aktuellen Ordner zu durchsuchen. Angebotspfade mit Leerzeichen.

Das Skript durchsucht rekursiv `.md` Dateien (ohne Berücksichtigung der Groß-/Kleinschreibung) und entfernt die oberste Ebene.
YAML-Titelblattfelder, deren Namen mit `helpx` beginnen, einschließlich ihrer mehrzeiligen Felder
-Werte. Andere Metadaten, Kommentare, Leerzeilen, Markdown-Inhalte werden beibehalten.
Kodierung und Zeilenenden. `helpx` Verweise im Textkörper werden nicht entfernt.
Überprüfen Sie den Testlauf, bevor Sie Modus &quot;`2`&quot; verwenden. Entfernen bearbeitet Dateien an Ort und Stelle ohne
Erstellen von Backups. Es werden Dateifehler und nicht geschlossenes Titelblatt gemeldet, die
einem Nicht-Null-Beendigungsstatus. Dateien mit nicht geschlossenem Titelblatt bleiben unverändert.