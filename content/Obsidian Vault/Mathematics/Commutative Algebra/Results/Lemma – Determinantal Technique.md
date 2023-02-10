#### $\lem$ – Determinantal Technique
Let $R$ be a ring, $B \in M_{n\times n}(R)$, $v\in R^n$, and $r\in R$.
(a) $\mathrm{adj}(B) B = \det(B) I_{n\times n}$.[^1]
(b) If $B v = r v$, then $\det(r I_{n\times n} - B) v=0$.

##### *Proof.*
(a) When $R$ is a field, this is a basic linear algebra fact. We will deduce the case of a general ring from the field case. The ring $R$ is a $\Z$-[[Algebra|algebra]],[^2] so we can write $R$ as a [[Quotient Ring|quotient]] of some polynomial ring $\Z[X]$.[^3] Let $\psi:\Z[X]\to R$ be a surjection, $a_{ij}\in \Z[X]$ be such that $\psi(a_{ij})=b_{ij}$, and let $A=[a_{ij}]$. Note that $$\psi(\mathrm{adj}(A)_{ij})=\mathrm{adj}(B)_{ij} \quad \textrm{ and } \quad \psi((\mathrm{adj}(A) A)_{ij}) = (\mathrm{adj}(B) B)_{ij},$$since $\psi$ is a homomorphism, and the entries are the same polynomial functions of the entries of the matrices $A$ and $B$, respectively. Thus, it suffices to establish $$\mathrm{adj}(B) B = \det(B) I_{n\times n}$$in the case when $R=\Z[X]$, and we can do this entry by entry. Now, $R=\Z[X]$ is an integral domain, hence a subring of a field (its [[Field of Fractions|fraction field]]). Since both sides of the equation 
$$\left( \mathrm{adj}(B) B \right)_{ij} = \left( \det(B) I_{n\times n}\right)_{ij}$$
live in $R$ and are equal in the fraction field (by linear algebra) they are equal in $R$. This holds for all $i, j$, and thus 1) holds.
(b) By assumption, we have $(r I_{n\times n} - B) v=0$, so by part 1)$$\det(r I_{n\times n} - B) v=\mathrm{adj}(r I_{n\times n} - B) (r I_{n\times n} - B) v = 0.$$

[^1]: Notation: [[Classical Adjoint]], [[Determinant]]
[^2]: See example
[^3]: This needs some fleshing out. It comes from the definition of a free algebra and modding out by the kernel 