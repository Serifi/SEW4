# 407_Batch

## Aufgabe:
Ergänze das Blog-Beispiel!
- Die Benutzertabelle soll mit dem Inhalt einer Benutzerdatei befüllt werden können (auch nachträglich!)
- Nutze dazu, wenn von der DB unterstützt (->Metainfo), die Batch-Funktionalität von PreparedStatement
- Erstelle eine Eingabedatei (>= 20 Einträge) mit den erforderlichen Werten (.csv-Format; ID, Name, Passwort, ...)

## Anmerkungen:
- Riesige Datenmengen in einem einzigen execute/commit zu persistieren kann im Fehlerfall das ganze Projekt (Datenübernahme, ...) gefährden.
- Deshalb soll die Batch-Größe und jedes einzelne commit nur einen Teil der gesamten Datenmenge umfassen.
- Im Fehlerfall soll der betroffene Eintrag/Bereich in einem Protokoll eindeutig vermerkt werden.
- Die übrigen Einträge/Bereiche sollen dennoch importiert werden. Diese Anforderungen wirkt sich massiv auf die Art und Weise der Fehlerbehandlung aus.
