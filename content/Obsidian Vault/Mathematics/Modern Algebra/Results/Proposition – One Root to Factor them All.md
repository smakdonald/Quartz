#### $\prop$ – One Root to Factor them All
Suppose $F \subseteq L$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] and $f(x)\in F[x]$[^1] is an [[Irreducible|irreducible]] polynomial. If $F \subseteq L$ is a [[Normal Extension|normal]] extension and $f$ has at least one root in $L$, then $f$ factors completely in $L$.

##### *Proof.*
Say $L$ is the splitting field of $g(x) \in F[x]$. Let $K$ be the splitting field of $g(x) \cdot f(x)$. So $F \subseteq L \subseteq K$. Say $\a$ is a root of $f$ that belongs to $L$, and let $\beta \in K$ be any other root. We aim to prove $\beta \in L$. 

Recall that we know that if $E$ is a splitting field over $F$ of an {\em irreducible} polynomial, then $\Aut(E/F)$ acts transitively on the roots of this polynomial. Something more general is true: If $E$ is the splitting field over $F$ of some possibly reducible polynomial $h(x)$, then for each irreducible factors $p(x)$, $\Aut(E/F)$ acts transitively on the roots of $p(x)$. I won't prove this, but will apply it to $F \subseteq K$. Since $f(x)$ is irreducible, we get that there is there a $\s \in \Aut(K/F)$ such that $\s(\a) = \beta$. Let $c_1, \dots, c_m \in L$ be all the roots of $g$, so that $L = F(c_1, \dots, c_m)$. Since $\s$ fixes $F$, it must permute these roots. In particular, $\s(L) \subseteq L$. But then $\beta = \s(\a) \in L$. 
***

[^1]: See: [[Polynomial Ring]]