## Würfelaufgaben
### Klausur WS 2006/07

Sie werfen zwei Würfel. Wie groß ist die Wahrscheinlichkeit, dass

---

### (a) Mindestens einer der Würfel zeigt eine 6

**Formel:** Laplace-Wahrscheinlichkeit ist die klassische Definition der Wahrscheinlichkeit für Zufallsexperimente mit endlicher Ergebnismenge, bei der alle Ergebnisse gleichwahrscheinlich sind. Die Wahrscheinlichkeit für ein Ereignis $$A$$ berechnet sich als: 

$$P(A) = \frac{\text{Anzahl der Ergebnisse, bei denen das Ereignis } A \text{ eintritt}}{\text{Anzahl aller möglichen Ergebnisse}} = \frac{|A|}{|\Omega|}$$

Hierbei bezeichnet:

- $$|A|$$ die Anzahl der günstigen Ergebnisse (Elemente des Ereignisses $$A$$),
- $$|\Omega|$$ die Anzahl aller möglichen Ergebnisse (Ergebnismenge).

Diese Definition setzt voraus, dass alle Elementarereignisse gleichwahrscheinlich sind.

- Anzahl aller möglicher Ergebnisse: $$(6 \times 6 = 36)$$
- Anzahl der Ergebnisse ohne eine 6: $$(5 \times 5 = 25)$$
- Wahrscheinlichkeit

$$\[P(\text{mind. eine 6}) = 1 - \frac{25}{36} = \frac{11}{36} \approx 0,31\]$$

---

### (b) Die Summe der beiden Augenzahlen ist 7

- Mögliche Paare: (1,6), (2,5), (3,4), (4,3), (5,2), (6,1)
- Anzahl der günstigen Ergebnisse: 6
- Wahrscheinlichkeit:

$$\[P(\text{Summe} = 7) = \frac{6}{36} = \frac{1}{6} \approx 0,167\]$$

---

### (c) Das Produkt der beiden Augenzahlen ist ein Vielfaches von 10

- Zahlen auf den Würfeln: 1 bis 6
- Produkt ist durch 10 teilbar, wenn Produkt mindestens einen Faktor 2 und einen Faktor 5 enthält.
- 5 erscheint nur als Faktor bei einer 5.
- Die Faktoren 2 erhält man bei einer 2, 4 oder 6.
- Vorgehen:

Alle Paare ($$(x,y)$$), bei denen $$(x=5)$$ und $$(y)$$ gerade (2,4,6) oder $$(y=5)$$ und $$(x)$$ gerade.

- Günstige Paare:  
(5,2), (5,4), (5,6), (2,5), (4,5), (6,5)

- Anzahl günstiger Ergebnisse: 6
- Wahrscheinlichkeit:

$$\[P(\text{Produkt Vielfaches von 10}) = \frac{6}{36} = \frac{1}{6} \approx 0,167\]$$

<img width="3600" height="2400" alt="image" src="https://github.com/user-attachments/assets/3cedbccd-6507-421d-ad6a-37d909cf82f8" />


***
## Aufgabe Klausur SS 2014 a) Welche Augensumme hat die größte Wahrscheinlichkeit?

### Schritt 1: Alle möglichen Ergebnisse bestimmen

- Beim Würfeln mit zwei sechsseitigen Würfeln gibt es $6 \times 6 = 36$ mögliche Ergebnisse.


### Schritt 2: Mögliche Augensummen

- Die kleinste Summe ist $2$ (1+1).
- Die größte Summe ist $12$ (6+6).
- Mögliche Augensummen sind also $2, 3, 4, ..., 11, 12$.


### Schritt 3: Anzahl der Kombinationen für jede Summe zählen

| Summe | Kombinationen (Würfel 1, Würfel 2) |
| :-- | :-- |
| 2 | (1,1) |
| 3 | (1,2), (2,1) |
| 4 | (1,3), (2,2), (3,1) |
| 5 | (1,4), (2,3), (3,2), (4,1) |
| 6 | (1,5), (2,4), (3,3), (4,2), (5,1) |
| 7 | (1,6), (2,5), (3,4), (4,3), (5,2), (6,1) |
| 8 | (2,6), (3,5), (4,4), (5,3), (6,2) |
| 9 | (3,6), (4,5), (5,4), (6,3) |
| 10 | (4,6), (5,5), (6,4) |
| 11 | (5,6), (6,5) |
| 12 | (6,6) |



### Schritt 4: Wahrscheinlichkeit berechnen

- Wahrscheinlichkeit für eine Summe ist Anzahl der Kombinationen für die Summe geteilt durch 36.
- Beispiel: Für Summe 7 ist das $\frac{6}{36} = \frac{1}{6}$.


### Schritt 5: Ergebnis

- Die Augensumme 7 hat die meisten mögliche Kombinationen (6) und somit die größte Wahrscheinlichkeit von $\frac{1}{6} \approx 0,1667$.

***

## Aufgabe b) Wahrscheinlichkeit, dass mindestens einer der Würfel eine 1 oder 2 zeigt

### Schritt 1: Gegenereignis definieren

- Statt direkt zu zählen, wann mindestens eine 1 oder 2 kommt, zählen wir die Fälle, in denen *keine* 1 oder 2 geworfen wird.


### Schritt 2: Möglichkeiten ohne 1 oder 2 zählen

- Die möglichen Augenzahlen ohne 1 oder 2 sind: 3, 4, 5, 6 — also 4 Möglichkeiten pro Würfel.
- Anzahl Kombinationen mit beiden Würfeln aus {3,4,5,6} sind $4 \times 4 = 16$.


### Schritt 3: Wahrscheinlichkeit des Gegenereignisses

- Wahrscheinlichkeit, dass keiner der Würfel eine 1 oder 2 zeigt, ist $\frac{16}{36} = \frac{4}{9}$.


### Schritt 4: Gewünschte Wahrscheinlichkeit berechnen

- Wahrscheinlichkeit dafür, dass mindestens einer eine 1 oder 2 zeigt, ist das Gegenereignis:

$$
1 - \frac{4}{9} = \frac{5}{9} \approx 0,5556
$$

***
