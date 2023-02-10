#### Corollary – Maximal Ideals in Algebraically Closed Fields
For an [[Algebraically Closed|algebraically closed]] field $k$, every [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] ideal of $k[x_1, \dots, x_n]$ is of the form $(x_1 - a_1, \dots, x_n - a_n)$ for elements $a_1, \dots, a_n \in k$. In fact, the function $$\Psi: \A^n_k \to \mSpec k[x_1, \dots, x_n]$$sending $(a_1 \dots, a_n)$ to $(x_1 - a_1, \dots, x_n - a_n)$ is a bijection. 

##### *Proof.*
Let $F$ be the collection of all ring maps $\a: k[x_1, \dots, x_n] \to k$ such that $\a$ restricts to the identity map on the subset $k$ of $k[x_1, \dots, x_n]$. (In other words, $F$ is the set of all morphisms of $k$-algebras between these two $k$-algebras.) We show there are bijections
$$\mSpec(k[x_1, \dots, x_n]) \xra{\cong} F \xra{\cong} \A^n_k.$$
Define $\A^n_k \to F$ by sending $(a_1, \dots, a_n)$ to the evaluation map $\eval_{(a_1, \dots, a_n)}: k[x_1, \dots, x_n] \onto k$ given by $f \mapsto f(a_1, \dots, a_n)$.

It is not hard to see that this is well-defined and injective.

Given $\alpha \in F$,  set $a_i = \a(x_i)$ for each $i$. Then one may check that $\alpha = \eval_{(a_1, \dots, a_n)}$. This gives the first bijection. (Note that we didn't need that $k$ is algebraically closed for this part.) 
  
Given $\a \in F$, since $\a$ maps onto a field its [[Kernel|kernel]] is a maximal ideal. Thus we may define a function $F \to \mSpec(k[x_1, \dots, x_n])$ given by $\a \mapsto \ker(\a)$. It is not hard to see it is injective (i.e., if $\a$ and $\a'$ in $F$ have the same kernel then they are indeed the same ring map). We still have not yet used that $k$ is algebraically closed. 

Finally, let $\fm$ be any maximal ideal of $k[x_1, \dots, x_n]$. By the [[Theorem – Abstract Nullstellensatz|Abstract Nullstellensatz]], the canonical map $\phi: k \to k[x_1, \dots, x_n]/\fm$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of fields, and so, since $k$ is algebraically closed, it must be an [[Isomorphism|isomorphism]]. The composition $\alpha$ of$$k[x_1, \dots, x_n] \xora{\can}k[x_1, \dots, x_n]/\fm \xra{\phi^{-1}} k$$restricts to the identity on $k$; that is, $\a \in F$. Since $\ker(\a) = \fm$, this proves that the function $F \to \mSpec(k[x_1, \dots, x_n])$ is onto. 

To complete the proof, note that the composition
$$
\A^n_k \to F \to \mSpec(k[x_1, \dots, x_n])
$$
of the two bijections we have used does indeed send $(a_1, \dots, a_n)$ to $(x_1 - a_1, \dots, x_n - a_n)$. 
***

[^1]: Notation: [[Polynomial Ring]] 
[^2]: Notation: $\operatorname{mSpec}$ is the set of all maximal ideals of $k[x_1,\dots,x_n]$.