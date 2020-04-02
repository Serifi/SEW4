# 502_DB_Storage

## Objektorientierte Struktur
Implementiere eine objektorientierte Struktur:
- Klasse ```Song```
- Klasse ```Album```
- sowie  die entsprechende Beziehung dazwischen (Song:Album , n:m Beziehung -> wie in der Datenbank)

Wähle eine gut geeignete Collection-Klasse zur Speicherung der Songs im Album. 

Die Klassen sollen wie üblich ```Konstruktor```, notwendige ```Getter/Setter``` und ```toString``` (für einfache Auflistungen/Anzeigen) besitzen.


## DAO (Data-Access-Object)
Wir wollen nun je eine eigene Klasse für Song und Album erstellen, die den Datenbankzugriff – und später vielleicht Dateizugriff, ... - auf die jeweilige Tabelle verwalten. Diese Klassen nennt man DAO (Data-Access-Object).

## Aufgabe:
Verwende PreparedStatement und Transaktionen, wenn notwendig/sinnvoll!

### Implementiere eine Klasse ```SongDAO```:
Diese besitzt folgende Methoden:
- ```int insertSong(Song s)```: Rückgabewert: 0....ok, 1....bereits vorhanden, 2....sonstiger Fehler

### Implementiere eine Klasse ```AlbumDAO```:
Diese besitzt folgende Methoden :
- ```int insertAlbum(Album a)```: Rückgabewert: 0....ok, 1....bereits vorhanden, 2....sonstiger Fehler
- ```int addSongToAlbum(Song s, Album a)```: Rückgabewert: 0....ok, 1....bereits vorhanden, 2....sonstiger Fehler
- ```Album getAlbum(String albumName)```


### Teste deine Klassen in einer eigenen Klasse ```SongManagement```:
- Lies ein beliebiges Album aus der DB.
- Gib dieses Album am Bildschirm aus.
- Füge einen Song zu diesem Album hinzu.
- Lies das Album erneut aus der DB.
- Gib dieses Album nochmals am Bildschirm aus.
- Hinweis: Die DAO-Klassen werden später noch erweitert und ausgebaut (Interfaces und Methoden)!
