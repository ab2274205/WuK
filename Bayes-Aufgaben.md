# Aufgabe SS 2014
Eine seltene Krankheit tritt mit einer Wahrscheinlichkeit von $10^{-5}$ auf. Ein Antikörpertest für diese Krankheit erkennt eine Infektion mit einer Wahrscheinlichkeit von 95%. Gesunde Probanden werden mit einer Wahrscheinlichkeit von 0,5% irrtümlich als krank 
eingestuft (positives Testergebnis). Wie groß ist die Wahrscheinlichkeit, dass bei einem positiven Testergebnis tatsächlich eine Infektion vorliegt? 

## Gegebene Wahrscheinlichkeiten

- $P(\text{Krank}) = 10^{-5}$ — Wahrscheinlichkeit, dass eine Person tatsächlich krank ist (sehr selten).
- $P(\text{Gesund}) = 1 - P(\text{Krank}) = 1 - 10^{-5} \approx 0{,}99999$.
- $P(\text{Positiv} | \text{Krank}) = 0{,}95$ — Wahrscheinlichkeit, dass der Test positiv ist, wenn die Person krank ist (Sensitivität).
- $P(\text{Positiv} | \text{Gesund}) = 0{,}005$ — Wahrscheinlichkeit, dass der Test positiv ist, obwohl die Person gesund ist (Falsch-Positiv-Rate).

***

## Gesuchte Wahrscheinlichkeit

- Gesucht ist $P(\text{Krank} | \text{Positiv})$ — die Wahrscheinlichkeit, dass die Person tatsächlich krank ist, wenn das Testergebnis positiv ist.

***

## Schritt 1: Satz von Bayes anwenden

Der Satz von Bayes lautet:

$$
P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}
$$

Hier übersetzt auf unser Problem:

$$
P(\text{Krank} | \text{Positiv}) = \frac{P(\text{Positiv} | \text{Krank}) \times P(\text{Krank})}{P(\text{Positiv})}
$$

***

## Schritt 2: Berechnung von $P(\text{Positiv})$ — Gesamtwahrscheinlichkeit für ein positives Testergebnis

Ein positives Testergebnis entsteht entweder, wenn die Person krank ist und der Test richtig positiv ausfällt oder wenn die Person gesund ist und ein Fehler (Falsch-Positiv) auftritt:

$$
P(\text{Positiv}) = P(\text{Positiv} | \text{Krank}) \times P(\text{Krank}) + P(\text{Positiv} | \text{Gesund}) \times P(\text{Gesund})
$$

Einsetzen der Werte:

$$
P(\text{Positiv}) = 0{,}95 \times 10^{-5} + 0{,}005 \times 0{,}99999
$$

$$
P(\text{Positiv}) \approx 9,5 \times 10^{-6} + 0{,}00499995 \approx 0{,}00500945
$$

***

## Schritt 3: Einsetzen in Satz von Bayes

$$
P(\text{Krank} | \text{Positiv}) = \frac{0{,}95 \times 10^{-5}}{0{,}00500945} \approx \frac{9,5 \times 10^{-6}}{0{,}00500945} \approx 0{,}001896
$$

***

## Ergebnis

Die Wahrscheinlichkeit, dass die Person bei einem positiven Testergebnis tatsächlich krank ist, liegt bei etwa 0,0019 oder 0,19%.

***
