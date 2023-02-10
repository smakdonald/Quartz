#### $\thm$ – Fermat’s Two-Square Lemma
For every prime $p \equiv 1 \mod 4$, there exist unique (up to sign and ordering) $a, b \in\Z$ such that $p = a^{2} + b^{2}$.

##### *Proof.*
Suppose p is a rational prime congruent to 1 
(\mod 4). We show that p is not a Gaussian prime. By Lagrange’s Lemma, we can 
choose m so that p | m2 + 1. In \Z[i], we factor 
m2 + 1 = (m + i)(m - i). 
Suppose p were a Gaussian prime. Then by the Prime Divisor Property in \Z[i], since 
p | m2 + 1, either p | m + i or p | m - i. However, p does not divide either of 
these since m 
p \pm 1 
p /\in\Z[i]. Thus p is not a Gaussian prime, so by Theorem 5.2.12, 
p = a^{2} + b^{2} for some a, b \in\Z. 
To prove uniqueness, suppose p = a^{2} +b^{2} = c^{2} +d2. It follows that (a +bi)(a - 
bi) = (c + di)(c - di) in \Z[i]. Since all four of these factors have norm p, they are 
all prime, and hence by unique factorization in \Z[i], must be associates of one of
another. Running through the units we find (a, b) = (\pmc, \pmd) or (a, b) = (∓d, \pmc). 
In all cases, {a^{2}, b^{2}} = {c^{2}, d2}.