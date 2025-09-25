# Urnen-Aufgaben

### In einer Urne liegen 3 blaue, 2 rote und 5 grüne Bälle. Wie groß ist jeweils die Wahrscheinlichkeit, zwei gleichfarbige Bälle zu erhalten? Sie greifen blind hinein und holen nacheinander 2 Bälle heraus, und zwar
#### Klausur WS 2006/07
a) ohne Zurücklegen,

Beim Ziehen ohne Zurücklegen verändert sich nach dem ersten Zug die Anzahl der Bälle einer Farbe und die Gesamtzahl im zweiten Zug. Wir berechnen für jede Farbe die Wahrscheinlichkeit, dass beide gezogenen Bälle diese Farbe haben, und addieren die Wahrscheinlichkeiten:

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

<img width="3600" height="2400" alt="image" src="https://github.com/user-attachments/assets/8331dc0d-b7f0-4cc5-8db9-e3f2fc93f641" />
