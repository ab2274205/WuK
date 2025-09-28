# [Kombinatorik](https://github.com/ab2274205/WuK/blob/main/Kombinatorik-Aufgaben.md) und [Kombinatorik-Auswahl](https://github.com/ab2274205/WuK/blob/main/Auswahl-Kombinatorik-Aufgaben.md)

| Menge            | Name         | Reihenfolge | mit/ohne Wiederholung | Formel                                     |Verwendung |
|------------------|--------------|-------------|-----------------------|--------------------------------------------|-----------|
| alle Elemente    | Permutation  | ja          | ohne Wiederholung (ohne Zurücklegen)     | $$n!$$       | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md), [Schachspiel](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md#beim-schachspiel-kann-ein-turm-nur-vertikal-oder-horizontal-ziehen-beziehungsweise-schlagen-wir-betrachten-nun-ein-verallgemeinertes-schachbrett-mit-nn-feldern-wie-viele-m%C3%B6glichkeiten-gibt-es-n-ununterscheidbare-t%C3%BCrme-so-auf-diesem-brett-zu-verteilen-dass-keiner-einen-anderen-bedroht-in-jeder-horizontalen-reihe-und-jeder-vertikalen-linie-darf-also-nur-h%C3%B6chstens-ein-turm-stehen) |
| alle Elemente    | Permutation  | ja          | mit Wiederholung      | $$\frac{n!}{(n₁! · n₂! · ... · nₙ!)}$$       | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Variation    | ja          | ohne Wiederholung     | $$\frac{n!}{(n - k)!}$$                     | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Variation    | ja          | mit Wiederholung      | $$n^k$$                                   | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Kombination  | nein        | ohne Wiederholung     | $$\binom{n}{k}$$ = $$\frac{n!}{[(n - k)! · k!]}$$ (Binomialkoeffizient) | [Auswahl](https://github.com/ab2274205/WuK/blob/main/Auswahl-Kombinatorik.md) | 
| Stichprobe (k)   | Kombination  | nein        | mit Wiederholung      | $$\binom{n + k - 1}{k}$$                   | [Sträuße](https://github.com/ab2274205/WuK/blob/main/Auswahl-Kombinatorik-Aufgaben.md#ein-florist-hat-rosen-in-4-verschiedenen-farben-vorr%C3%A4tig-auf-wie-viele-weisen-k%C3%B6nnen-sie-str%C3%A4u%C3%9Fe-aus-6-rosen-zusammenstellen-wenn)|

**Legende:**  
- *n* - Gesamtanzahl der Elemente in der Grundmenge
- *n₁*,*n₂*,... - Anzahl gleicher Elemente  
- *k* - Anzahl der Elemente in der Stichprobe  

---

**[Urnenmodell:](https://github.com/ab2274205/WuK/blob/main/Urnen-Aufgaben.md)**

Ziehen ohne Zurücklegen ohne Reihenfolge:
$$\binom{N}{n} = \frac{N!}{n! \cdot (N - n)!}$$

Hypergeometrische Verteilung (Dichtefunktion):
$$f(x) = \frac{\binom{M}{x} \cdot \binom{N - M}{n - x}}{\binom{N}{n}}$$

**Legende:**  
- $$N$$: Anzahl der Kugeln insgesamt 
- $$M$$: Anzahl der schwarzen Kugeln 
- $$n$$: Anzahl der Ziehungen
- $$x$$: Anzahl der gezogenen schwarzen Kugeln


---
**[Würfel-Aufgaben](https://github.com/ab2274205/WuK/blob/main/Würfel-Aufgaben.md)**

**Formel:** Laplace-Wahrscheinlichkeit ist die klassische Definition der Wahrscheinlichkeit für Zufallsexperimente mit endlicher Ergebnismenge, bei der alle Ergebnisse gleichwahrscheinlich sind. Die Wahrscheinlichkeit für ein Ereignis $$A$$ berechnet sich als: 

$$P(A) = \frac{\text{Anzahl der Ergebnisse, bei denen das Ereignis } A \text{ eintritt}}{\text{Anzahl aller möglichen Ergebnisse}} = \frac{|A|}{|\Omega|}$$

Hierbei bezeichnet:

- $$|A|$$ die Anzahl der günstigen Ergebnisse (Elemente des Ereignisses $$A$$),
- $$|\Omega|$$ die Anzahl aller möglichen Ergebnisse (Ergebnismenge).

---
**[Binomialverteilung, Laplace-Experiment: Wahrscheinlichkeitsfunktion](https://github.com/ab2274205/WuK/blob/main/Binomialverteilung-Aufgabe.md)**

$$
P(k) = \binom{n}{k} p^k q^{n-k}
$$

- $n$: Anzahl der Sätze (Versuche)
- $k$: Anzahl der gewonnenen Sätze (Erfolge)
- $\binom{n}{k}$: Binomialkoeffizient, Anzahl der Möglichkeiten, $k$ Erfolge aus n Sätzen zu wählen
- $p^k$: Wahrscheinlichkeit für $k$ Erfolge (Erfolgswahrscheinlichkeit)
- $q^{n-k}$: Wahrscheinlichkeit für ($n-k$) Misserfolge (Misserfolgswahrscheinlichkeit)

---

**[Der Satz von Bayes](https://github.com/ab2274205/WuK/blob/main/Bayes-Aufgaben.md)**

$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$
$$P(\text{Positiv}) = P(\text{Positiv} | \text{Krank}) \times P(\text{Krank}) + P(\text{Positiv} | \text{Gesund}) \times P(\text{Gesund})$$

---
**Wahrscheinlichkeit**

$$P(A) = 1 − P(A)$$
$$P(A ∪ B) = P(A) + P(B) − P(A ∩ B)$$
$$P(A \ B) = P(A) − P(A ∩ B)$$

---
**[Übersicht typischer Stammfunktionen in der Integralrechnung](https://github.com/ab2274205/WuK/blob/main/Zufallsvariable-Aufgaben.md)**

Wenn $F$ eine Stammfunktion von $f$ ist und $C$ eine beliebige reelle Zahl (Konstante), dann ist auch $F(x) + C$ eine Stammfunktion von $f$.

$$f(x) = ax^n$$

$$F(x) = \frac{a}{n+1} x^{n+1}$$

|  | Unbestimmtes Integral | Bestimmtes Integral |
| :-- | :-- | :-- |
| Darstellung | $$\int f(x) dx$$ = F(x) + C$$ | $$\int_a^b f(x) dx$$ |

Dabei ist $\int$ das Integrationszeichen und $f(x)$ der Integrand. Die Variable $x$ heißt Integrationsvariable und $C$ ist die Integrationskonstante.

| f(x) | F(x) |
| :-- | :-- |
| f(x) = 1 | F(x) = x |
| f(x) = 2 | F(x) = 2x |
| f(x) = eˣ | F(x) = eˣ |
| f(x) = sin(x) | F(x) = -cos(x) |
| f(x) = cos(x) | F(x) = sin(x) |
| f(x) = 1/x | F(x) = ln(x) |

$$
\int_a^b f(x)\, dx = [F(x)]_a^b = F(b) - F(a) = (F(b) - F(a)) * C = 1
$$

