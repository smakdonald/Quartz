#### $\thm$ – Hilbert’s Basis Theorem
If $R$ is a [[Noetherian Ring|noetherian ring]], then the [[Polynomial Ring|polynomial rings]] $R[x_1,\dots,x_d]$ and $R\llbracket x_1,\dots,x_d\Rbracket$ are noetherian for any $d \geqslant 1$.

##### *Proof.*
We will give the proof for polynomial rings, and at the end we will indicate what the difference is in the argument for the power series ring case. First, note that by induction on $d$, we can reduce to the case $d=1$. 

Given an ideal $I\subseteq R[x]$, consider the set of leading coefficients of all polynomials in $I$,
$$J :=  \{ a \in R \ \mid  \ \textrm{there is some } a x^n + \text{lower order terms (with respect to }x) \in I\}.$$
We can check (exercise!) that this is an ideal of $R$. Since $R$ is noetherian, \Cref{Noetherian properties} says that $J$ is finitely generated, so let $J = (a_1,\dots,a_t)$. Pick $f_1,\dots,f_t\in R[x]$ such that the leading coefficient of $f_i$ is $a_i$, and set $N=\displaystyle\max_i \{\deg{f_i} \}$.

Let $f \in I$. The leading coefficient of $f$ is an $R$-linear combination of $a_1, \ldots, a_t$. If $f$ has degree greater than $N$, then we can cancel off the leading term of $f$ by subtracting a suitable combination of the $f_i$. Therefore, any $f \in I$ can be written as $f = g+ h$ for some $h \in (f_1, \ldots, f_t)$ and $g \in I$ with degree at most $N$. In particular, note that $g \in I \cap (R + Rx + \cdots + R x^N)$. Since $I \cap (R + Rx + \cdots + R x^N)$ is a submodule of the finitely generated free $R$-module $R + Rx + \cdots + R x^N$, it must also be finitely generated as an $R$-module. Given such a generating set, say $I \cap (R + Rx + \cdots + Rx^N) = (f_{t+1}, \ldots, f_s)$, we can write any element $f \in I$ as an $R[x]$-linear combination of these generators $f_{t+1}, \ldots, f_s$ and the original $f_{1}, \ldots, f_t$. Therefore, $I = (f_1, \ldots, f_t, f_{t+1}, \ldots, f_s)$ is finitely generated as an ideal in $R[x]$, and $R[x]$ is a noetherian ring.

In the power series case, take $J$ to be the set of coefficients of \emph{lowest degree} terms.

[^1]: See: [[Polynomial Ring]]