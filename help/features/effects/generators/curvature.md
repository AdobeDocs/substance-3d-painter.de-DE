---
title: Krümmung
description: Erfahren Sie, wie Sie den Krümmung-Generator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 8%

---


# Biegung

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_curvature.webp" alt=""/><br><strong>In:</strong> Maske, Generator, Graustufen, Überblendung</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Maskengenerator erstellt eine Krümmung auf der Grundlage der Baking geführt Krümmungs-Map mit der Option, eine Textur oder Mikrodetails in die Maske einzufügen.<br><br>Der Krümmung-Generator gibt eine monochrome (schwarz-weiß) Textur aus. Daher ist sie zum Generieren von Masken nützlich, anstatt sie direkt auf eine Ebene anzuwenden.<br><br>Eine Baking geführt Positionszuordnung ist als Eingabe erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Micro Normal** Farbe | Verwenden Sie eine benutzerdefinierte Textur oder einen benutzerdefinierten Ankerpunkt. |
| **Micro Height** Color | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Krümmung** Graustufen | Verwenden Sie die Baking geführt Krümmungs-Map. |
| **Welt-Raum-Normale** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Positionsverlauf** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Weicht die endgültige Maske gleichmäßig auf, nachdem alle Effekte kombiniert wurden. |
| **Globaler Saldo** | Verschiebt die Balance der letzten Maske, nachdem alle Effekte zwischen Schwarz und Weiß kombiniert wurden, wie bei einer Helligkeitsanpassung. |
| **Globaler Kontrast** | Passt den Kontrast der letzten Maske an, nachdem alle Effekte kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Textur-Map ein oder aus. |
| **Micro-Details verwenden** | Schalten Sie die Verwendung der benutzerdefinierten Mikro-Details-Karte ein oder aus. |

### Biegung

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Generierte Krümmungs-Map umkehren.</td>
  </tr>
  <tr>
    <td><strong>Modus</strong></td>
    <td>Setze den Kurvenmodus. <br><ul><li><strong>Kanten</strong>: Maskiert die Kanten (konvexe Bereiche).</li><li><strong>Hohlräume</strong>: Maskiert die Hohlräume (konkave Bereiche)</li><li><strong>Dual</strong>: Masken für konkave und konvexe Bereiche.</li><li><strong>Unverarbeitet</strong>: Normale Krümmung.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Scharf</strong></td>
    <td>Passe die Stärke der Details der scharfen Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Fein</strong></td>
    <td>Passe die Stärke der Details der Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Weich</strong></td>
    <td>Passe die Stärke der Details der weichen Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Mittel</strong></td>
    <td>Passen Sie die Stärke der Details mittlerer Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Groß</strong></td>
    <td>Passe die Stärke der großen Krümmungen an.</td>
  </tr>
  <tr>
    <td><strong>Groß</strong></td>
    <td>Passe die Stärke der großen Krümmungen an.</td>
  </tr>
  <tr>
    <td><strong>Riesig</strong></td>
    <td>Passen Sie die Stärke der riesigen Krümmungsdetails an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie den Kontrast/Abfall der Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der Krümmung an.</td>
  </tr>
</table>

### Textur

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Strukturdeckkraft</strong></td>
    <td>Steuern Sie die Sichtbarkeit der benutzerdefinierten Textur.</td>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehre nur die Textur um.</td>
  </tr>
  <tr>
    <td><strong>Graustufenkonvertierung</strong></td>
    <td>Wählen Sie die Methode aus, mit der die Farbeingabe in Schwarz-Weiß konvertiert werden soll. </td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Legen Sie den Mischmodus für die benutzerdefinierte Textur fest.</td>
  </tr>
  <tr>
    <td><strong>Skalieren</strong></td>
    <td>Passen Sie die Größe der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Legen Sie den Kontrast/Abfall der benutzerdefinierten Textur fest.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Legen Sie die Luminanz der benutzerdefinierten Textur fest.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Wenn Triplanar aktiviert ist, wird die Textur aus drei Richtungen projiziert (X-, Y-, Z-Achsen), anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne die Option "Triplanar" folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarem Mapping projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Projektionen aus jeder Richtung angepasst.</td>
  </tr>
</table>

### Mikrodetails

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Mikrohöhe</strong></td>
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Höhen-Map.</td>
  </tr>
  <tr>
    <td><strong>Mikro-Normale</strong></td>
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Normalen-Map.</td>
  </tr>
  <tr>
    <td><strong>Biegungstyp</strong></td>
    <td>Legen Sie die Krümmung fest. <br><ul><li><strong>Standard</strong>: Erstellt ein normalerweise recht scharfes Ergebnis, kann jedoch größere Details vermissen lassen.</li><li><strong>Sobel</strong>: Ergibt ähnliche Ergebnisse wie bei der Standardausgabe, ist jedoch leicht unscharf, da die Normalen-Map mit einem Sobel-Filter ausgewertet wird.</li><li><strong>Glatt</strong>: Erzeugt verschiedene Weichzeichnungsstufen (wie Mipmaps), um Informationen zu sammeln. Dadurch entstehen in der Regel glattere Kurven, aber Details können verloren gehen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie die Stärke der Krümmung in den Modi <strong>Standard </strong> und <strong>Sobel </strong> Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Höhendetailstärke</strong></td>
    <td>Passen Sie die Stärke der Micro Height-Details an.</td>
  </tr>
</table>
