### Problem 9 – Cubic with Two Complex Roots

Let $f (x) \in \Q[x]$ be an [[Irreducible|irreducible]] cubic ([[Polynomial Degree|degree]] $3$) polynomial having exactly one real root. Let $L$ be the [[Splitting Field|splitting field]] of $f(x)$ over $\Q$. Show that $\Gal(L/\Q) \cong S_3$.

##### *Proof.*
Let $f(x) \in \Q[x]$ be an irreducible cubic (degree $3$) polynomial having exactly one real root, and let $L$ be the splitting field of $f(x)$ over $\Q$.

As $L$ is the splitting field of $f$, it is a normal extension. As $\Q$ has characteristic 0, $L$ is separable (because $L$ is algebraic extension, as its the extension caused by adjoining each root of $f$, and algebraic extensions of algebraic extensions are algebraic). Thus by we see that $|\Aut(L/\Q)|=[L:F]$.

By Proposition 2.83 we see that $\Aut(L/F)$ is isomorphic to some subgroup of $S_m$, where $m$ is the number of distinct roots of $f$. As $f$ cubic and irreducible we know that the real root must be irrational, which we will denote $\alpha$. Consider the extension $\Q(\alpha)$. As $\alpha\not\in\Q$, we see that $[\Q(\alpha):\Q]\geq 2$. However, neither of our complex roots are in this extension, and so another extension is needed to reach $L$. But this extension would also have a degree larger than $1$, so $[L:\Q]\geq4$. As $|S_2|=2$, there exists no subgroup of it that $\Aut(L/F)$ can be isomorphic to, given that $|\Aut(L/\Q)|=[L:F]$. Thus we see that $m=3$, meaning that our complex roots are distinct.

Then $|\Aut(L/F)|=1,2,3,$ or $6$, the only possible sizes of subgroups of $S_3$. However, by the previous argument we see that as $[L:\Q]\geq4$, the only viable subgroup of $S_3$ is $S_3$ itself. Thus $\Aut(L/\Q) \cong S_3$.
#qual