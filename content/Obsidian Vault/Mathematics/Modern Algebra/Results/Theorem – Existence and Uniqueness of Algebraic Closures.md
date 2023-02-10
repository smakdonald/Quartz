#### $\thm$ – Existence and Uniqueness of Algebraic Closures
For any [[Field|field]] $F$, there exists an [[Algebraic Closure|algebraic closure]] of $F$. If $L$ and $L'$ are two algebraic closures of the same field $F$, then there exists a field [[Isomorphism|isomorphism]] $\phi: L \xra{\cong} L'$ such that $\phi|_F = \id_F$ (i.e., $\phi(a) = a$ for all $a \in F$).

##### *Proof.*
Fake Proof of Existence

Let $\cS$ be the collection of all algebraic field extensions of $F$. Make $\cS$ into a poset by declaring $L \leq L'$ iff $L \subseteq L'$.  We prove $\cS$ has a maximal element.

Let $\cT$ be any totally ordered subset of $\cS$. If $\cT$ is empty, then $F \in \cS$ is an upper bound for $\cT$. If $\cT$ is non-empty, set $K := \cup_{E \in \cT} E$. Using that $\cT$ is totally ordered, it is not hard to see that $K$ is indeed a field. It clearly contains $F$ as a subfield and every element of it is algebraic over $F$. So $K \in \cS$ and it is  an upper bound for $\cT$. By Zorn's Lemma, $\cS$ has a maximal member $L$.

By construction $L$ is algebraic over $F$.  If $L$ were not algebraically closed, then there would be
a non-trivial algebraic extension $L \subsetneq E$ of it, by Proposition \ref{prop412}. But then $F \subseteq E$ is algebraic by Proposition \ref{prop:algebraictower}, and this contradicts the maximality of $L$.

Why is this only a fake proof? It's because $\cS$, as we've defined it, is not a {\em set} but rather it is something bigger than that. Zorn's Lemma only applies to po{\em sets}. How annoying!
***