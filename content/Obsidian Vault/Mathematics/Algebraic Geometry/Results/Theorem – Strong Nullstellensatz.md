#### Theorem – Strong Nullstellensatz
Assume $k$ is an [[Algebraically Closed|algebraically closed]] field. Then both of the containments in this [[Proposition – Compositions of Vanishing Sets and Zero Loci|Proposition]] are actually equalities: $$I(V (J)) = J\text{ for any radical ideal }J\text{ and }V (I(W)) = W \text{ for any affine variety }W$$Thus, there is a order-reversing bijection between the [[Poset and Lattice|poset]] (under containment) of all [[Affine Variety|affine varieties]] in $\A^n_k$[^1] and the poset (under containment) of all [[Radical Ideal|radical]] ideals in $k[x_1,\dots,x_n]$[^2].

##### *Proof.*
Let $L$ be the ideal of $k[x_1, \dots, x_n, y]$ [[Generator|generated]] by (the image of) $J$ and $1 - yf(x_1, \dots, x_n)$. 
I claim $V(L)$ is the empty set: If $(a_1, \dots, a_n, b) \in V(L)$ then $(a_1, \dots, a_n) \in V(J)$ and so $f(a_1, \dots, a_n) = 0$. But we also have $b f(a_1, \dots, a_n) = 1$, which is impossible.

By the [[Corollary – Weak Nullstellensatz|Weak Nullstellensatz]], $L = \igen{1}$.

Now, by this [[Lemma – Algebras and Localizations|Lemma]] there is an [[Isomorphism|isomorphism]]
$$
\frac{(k[x_1, \dots, x_n]/J) [ y]}{(1 - yf)} \xra{\cong}
S^{-1} k[x_1, \dots, x_n]/J 
$$
of commutative rings,  where $S = \{f^m \mid m \geq 1\}$. We also have the canonical isomorphism
$$
(k[x_1, \dots, x_n]/J)[ y]/(1 - yf) \cong k[x_1, \dots, x_n, y]/L.
$$
Since $L = \igen{1}$, this proves that $S^{-1} (k[x_1, \dots, x_n]/J)$ is the trivial ring, and hence $\frac{1}{1} = \frac{0}{1}$ in this ring. Thus $f^m = 0$ in $k[x_1, \dots, x_n]/J$ for some $m$. We have proven that $I(V(J)) = J$ for any radical ideal $J$.

For the other assertion, let $W$ be any affine variety in $\A^n_k$. Then by Proposition \ref{prop121a} we have  $W = V(J)$ for some radical ideal $J$. By what has already been proven we have $I(V(J)) = J$ and hence $$V(I(W)) = V(I(V(J)) = V(J) = W.$$
***

[^1]: Notation: [[Affine Space]]
[^2]: Notation: [[Polynomial Ring]]