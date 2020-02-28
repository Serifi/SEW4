# Herzlich Willkommen bei SEW4!

## 0. Wichtige Links
* SEW-Repository: [4AHIT Classroom](https://classroom.github.com/a/3rzQ6clL), [4BHIT Classroom](https://classroom.github.com/a/i1RMN8wW)
* Hilfe bekommst du fast immer hier:
	+ [Stack Overflow](http://stackoverflow.com)

## 1. Source Code Verwaltung mit git

Arbeite folgende Links durch, um mit git bzw. GitHub vertraut zu machen:
* [git - Der einfache Einstieg](https://rogerdudler.github.io/git-guide/index.de.html)
* [git Cheat Sheet](https://rogerdudler.github.io/git-guide/files/git_cheat_sheet.pdf)
* [git für Einsteiger](https://svij.org/blog/2014/10/25/git-fur-einsteiger-teil-1/)
* [GitHub Guide](https://guides.github.com/activities/hello-world/)
* [git Reference](https://git-scm.com/docs)

### 1.1 Git in SEW
Sämtliche Programmierarbeit ist auf GitHub "abzugeben". Sofern Programmieraufgabe gestellt werden, sind diese nach Beendigung der letzten SEW Stunde an diesem Tag in die Repository zu pushen. Selbiges gilt auch für Hausübungen und Projekte.
Dazu ist es notwendig EIN Verzeichnis zu erstellen, wo ALLE IntelliJ/CLion Projekte in Unterordner enthalten sind.

Die Aufgaben sind in eigenen Unterordnern(=Projekten) bereitzustellen. Der Name des Projekts entspricht der Angabe, Beispiel: "101_Ausgabe"
Jede Commitmessage beginnt mit dem Datum "031017 - Test Projekt erstellt"

Bei korrekter Konfiguration erkennt auch IntelliJ in den Unterprojekten, dass es unter GIT Kontrolle steht. Die Einstellung findest du unter "Preferences - Version Control" - hier kann das VCS root-Verzeichnis angegeben werden, d.h. das ist euer "IntelliJ"-Ordner, in dem alle Projekte enthalten sind.

### 1.2 Erstelle deine Repository
Deine persönliche Repository für dieses Schuljahr findest du hier: 
* [4AHIT Classroom](https://classroom.github.com/a/3rzQ6clL)
* [4BHIT Classroom](https://classroom.github.com/a/i1RMN8wW)


### 1.3 ".gitignore"
git kann mittels der Datei ".gitignore" mitgeteilt werden, welche Dateien bzw. Ordner NICHT unter git-Kontrolle stehen. Das ist natürlich sinnvoll, denn Beispielsweise .class Dateien oder IntelliJ Projekteinstellungen sollten nicht hochgeladen werden.

Daher erstelle eine Datei ".gitignore" im deinem Hauptordner (dort findest du auch einen Ornder ".git"). Entnimm den Inhalt meiner .gitignore Datei (siehe Repository von oben).

### 1.4 README.md
Erstelle eine Datei <b>README.md</b> mit folgendem Inhalt bzw. ändere eine Datei, sofern sie schon erstellt wurde:
```
# SEW 4 - SJ 20xx/xx
----
Name: Vorname Nachname
...
```

Damit ist es mir schneller möglich dich mit deinem richtigen Namen zu identifizieren - die Repos kommen beim clonen immer mit deinem GitHub-Usernamen an. Daraus läßt sich unter Umständen nicht schließen, von wem die Arbeit kommt.
