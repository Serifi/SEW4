# 501_Database

## Aufgabe:
Schreibe ein Java-Programm, das die Alben-Datenbank im Batch anlegt und mit mindestens 3 Alben und deren Liedern befüllt. Zu diesem Zweck soll der Beispiel-Code zur Batch-Verarbeitung eigenständig durchgearbeitet werden.

Das Anlegen der Datenbank soll mit PreparedStatement-Instanzen erfolgen. Alle Create-Anweisungen sollen dabei in einer Transaktion zusammengefasst werden, ebenso alle Insert-Anweisungen.

Die Datenbank soll folgende Anforderungen erfüllen:

- ```database albums```
  - ```table songs: songtitle, artist, year, genre```  
  - ```table album_songs: albumtitle, songtitle, tracknumber```  
  - ```table albums: albumtitle, artist, label```

Die Zugangsdaten dieser Datenbank lauten wie folgt:
```
Driver=org.hsqldb.jdbc.jdbcDriver 
Url=jdbc:hsqldb:file:./hsqldb/albums;shutdown=true;ifexists=false
User=SA
Password=
```
und sind in einer ```.properties-Datei``` abgelegt (siehe Java-Klasse Properties)
