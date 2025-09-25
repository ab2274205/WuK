## Aufgabe

### Die kontinuierliche Zufallsvariable \$ X \$ besitze die Dichtefunktion
$$
f(x) = 
\begin{cases}
C (1 - x^2) & \text{für } -1 \leq x \leq 1 \\
0 & \text{sonst}
\end{cases}
$$

### a) Welchen Wert muss $$C$$ haben?

Die Dichtefunktion muss so normiert sein, dass das Integral über den gesamten Definitionsbereich gleich 1 ist:

$$\int_{-\infty}^{\infty} f(x) \, dx = 1$$

Da $$f(x) = C(1-x^2)$$ für $$-1 \leq x \leq 1$$ und sonst 0, gilt:

$$
\int_{-1}^{1} C(1-x^2) \, dx = 1
$$

Berechne das Integral:

$$
C \int_{-1}^{1} (1-x^2) dx = 1
$$

Das Integral:

$$
\int_{-1}^{1} (1-x^2) dx = \left[ x - \frac{x^3}{3} \right]_{-1}^{1} = \left(1 - \frac{1}{3}\right) - \left(-1 + \frac{1}{3}\right) = \left(\frac{2}{3}\right) - \left(-\frac{2}{3}\right) = \frac{4}{3}
$$

Also:

$$
C \cdot \frac{4}{3} = 1 \implies C = \frac{3}{4}
$$

***

### Skizze \$ f(x) \$:

- Die Dichte ist eine nach unten geöffnete Parabel, nach oben verschoben, im Bereich $[-1,1]$ und bei $|x| = 1$ verschwindet sie.
- Maximalwert bei \$ x = 0 \$ (dort $f(0) = \frac{3}{4}$).

### b) Standardabweichung von $$X$$

Erwartungswert $$E(X)$$:

Aufgrund der Symmetrie um $$x=0$$:

$$E(X) = 0$$

Varianz:

$$\text{Var}(X) = E(X^2) - (E(X))^2 = E(X^2)$$

Berechne $$E(X^2)$$:

$$E(X^2) = \int_{-1}^{1} x^2 \cdot f(x) dx = \int_{-1}^{1} x^2 \cdot \frac{3}{4}(1-x^2) dx$$

$$= \frac{3}{4} \int_{-1}^{1} (x^2 - x^4) dx$$

$$= \frac{3}{4} \left( \int_{-1}^{1} x^2 dx - \int_{-1}^{1} x^4 dx \right)$$

$$\int_{-1}^{1} x^2 dx = \left[ \frac{x^3}{3} \right]_{-1}^1 = \frac{1}{3} - \left(-\frac{1}{3}\right) = \frac{2}{3}$$

$$\int_{-1}^{1} x^4 dx = \left[ \frac{x^5}{5} \right]_{-1}^1 = \frac{1}{5} - \left(-\frac{1}{5}\right) = \frac{2}{5}$$

Setze ein:

$$E(X^2) = \frac{3}{4} \left( \frac{2}{3} - \frac{2}{5} \right ) = \frac{3}{4} \cdot \frac{10-6}{15} = \frac{3}{4} \cdot \frac{4}{15} = \frac{1}{5}$$

Standardabweichung:

$$\sigma = \sqrt{\text{Var}(X)} = \sqrt{\frac{1}{5}} = \frac{1}{\sqrt{5}}$$

### c) Wahrscheinlichkeit, dass $$|X| < \frac{1}{2}$$:

Gesucht ist $$P(|X| < \frac{1}{2})$$:

$$P\left(-\frac{1}{2} < X < \frac{1}{2}\right) = \int_{-\frac{1}{2}}^{\frac{1}{2}} f(x) dx$$

$$= \int_{-\frac{1}{2}}^{\frac{1}{2}} \frac{3}{4}(1-x^2) dx$$

Da die Funktion symmetrisch ist, genügt das Doppelte des Integrals von 0 bis 1/2:

$$= 2 \cdot \int_{0}^{\frac{1}{2}} \frac{3}{4}(1-x^2) dx$$

$$= \frac{3}{2} \int_{0}^{\frac{1}{2}} (1-x^2) dx$$

$$\int (1-x^2) dx = x - \frac{x^3}{3}$$

Eingesetzt:

$$\int_{0}^{\frac{1}{2}} (1-x^2) dx = \left[x - \frac{x^3}{3}\right]_0^{1/2} = \frac{1}{2} - \frac{1}{3} \cdot \left(\frac{1}{8}\right) = \frac{1}{2} - \frac{1}{24} = \frac{11}{24}$$

Somit:

$$P\left(|X| < \frac{1}{2}\right) = \frac{3}{2} \cdot \frac{11}{24} = \frac{33}{48}$$

***
