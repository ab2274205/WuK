# Urnen-Aufgaben

### In einer Urne liegen 3 blaue, 2 rote und 5 grüne Bälle. Wie groß ist jeweils die Wahrscheinlichkeit, zwei gleichfarbige Bälle zu erhalten? Sie greifen blind hinein und holen nacheinander 2 Bälle heraus, und zwar
#### Klausur WS 2006/07
a) ohne Zurücklegen,

Beim Ziehen ohne Zurücklegen verändert sich nach dem ersten Zug die Anzahl der Bälle einer Farbe und die Gesamtzahl im zweiten Zug. Wir berechnen für jede Farbe die Wahrscheinlichkeit, dass beide gezogenen Bälle diese Farbe haben, und addieren die Wahrscheinlichkeiten. 

- **Blaue:**
$$P_{blau}$$ = $$\frac{3}{10} \times \frac{2}{9}$$
- **Rote:**
$$P_{rot}$$ = $$\frac{2}{10} \times \frac{1}{9}$$
- **Grüne:**
$$P_{gruen}$$ = $$\frac{5}{10} \times \frac{4}{9}$$

Gesamtwahrscheinlichkeit (Summe):

$$P_{\text{gleich}} = \frac{3}{10} \cdot \frac{2}{9} + \frac{2}{10} \cdot \frac{1}{9} + \frac{5}{10} \cdot \frac{4}{9}= \frac{14}{45} \approx 0,31$$

Hier wurde das **multiplikative Gesetz** der Wahrscheinlichkeit für aufeinanderfolgendes Ziehen ohne Zurücklegen verwendet.

***

b) mit Zurücklegen

Beim Ziehen mit Zurücklegen bleibt die Anzahl der Kugeln im zweiten Zug gleich. Die Wahrscheinlichkeit, dass man zweimal eine bestimmte Farbe zieht, ist:

- **Blaue:**
$$P_{blau} = \frac{3}{10} \times \frac{3}{10}$$
- **Rote:**
$$P_{rot} = \frac{2}{10} \times \frac{2}{10}$$
- **Grüne:**
$$P_{gruen} = \frac{5}{10} \times \frac{5}{10}$$

Gesamtwahrscheinlichkeit (Summe):

$$P_{\text{gleich}} = \frac{3 \cdot 3 + 2 \cdot 2 + 5 \cdot 5}{10 \cdot 10}= \frac{9+4+25}{100}= \frac{38}{100}= 0,38$$

<img width="4200" height="3000" alt="image" src="https://github.com/user-attachments/assets/edcfafa3-5f03-4f0f-831f-ddb3d48521fc" />


***
### Aufgabe SS 2014
In einem Sack befinden sich 2 rote, 2 blaue, 2 gelbe und 2 weiße Bälle. Sie greifen blind hinein und holen gleichzeitig 3 Bälle heraus. 
 Wie groß ist die Wahrscheinlichkeit dafür, dass 
a) die gezogenen Bälle alle verschiedenfarbig sind,
b) Sie genau zwei gleichfarbige Bälle und einen andersfarbigen Ball ziehen, 
c) mindestens ein roter Ball dabei ist? 

#### Schritt 1: Gesamtzahl der möglichen Kombinationen

Die Gesamtzahl der möglichen Arten, $n = 3$ Kugeln aus $N = 8$ zu ziehen, berechnet sich mit der Kombination ohne Reihenfolge:

$$
\binom{8}{3} = \frac{8!}{3! \cdot 5!} = \frac{8 \times 7 \times 6}{3 \times 2 \times 1} = 56
$$

***

#### Schritt 2: Wahrscheinlichkeit a) — alle drei Kugeln haben verschiedene Farben

- Zuerst wählen wir 3 verschiedene Farben aus 4 möglichen aus:

$$
\binom{4}{3} = 4
$$

- Für jede davon gibt es 2 Kugeln, aus denen wir jeweils 1 Kugel wählen können, also $2$ Möglichkeiten pro Farbe:

$$
2 \times 2 \times 2 = 2^3 = 8
$$

- Die Anzahl günstiger Ereignisse ist somit:

$$
4 \times 8 = 32
$$

- Die Wahrscheinlichkeit ergibt sich aus dem Verhältnis günstiger Ereignisse zur Gesamtzahl der Ereignisse:

$$
P(a) = \frac{32}{56} = \frac{4}{7}
$$

***

## Schritt 3: Wahrscheinlichkeit b) — genau zwei Kugeln gleicher Farbe und eine Kugel anderer Farbe

- Wähle die Farbe, von der 2 Kugeln gezogen werden:

$$
\binom{4}{1} = 4
$$

- Wähle 2 Kugeln aus den 2 vorhandenen Kugeln dieser Farbe (nur 1 Möglichkeit):

$$
\binom{2}{2} = 1
$$

- Wähle eine andere Farbe aus den verbleibenden 3 Farben:

$$
\binom{3}{1} = 3
$$

- Wähle 1 Kugel aus den 2 vorhandenen Kugeln dieser anderen Farbe:

$$
\binom{2}{1} = 2
$$

- Die Anzahl günstiger Ereignisse ist:

$$
4 \times 1 \times 3 \times 2 = 24
$$

- Die Wahrscheinlichkeit ist:

$$
P(b) = \frac{24}{56} = \frac{3}{7}
$$

***

## Schritt 4: Wahrscheinlichkeit c) — mindestens eine rote Kugel

- Zuerst bestimmen wir die Gegenwahrscheinlichkeit, dass keine rote Kugel gezogen wird.
- Anzahl der Kugeln ohne rot ist $6$ (2 blau + 2 gelb + 2 weiß).
- Anzahl der Arten, 3 Kugeln aus den 6 nicht-roten zu ziehen:

$$
\binom{6}{3} = \frac{6 \times 5 \times 4}{3 \times 2 \times 1} = 20
$$

- Wahrscheinlichkeit, keine rote Kugel zu ziehen:

$$
P(\text{kein Rot}) = \frac{20}{56} = \frac{5}{14}
$$

- Wahrscheinlichkeit für mindestens eine rote Kugel:

$$
P(c) = 1 - P(\text{kein Rot}) = 1 - \frac{5}{14} = \frac{9}{14}
$$


