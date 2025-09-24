# Kombinatorik

| Menge            |              | Reihenfolge | mit/ohne Wiederholung | Formel                                     |
|------------------|--------------|-------------|-----------------------|--------------------------------------------|
| alle Elemente    | Permutation  | ja          | ohne Wiederholung     | n!                                         |
| alle Elemente    | Permutation  | ja          | mit Wiederholung      | n! / (n₁! · n₂! · ... · nₙ!)               |
| Stichprobe (k)   | Variation    | ja          | ohne Wiederholung     | n! / (n - k)!                              |
| Stichprobe (k)   | Variation    | ja          | mit Wiederholung      | n^k                                        |
| Stichprobe (k)   | Kombination  | nein        | ohne Wiederholung     | C(n, k) = n! / [(n - k)! · k!] (Binomialkoeffizient) |
| Stichprobe (k)   | Kombination  | nein        | mit Wiederholung      | C(n + k - 1, k)                            |

---

**Legende:**  
- *n* - Gesamtanzahl der Elemente in der Grundmenge
- *n₁*,*n₂*,... - Anzahl gleicher Elemente  
- *k* - Anzahl der Elemente in der Stichprobe  
