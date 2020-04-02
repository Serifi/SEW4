# 503_DAO

## Erklärung:
DAO (Data Access Object) ist eigentlich auch ein Designpattern (oder Muster wie man ein bestimmtes Problem löst). Dabei wird die Persistenzschicht (also jene Klassen, welche für die dauerhafte "Speicherung" von z.B. Alben und Songs zuständig sind) von den Domainklassen (das sind die Klassen welche die objektorientierte Struktur des Inhalts widerspiegeln; z.B. Klasse ```Song``` und Klasse ```Album```) getrennt.

Um die Trennung der Domainklassen von den DAO-Klassen möglichst optimal zu gestalten benötigen wir?...... richtig!......... ein Interface. Damit können die Persistenzklassen ausgetauscht werden, ohne die Domainklassen und eigentliche Anwendung ändern zu müssen.
In unserem Fall benötigen wir 2 Interfaces, die von ```SongDAO``` und ```AlbumDAO``` implementiert werden müssen. Normalerweise würde man zuerst die gewünschten Interfaces definieren und dann die implementierenden Klassen realisieren. 

## Aufgabe 1:

Erstelle nun die beiden Interfaces
- ```SongDAOInterface```
- ```AlbumDAOInterface```

mit den benötigten Methoden (die ja schon implementiert sind) basierend auf den bereits erstellten DAO-Klassen.

IntelliJ unterstützt das Herausheben von Interfaces aus Klassen (Rechte Maustaste - Refactor – Extract – Interface).


## Aufgabe 2:  
Ergänze (die Album-Interfaces und -/Klassen) zusätzlich um folgende Methoden:
- ```Collection<Albums> getAllAlbums()```
- ```boolean removeSongFromAlbum(Song s)```

Wenn du alles richtig gemacht hast, kannst du in der Klasse ```SongManagement``` die Typen der Referenzvariablen von ```SongDAO``` und ```AlbumDAO``` auf die entsprechenden Interfaces umstellen.

z.B:
von: ```SongDAO sdi=new SongDAO();```  
zu:  ```SongDAOInterface sdi=new SongDAO();```

Teste die bisherigen und auch die neuen Methoden!
