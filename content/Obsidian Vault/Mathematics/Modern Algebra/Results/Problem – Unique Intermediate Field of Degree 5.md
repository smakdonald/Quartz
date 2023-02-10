### Problem 4 – Unique Intermediate Field of Degree 5
Let $L/F$ be a [[Degree of Field Extension|finite]] [[Galois Extension|Galois field extension]] of [[Degree of Field Extension|degree]] $45$. Prove there exists a unique [[Intermediate Field|intermediate field]] $E$ (i.e., $F \sse E \sse L)$ such that $[E : F ] = 5$[^1].

##### *Proof.*
Let $F \subseteq L$ be a finite Galois field extension of degree $45$. 

Note that as $45=5\cdot 9$, we see that the number of Sylow-$5$ subgroups of $G$ divides $9$ and is congruent to $1\mod{5}$. Thus there is exactly one Sylow-$5$ subgroup of $G$, which we denote $H$. By the Fundamental Theorem of Galois Theory, $H$ corresponds to an intermediate field extension $E$. Note that as $H$ has order 5, we see that $[G:H]=9$, and thus $[L:E]=9$ as well. By the Degree Formula we see that $[L:F]=[L:E][E:F]$. As $[L:F]=45$ and $[L:E]=9$, we see that $[E:F]=5$, as desired. As $E$ corresponds to the unique subgroup of $G$ or order 5, we see that this extension must be unique as well.

#qual

[^1]: Notation: [[Degree of Field Extension]]