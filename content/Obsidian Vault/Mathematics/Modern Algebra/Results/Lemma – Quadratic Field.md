#### $\lem$ – Quadratic Field
Let $d$ be a squarefree integer (that is, the prime factorization of $d$ has no repeated primes). Then the subset $$\Q(\sqrt {d}) = \{a + b\sqrt{d} \mid a,b \in \Q\}$$ of $\C$ is a [[Subring|subring]] that is a [[Field|field]] (called a *quadratic field*), and $\Z[\sqrt{d}] = \{a + b\sqrt{d} | a,b \in \Z\}$ is a subring of $\Q(\sqrt{d})$.

###### *Proof.* 
Both $\Q(\sqrt {d})$ and $\Z[\sqrt{d}]$ are closed under subtraction and multiplication, so they are subrings of $\C$.

The fact that $\Q(\sqrt {d})$ is a {\em subfield} follows since $\Q(\sqrt {d})$ is also closed under taking inverses. Indeed the inverse of $r + q \sqrt{d}$ (from $\C$) turns out to be 
$$
(r + q \sqrt{d})^{-1} = \frac{r - q \sqrt{d}}{r^2 - d q^2} \in \Q(\sqrt {d})
$$
whenever $r + q \sqrt{d}\neq 0$. A slightly subtle point here is that the fraction above makes sense since $r^2 -d q^2 \ne 0$ provided $r$ and $q$ are not simultaneously $0$. This is because, if $r^2 -d q^2 = 0$ then either $d=(r/q)^2$, which contradicts the assumption that $d$ is squarefree, or $r=q=0$, which contradicts the assumption $r + q \sqrt{d}\neq 0$.
***