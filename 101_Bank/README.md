# 101_Bank

## Klasse Bank
- [ ] Ein Objekt der Klasse *SimpleBank* modelliert eine reale Bank, welche Konten für verschiedene Personen verwaltet.
- [ ] Die Bank führt eine Anzahl an Überweisungen durch.
- [ ] Da auch in einer realen Bank mehrere Angestellte beschäftigt sind, die sich gleichzeitig um die Bearbeitung solcher Überweisungen kümmern, werden auch im Programmodell die Überweisungen in parallelen Threads abgearbeitet.
- [ ] Die Implementierung der Bank wird durch eine Klasse *SimpleBank* realisiert.
- [ ] Diese Bank besitzt das Array *konten*, das die Stände der einzelnen Konten enthält.
- [ ] Der Array-Index dient uns  als Kontonummer.
- [ ] Für Transaktionen zwischen zwei Konten stellt SimpleBank die Methode *ueberweisung()* zur Verfügung. Ihr werden die beiden beteiligten Kontonummern sowie der Betrag der Überweisung übergeben.
- [ ] Zu Demonstrationszwecken wird die Ausführung der Überweisung zwischen der Berechnung des neuen Kontostands und dessen Zurückschreiben unterbrochen.
- [ ] Der Bankangestellte liest zuerst den aktuellen Kontostand aus und speichert ihn, dann wird die Bearbeitungsdauer durch ein sleep simuliert.
- [ ] Im Anschluss wird der neue Stand berechnet und auf das Konto zurückgeschrieben.
- [ ] Zufällige Zeit schlafen: *Thread.sleep((int)Math.random()*1000);*

´´´Java
class SimpleBank {
 private int[] konten = {30, 50, 100};

 public void ueberweisung(int von, int nach, int betrag)
 public void kontostand()
}
´´´

## Klasse Angestellter
- [ ] Die Überweisungen sollen durch Bankangestellte erfolgen.
- [ ] Diese werden durch die Klasse *Angestellter* implementiert.
- [ ] Damit mehrere Angestellte gleichzeitig Transaktionen vornehmen können, werden sie von Thread abgeleitet (Alternativ: Runnable).
- [ ] Jeder Angestellte gehört zu einer Bank.
- [ ] Deshalb wird dem Konstruktor ein Verweis auf SimpleBank übergeben. Über diesen Verweis wird die Methode *ueberweisung()* aufgerufen.
- [ ] Die beiden beteiligten Kontonummern sowie der Betrag werden dem Konstruktor übergeben und in entsprechenden Datenelementen der Klasse gespeichert.


## Aufgabe
- [ ] Implementiere die beiden Klassen
- [ ] Erstelle 3 Angestellte, welche jeweils eine Überweisung von einem Konto auf das andere durchführen (Ringüberweisung)
- [ ] Gib die Kontostände vor und nach den Überweisungen aus
- [ ] Pushe die Lösung auf Github
- [ ] Was fällt auf?
