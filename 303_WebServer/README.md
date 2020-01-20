# 303_WebServer

## Aufgabe:
Implementiere einen einfachen HTTP Server und grafischen Client

### Anforderungen HTTP-Server:
- Primitiver Webserver, welcher nur `HTTP GET` versteht (keine Query Strings!)
- Webserver implementiert Status 200, 400 und 404 korrekt
- Der eigene Webserver kann zum Test mit einem Webbrowser verbunden werden und liefert eine korrekte Website (inkl. CSS, JS und Bilder!)
- wird keine Datei in der übergebenen URL vom Client angegeben, so ist nach der Datei `index.htm` zu suchen und gegebenenfalls diese zu retournieren
- Konfiguration des Webservers:
  - Portnummer
  - Wurzelverzeichnis für Webprojekt


### Anforderungen HTTP-Client:
- Einfacher JavaFX Webclient
- URL kann eingegeben werden
- implementiert HTTP Protokoll - nimmt Verbindung mit Server auf und holt sich eine HTML Datei
- Kommunikation mit dem Server ist im grafischen Client anzuzeigen
- Client ist "so eine Art" von Debugger/Entwicklungswerkzeug für einen Webserver

![Anwendung](209.png)
