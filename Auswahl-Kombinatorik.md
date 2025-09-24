# Auswahl-Kombinatorik (7 P.)

#### Klausur SS25 (Auswahl ohne Zurücklegen ohne Reihenfolge - **Kombinatorik ohne Wiederholungen**)
## In einer Klausur können Sie sich aus 10 Aufgaben 7 aussuchen. Wieviele Wahlmöglichkeiten haben Sie, falls

(a) keine Einschränkungen vorliegen?
Gegeben:

- $$n$$ = 10 (Gesamtanzahl)
- $$k$$ = 7 (Anzahl der ausgewählten Aufgaben)

$$\binom{n}{k} = \binom{10}{7} = 120$$

(b) entweder die erste oder die zweite ausgewählt werden müssen (aber nicht beide)?
1. **Gegeben:**
    - Es gibt insgesamt 10 Aufgaben.
    - Es müssen 7 Aufgaben ausgewählt werden.
    - Einschränkung: Entweder Aufgabe 1 oder Aufgabe 2 muss ausgewählt werden, aber nicht beide gleichzeitig.
    
2. **Aufteilung in Fälle:** 
    - Fall 1: Aufgabe 1 ist ausgewählt, Aufgabe 2 nicht.
    - Fall 2: Aufgabe 2 ist ausgewählt, Aufgabe 1 nicht.
    
      (Auswahl 1 oder 2 -- Laplace-Wahrscheinlichkeit $$W=({1,2})=\frac{2}{10}$$)
      
3. **Restliche Aufgaben:**
    - Übrig bleiben 8 Aufgaben (alle außer den beiden ersten).
    - Aus diesen 8 müssen in beiden Fällen jeweils 6 Aufgaben zusätzlich ausgewählt werden, denn zusammen mit der schon gewählten Aufgabe ergibt das 7.
    
4. **Berechnung:**
    - Anzahl der Möglichkeiten im ersten Fall: $\binom{8}{6}$
    - Anzahl der Möglichkeiten im zweiten Fall: $\binom{8}{6}$
    - Wegen zwei Fällen: Gesamtzahl = $2 \times \binom{8}{6} = 2 \times 28 = 56$

(c) von den ersten 5 Aufgaben genau 3 ausgewählt werden müssen?

1. **Gegeben:**
    - 10 Gesamtaufgaben
    - 7 ausgewählte Aufgaben insgesamt
    - Von den ersten 5 Aufgaben müssen genau 3 ausgewählt werden.
2. **Aufteilung der Auswahl:**
    - Wähle 3 aus den ersten 5 Aufgaben: $\binom{5}{3}$ Möglichkeiten.
    - Wähle die verbleibenden 4 Aufgaben aus den restlichen 5 (10 - 5 = 5) Aufgaben: $\binom{10-5}{7-3}$ Möglichkeiten.
3. **Berechnung:**
    - Gesamtmöglichkeiten = $\binom{5}{3} \times \binom{5}{4} = 10 \times 5 = 50$


#### Klausur 2014 (Auswahl ohne Zurücklegen ohne Reihenfolge - **Kombinatorik ohne Wiederholungen**)
## Ein Student muss in einer Prüfung 10 von 13 Fragen beantworten.  
(a) Auf wie viele verschiedene Weisen kann er 10 Fragen auswählen (und beantworten)?

$$
\binom{13}{10} = 286
$$

(b) Auf wie viele Weisen, falls er auf jeden Fall die beiden ersten Fragen beantworten muss? 

Anzahl der Weisen, 10 Fragen auszuwählen, wenn die ersten beiden Fragen auf jeden Fall beantwortet werden müssen:
Hier sind die Fragen 1 und 2 fix ausgewählt, also wählt der Student 8 weitere Fragen aus den verbleibenden 11 aus:

$$
\binom{11}{8} = 165
$$

(c) Auf wie viele Weisen, falls er genau 3 der ersten 5 Fragen beantworten muss? 

Aus den ersten 5 Fragen wählt er genau 3, aus den restlichen 8 (13 - 5) wählt er 7 - 3 = 4 Fragen:

$$
\binom{5}{3} \times \binom{8}{4} = 10 \times 8 = 80
$$

(d) Auf wie viele Weisen, falls er mindestens 3 der ersten 5 Fragen beantworten muss? 

Das sind die Fälle genau 3, genau 4 oder genau 5 der ersten 5 Fragen:

$$
\binom{5}{3} \times \binom{8}{7-3} + \binom{5}{4} \times \binom{8}{7-4} + \binom{5}{5} \times \binom{8}{7-5} = 80 + 165 + 31 = 276
$$
