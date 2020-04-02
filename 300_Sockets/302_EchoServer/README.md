# 302_EchoServer

## Aufgabe:
Entwickle einen Echo Server und dazu passenden Client

### Server
- beim Start gibt der Server seine Socket Adresse in der Konsole aus (Recherche Internet/JavaAPI)
- Server wartet auf Port 2007 auf eingehende Verbindungen
- jede eingehende Verbinung wird in einem EIGENEN Thread bearbeitet
- somit können sich mehrere Clients gleichzeitig mit dem Server verbinden
- vom Client wird ein Text geschickt, dieser wird als Echo an den Client zurück gesendet

### Client
- baut Verbindung mit Server auf Port 2007 auf
- die entfernte Socket Adresse soll in der Konsole ausgegeben werden
- User kann Text eingeben, welcher an den Server geschickt wird
- empfangenes Echo wird am Bildschirm ausgegeben


### Erweiterung
- baue den EchoServer aus - verwende einen ThreadPool!
