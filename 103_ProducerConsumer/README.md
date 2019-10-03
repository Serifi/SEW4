# 102_ProducerConsumer

![Producer Consumer grafisch](ProducerConsumer.png)

## Producer
- [ ] der Produzent produziert Bälle (simuliert durch Zufallszahlen)
- [ ] die Produktion eines Balls dauert eine zufällige Zeit (z.B. zw. 500 und 1000ms)
- [ ] die produzierten Bälle werden gedanklich auf ein Fließband gelegt (Speicherung in Queue)
- [ ] das Fließband ist auf 10 Footballs begrenzt, ist das Fließband voll, muss der Produzent warten
- [ ] der Produzent informiert die Consumer, sobald etwas am Fließband liegt

## Consumer
- [ ] Consumer schlafen, bis sie vom Produzenten informiert werden
- [ ] sobald sie aufwachen, nehmen sie sich das erste Element vom Fließband und packen es ein
- [ ] die Verarbeitung dauert eine zufällige Zeit (z.B. zw. 500 und 1000ms)

## Aufgabe
- [ ] Implementiere das oben genannte Consumer/Producer Beispiel mittels Warten und Benachrichtigen
- [ ] Jede Aktion (Producer bzw. Consumer) mittels Konsolenoutputs dokumentieren
- [ ] Pushe die Lösung auf Github
