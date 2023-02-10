#### $\prop$ – AV Irreducible iff Coor. Integral Domain
An [[Affine Variety|affine variety]] $X$ is [[Irreducible Affine Variety|irreducible]] if and only if $A(X)$[^1] is an integral domain. More generally, the collection of irreducible affine subvarieties of a given affine variety is in bijective correspondence with the collection of [[Prime Ideal|prime ideals]] in its [[Coordinate Ring|coordinate ring]].

##### *Proof.*
If $X$ is not irreducible, then $X = Y \cup Z$ for proper closed subsets $Y$ and $Z$ of $X$. It follows that $I(X) \subsetneq I(Y)$, $I(X) \subsetneq I(Z)$[^4], and $I(X) = I(Y) \cap I(Z)$[^2]. So pick $f \in I(Y) \setminus I(X)$ and $g \in I(Z) \setminus I(X)$. Then $fg \in I(X)$, proving $I(X)$ is not [[Prime Ideal|prime]][^3].

Suppose $I(X)$ is not prime. Then there are polynomials $f$ and $g$ neither of which is in $I(X)$ and yet $fg \in I(X)$. Set $J = I(X) + \igen{f}$ and $L = I(X) + \igen{g}$ and $Y = V(J)$ and $Z = V(L)$. Then $Y \subsetneq X$, $Z \subseteq X$ and $$Y \cup Z = V(I) \cup V(L) = V(I \cdot L) = V(X)$$ since $I \cdot L = I(X)$.
  
For the second assertion, we already know there is a bijective correspondence between affine subvarieties of an affine variety $V$ and radical ideals of $A(V)$, given by $W \mapsto I(W)/I(V)$[^5]. The assertion holds since $I(W)/I(V)$ is prime in $A(V)$ if and only if $I(W)$ is prime in $k[\xdots].$[^6]

[^1]: Notation: [[Coordinate Ring]]
[^2]: As $X = Y \cup Z$, we see $I(X) = I(Y) \cap I(Z)$ from this [[Proposition – Unions of Vanishing Sets|Proposition]].
[^3]: Our coordinate ring is a [[Quotient Ring|quotient]] of a [[Polynomial Ring|polynomial ring]] by $I(X)$. This [[Theorem – Prime, Maximal, Domain, Field|Theorem]] tells us that $A(X)$ is an integral domain if and only if $I(X)$ is prime. 
[^4]: Notation: [[Vanishing Set]].
[^5]: This comes from the [[Corollary – Relative Nullstellensatz|Relative Nullstellensatz]].
[^6]: I'm pretty sure this is from the Lattice Isomorphism Theorem.