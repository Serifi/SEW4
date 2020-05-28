# 505_JavaFX_UI

Die Verwaltung von Alben und deren Songs soll durch eine ansprechende grafische Oberfläche in JavaFX realisiert werden.

![UML](./505.png)

## FUNTIONALITÄT (Mindestanforderung)
- Anzeige der Daten in einer GUI inkl. Bild
- Navigation innerhalb der Daten (Album wählen + dazugehörige Lieder anzeigen, nächstes/voriges Album/Direktauswahl?)
- Hinzufügen neuer Datensätze (Alben inkl. Album-Cover + dazugehörige Lieder)
- Löschen von Datensätzen
- Editieren von Datensätzen (Ändern vom Inhalt, Bilder, ...)
- Persistierung der Daten in HSQLDB gemäß vorhergehenden Übungen (DAO!)

## WICHTIG
- die Abfrage der Albendaten kann u.U. länger dauern und muss daher im Hintergrund ablaufen (vgl. Multithreading in JavaFX - Task/Service), bei allen anderen Abfragen ist dies nicht nötig
- Implementierung gemäß MVC
- Model (```Songmanagement```) beinhaltet (eigenen Klassen/Interface):  
  - Song zu Album hinzufügen
  - Songs eines Albums bereitstellen
  - ...
- Der Zugriff auf die DAO-Objekte darf NICHT in den Ereignisbehandlern stattfinden, sondern muss im Model gekapselt werden.  
- Die Ereignisbehandler rufen nur die Methoden des Models für die tatsächliche Umsetzung der Benutzerinteraktion (speichern, laden, hinzufügen, ...) auf.
- Sämtliche Abhängigkeiten der UI-Elemente von bestimmten Zuständen (Speichern nur bei ungespeicherten Änderungen aktiv, Fortschrittsanzeigen, ...) sind in Form von Bindings zu realisieren.
- Layout/Optik ist nach persönlichen Vorstellungen zu implementieren, gerne auch List/TableViews bzw. “Aufhübschung” mittels CSS
