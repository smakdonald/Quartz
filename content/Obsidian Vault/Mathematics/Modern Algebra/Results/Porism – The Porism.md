#### Porism – *The* Porism
If $L$ is the [[Splitting Field|splitting]] [[Field|field]] over $F$ of an [[Irreducible|irreducible]] polynomial $f(x) \in \F[x]$ and if $\a, \beta \in L$ are any two roots of $f$, then there is a field [[Automorphism|automorphism]] $\s: L \xra{\cong} L$ such that $\s|_F = \id_F$ and $\s(\a) = \beta$.

##### *Proof.*
We basically already proved this, but since it is of large importance, let's do so again:

Since $\a, \beta$ are roots of the same irreducible polynomial, by Corollary \ref{cor410} there is an isomorphism $\tau: F(\a) \to F(\beta)$ such that $\tau|_F = \id_F$ and $\tau(\a) = \beta$. We have two field maps, $F(\a) \into L$ (actual inclusion) and the composition of $F(\a) \xra{\tau} F(\beta)\into L$, and they realize $L$ as the splitting field of $f(x)$ over $F(\a)$ in two different ways. Since splitting fields are unique, an isomorphism such as $\s$ exists.
***