## KLAUSUR25 - Buchstabensalat, Mengen, Multimengen (7 P.)

### Gegeben sei das Wort MAMALAMML.

**(a) Wie viele verschiedene Worte kann man durch Vertauschen der Buchstaben von „MAMALAMML“ erzeugen?**

Vorbetrachtung: Das Wort besteht aus der Multimenge der Buchstaben
$$S$$ = {M, M , M , M , A, A, A, L, L}
Dabei ist $$S$$ eine Multimenge, weil Buchstaben mehrfach vorkommen.

Gegeben:

- $$n$$ = 9 (Gesamtanzahl der Buchstaben)
- $$n_1$$ = 4 (Anzahl der Buchstaben M)
- $$n_2$$ = 3 (Anzahl der Buchstaben A)
- $$n_3$$ = 2 (Anzahl der Buchstaben L)

Da es sich um eine Multimenge handelt, verwenden wir die allgemeine Formel für **Permutationen mit Wiederholungen**:

$$
P_n(n_1,n_2,\ldots,n_k) = \frac{n!}{n_1! \cdot n_2! \cdot \ldots \cdot n_k!}
$$

Berechnung:

$$
P_n(n_1,n_2,n_3) = \frac{9!}{4! \cdot 3! \cdot 2!} = \frac{362880}{24 \cdot 6 \cdot 2} = \boxed{1260}
$$

***

**(b) Wie viele dieser Worte beginnen und enden mit "M"?**

Festlegung: Das erste und letzte Zeichen sind jeweils ein M, also werden 2 M verwendet.

Verbleibende Buchstaben:

- $$n$$ = 9 - 2 = 7 (zu permutieren)
- $$n_1$$ = 2 (verbleibende M)
- $$n_2$$ = 3 (A)
- $$n_3$$ = 2 (L)

Wieder Anwendung der Permutationsformel (mit Wiederholungen):

$$
P_n(n_1,n_2,n_3) = \frac{7!}{2! \cdot 3! \cdot 2!} = \frac{5040}{2 \cdot 6 \cdot 2} = \boxed{210}
$$

***

**(c) Wie viele dieser Worte enthalten die Zeichenfolge „MAMA“?**

Betrachte die Zeichenfolge „MAMA“ als einen zusammenhängenden Block.

Neue Multimenge:

$$S'$$ = {MAMA, M, M, A, L, L}

Anzahl der Elemente in $$S'$$: $$n$$ = 6

Vielfachheiten:

- $$n_1$$ = 2 (M)
- $$n_2$$ = 2 (L)
- $$n_3$$ = 1 (A)
- $$n_4$$ = 1 (MAMA)

Formel für Permutationen mit Wiederholungen:

$$
P_n(n_1,n_2,n_3,n_4) = \frac{6!}{2! \cdot 2! \cdot 1! \cdot 1!} = \frac{720}{2 \cdot 2 \cdot 1 \cdot 1} = \boxed{180}
$$


## ESA1 - Aufgabe 4 – Buchstabenpermutationen des Wortes ELEVEN

**Gegeben:** 6 Buchstaben mit $$E$$ dreifach, andere Buchstaben einfach.

Gegeben:

- $$n$$ = 6 (Gesamtanzahl der Buchstaben)
- $$n_1$$ = 3 (Anzahl der Buchstaben E)
- $$n_2$$ = 1 (Anzahl der Buchstaben L)
- $$n_3$$ = 1 (Anzahl der Buchstaben V)
- $$n_4$$ = 1 (Anzahl der Buchstaben N)

### (a) Wie viele Worte kann man hieraus durch Buchstabenvertauschungen erzeugen ?

**Verwendete Formel: Permutationen mit Wdh.:**

$$
\frac{n!}{(n_1)! * (n_2)! * (n_3)! * (n_4)!} = \frac{6!}{3!} = 4 * 5 * 6 = 120
$$

### (b) Wie viele dieser Worte beginnen und enden mit einem E ?

Fixierte Positionen: Anfang und Ende = E → verbleibend: L, V, N, E

$$
\frac{(n-2)!}{(n_1 - 2)! * (n_2)! * (n_3)! * (n_4)!} = 4! = 24
$$

### (c) Wie viele dieser Worte enthalten die drei E's direkt hintereinander ?

Block `EEE`, restliche Buchstaben: L, V, N → 4 Elemente:

$$
n! = 4! = 24
$$

### (d) Wie viele dieser Worte beginnen mit E und enden mit N ?

Verbleibende Buchstaben: 2xE, L, V

$$
\frac{(n-2)!}{(k_1-1)! *(k_2)! * (k_3)! * (k_4-1)!} = 
        \frac{4!}{2!} = \frac{24}{2} = 12
$$
