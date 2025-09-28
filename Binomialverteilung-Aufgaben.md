### Aufgabe
#### WS 2006/07
Anne und Britta spielen ein Tennismatch über 4 Sätze. Anne ist die bessere Spielerin: Sie gewinnt einen Satz mit einer Wahrscheinlichkeit von $\frac{2}{3}$.

Wie groß ist die Wahrscheinlichkeit, dass"

### a) Anne alle 4 Sätze gewinnt?

### Binomialverteilung: Wahrscheinlichkeitsfunktion

$$
P(k) = \binom{n}{k} p^k q^{n-k}
$$

- $n$: Anzahl der Sätze (Versuche)
- $k$: Anzahl der gewonnenen Sätze von Anne (Erfolge)
- $\binom{n}{k}$: Binomialkoeffizient, Anzahl der Möglichkeiten, $k$ Erfolge aus n Sätzen zu wählen
- $p^k$: Wahrscheinlichkeit für $k$ Erfolge (Erfolgswahrscheinlichkeit)
- $q^{n-k}$: Wahrscheinlichkeit für ($n-k$) Misserfolge (Misserfolgswahrscheinlichkeit)

Gegeben:

- $$n$$ = 4
- $$k$$ = 4
- $$p$$ = $\frac{2}{3}$
- $$q$$ = $\frac{1}{3}$
  
$$
P(4) = \binom{4}{4} \left(\frac{2}{3}\right)^4 \left(\frac{1}{3}\right)^0 = 1 \cdot \left(\frac{16}{81}\right) \cdot 1 = \frac{16}{81}
$$

### b) Anne genau 2 Sätze gewinnt und 2 verliert?

Gegeben:

- $$n$$ = 4
- $$k$$ = 2
- $$p$$ = $\frac{2}{3}$
- $$q$$ = $\frac{1}{3}$
  
$$
P(2) = \binom{4}{2} \left(\frac{2}{3}\right)^2 \left(\frac{1}{3}\right)^2 = 6 \cdot \frac{4}{9} \cdot \frac{1}{9} = \frac{24}{81} = \frac{8}{27}
$$

### c) Anne mindestens 2 Sätze gewinnt?

$$
P(\geq 2) = P(2) + P(3) + P(4)
$$

Berechnen wir $P(3)$:

$$
P(3) = \binom{4}{3} \left(\frac{2}{3}\right)^3 \left(\frac{1}{3}\right)^1 = 4 \cdot \frac{8}{27} \cdot \frac{1}{3} = \frac{32}{81}
$$

Summieren:

$$
P(\geq 2) = \frac{8}{27} + \frac{32}{81} + \frac{16}{81} = \frac{24}{81} + \frac{32}{81} + \frac{16}{81} = \frac{72}{81} = \frac{8}{9}
$$

***
