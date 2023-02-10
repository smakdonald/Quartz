#### $\thm$ – The Class Equation
Let $G$ be a [[Order|finite]] [[Group|group]] and let $g_1,\ldots g_r \in G$ be a list of unique representatives of all of the [[Conjugacy Class|conjugacy classes]] of $G$ of size greater than 1. Then[^1] $$|G| = |Z(G)| + \sum_i^r |G : C_G(g_i)|.$$
###### *Proof.* 
The elements of $Z(G)$ are precisely the group elements that are conjugate to only themselves; that is, they are the one-element orbits for the conjugation action. Because the conjugacy classes (orbits of the conjugation action) partition $G$ we have $$|G| = |Z(G)| + \sum_i^r [g_i]_c.$$For each $g_i$ as in the statement, by Theorem \ref{thm:conjclass}, we have $[G: C_G(g_i)] =[g_i]_c$. The class equation follows from substituting this into the equation above.
***

[^1]: See: [[Order]], [[Center]], [[Index]], [[Centralizer & Normalizer|Centralizer]]