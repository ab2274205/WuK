# Buchstabensalat, Mengen, Multimengen (7 P.)

### Gegeben sei das Wort MAMALAMML.
#### Klausur SS25
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

***
### Gegeben sei das Wort ELEVEN.
#### ESA1 25

**(a) Wie viele Worte kann man hieraus durch Buchstabenvertauschungen erzeugen ?**
Gegeben:
- $$n$$ = 6 (Gesamtanzahl der Buchstaben)
- $$n_1$$ = 3 (Anzahl der Buchstaben E)
- $$n_2$$ = 1 (Anzahl der Buchstaben L)
- $$n_3$$ = 1 (Anzahl der Buchstaben V)
- $$n_4$$ = 1 (Anzahl der Buchstaben N)

**Verwendete Formel: Permutationen mit Wdh.:**

$$
\frac{n!}{(n_1)! * (n_2)! * (n_3)! * (n_4)!} = \frac{6!}{3!} = 4 * 5 * 6 = 120
$$

**(b) Wie viele dieser Worte beginnen und enden mit einem E ?**

Fixierte Positionen: Anfang und Ende = E → verbleibend: L, V, N, E → (n = 4)

**Verwendete Formel: Permutationen ohne Wdh.:**

$$
n! = 4! = 24
$$

**(c) Wie viele dieser Worte enthalten die drei E's direkt hintereinander ?**

Block `EEE`, restliche Buchstaben: L, V, N → 4 Elemente:
**Verwendete Formel: Permutationen ohne Wdh.:**
$$
n! = 4! = 24
$$

**(d) Wie viele dieser Worte beginnen mit E und enden mit N ?**

Verbleibende Buchstaben: 2xE, L, V

**Verwendete Formel: Permutationen mit Wdh.:**

$$
\frac{(n-2)!}{(n_1-1)! *(n_2)! * (n_3)! * (n_4-1)!} = 
        \frac{4!}{2!} = \frac{24}{2} = 12
$$

***
### Gegeben seien die Ziffern 1, 2, 3, 4, 5.
#### Präsenzveranstaltung SS 2025

**(a) Wie viele verschiedene Anordnungen dieser 5 Ziffern gibt es?**

Vorbetrachtung: Die 5 Ziffern sind alle verschieden.

Gegeben:

- **n = 5** (Anzahl der Ziffern)

Da alle 5 Ziffern verschieden sind, verwenden wir die Formel für **Permutationen ohne Wiederholung**:

$$
P_n = n! = 5! = 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 120
$$


**(b) Wie viele vierstellige Zahlen kann man aus diesen Ziffern bilden, wenn jede Ziffer beliebig oft vorkommen kann?**

Vorbetrachtung: Hier dürfen Ziffern mehrfach verwendet werden (mit Wiederholung), und die Zahl besteht aus 4 Stellen (Variation).

- **k** - Anzahl der Stellen: **4**
- **n** - Anzahl der möglichen Ziffern pro Stelle: **5**

Da jede Stelle unabhängig gewählt werden kann mit 5 möglichen Ziffern, gilt:

$$
n^k = 5^4 = 5 \cdot 5 \cdot 5 \cdot 5 = 625
$$

**(c) Wie viele dreistellige Zahlen kann man bilden, wenn jede Ziffer nur höchstens einmal vorkommen darf?**

Vorbetrachtung: Es handelt sich um Variation ohne Wiederholung von 3 Ziffern aus 5.

- **k** - Anzahl der Stellen: **3**
- **n** - Anzahl der möglichen Ziffern pro Stelle: **5**

Die Anzahl der Permutationen von $n=5$ Elementen zur Auswahl von $k=3$ lautet:

$$
P(5,3) = \frac{5!}{(5-3)!} = \frac{5!}{2!} = \frac{120}{2} = 60
$$

***
### Gegeben seien BAFANABAFANA
#### Einsendeaufgabe 2020

Gegeben:
- $$n$$ = 12 (Gesamtanzahl der Buchstaben)
- $$n_1$$ = 2 (Anzahl der Buchstaben B)
- $$n_2$$ = 2 (Anzahl der Buchstaben F)
- $$n_3$$ = 2 (Anzahl der Buchstaben N)
- $$n_4$$ = 6 (Anzahl der Buchstaben A)

(a) Wie viele Woerter kann man hieraus durch Buchstabenvertauschungen erzeugen?

Es gibt:
        12! / (6! 2! 2! 2!) = 83160
    Anordnungen

(b) Wie viele dieser Woerter beginnen mit BA und enden mit NA?

Es gibt:
        (12 - 4)!/ (6-2)! * (2)! * (2-1)! * (2-1)! = 8! / (4! 2! 1! 1!) = 840
    Anordnungen, die mit einem BA beginnen und einem NA enden.

(c) Wie viele dieser Woerter kann man so erzeugen, bei denen die B’s, die F’s und die
 N‘s nur paarweise nebeneinander auftreten (also als BB, FF bzw. NN)?)
BB, FF, NN, 6 x A 
**n** = 9 (12 - 3)

 Es gibt:
        9! / (6! 1! 1! 1!) = 504
    Anordnungen.
