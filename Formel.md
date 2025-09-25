# Kombinatorik

| Menge            | Name         | Reihenfolge | mit/ohne Wiederholung | Formel                                     |Verwendung |
|------------------|--------------|-------------|-----------------------|--------------------------------------------|-----------|
| alle Elemente    | Permutation  | ja          | ohne Wiederholung (ohne Zurücklegen)     | $$n!$$       | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md), [Schachspiel](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md#beim-schachspiel-kann-ein-turm-nur-vertikal-oder-horizontal-ziehen-beziehungsweise-schlagen-wir-betrachten-nun-ein-verallgemeinertes-schachbrett-mit-nn-feldern-wie-viele-m%C3%B6glichkeiten-gibt-es-n-ununterscheidbare-t%C3%BCrme-so-auf-diesem-brett-zu-verteilen-dass-keiner-einen-anderen-bedroht-in-jeder-horizontalen-reihe-und-jeder-vertikalen-linie-darf-also-nur-h%C3%B6chstens-ein-turm-stehen) |
| alle Elemente    | Permutation  | ja          | mit Wiederholung      | $$\frac{n!}{(n₁! · n₂! · ... · nₙ!)}$$       | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Variation    | ja          | ohne Wiederholung     | $$\frac{n!}{(n - k)!}$$                     | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Variation    | ja          | mit Wiederholung      | $$n^k$$                                   | [Buchstabensalat](https://github.com/ab2274205/WuK/blob/main/Kombinatorik.md) |
| Stichprobe (k)   | Kombination  | nein        | ohne Wiederholung     | $$\binom{n}{k}$$ = $$\frac{n!}{[(n - k)! · k!]}$$ (Binomialkoeffizient) | [Auswahl](https://github.com/ab2274205/WuK/blob/main/Auswahl-Kombinatorik.md) | 
| Stichprobe (k)   | Kombination  | nein        | mit Wiederholung      | $$\binom{n + k - 1}{k}$$                   ||

---

**Legende:**  
- *n* - Gesamtanzahl der Elemente in der Grundmenge
- *n₁*,*n₂*,... - Anzahl gleicher Elemente  
- *k* - Anzahl der Elemente in der Stichprobe  
