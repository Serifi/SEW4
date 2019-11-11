# 206_ObjectBinding

Implementiere folgende

## Aufgaben
Zu entwickeln ist eine ImageViewer App. Der User gibt einen Dateinamen ein und es wird automatisch das dazugehörige Bild per Bindings geladen.

## GUI
- [ ] TextField für die Eingabe des Dateinamens
- [ ] ImageView für die Darstellung des Bilds

## Klasse ImageViewerBinding
- [ ] entwickle die Klasse, welche ObjectBinding überschreibt
- [ ] im Konstruktor wird ein StringProperty übergeben, welches den Dateinamen beinhaltet
- [ ] die Methode computeValue() gibt das Bild zurück

## Bindings
- [ ] binde das imageProperty der ImageView an das TextProperty des TextFields
