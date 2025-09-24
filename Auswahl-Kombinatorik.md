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
