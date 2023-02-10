#### Lemma – Regular Functions on all of Affine Space
Every regular function $\a$ defined on all of $\A^n_k$ is given by some polynomial $f$.

##### *Proof.*
We start by proving that if a polynomial $f$ is identically $0$ on a non-empty open subset $V$ of $\A^n_k,$ then $f$ is the $0$ polynomial. To see this, note that we may assume $V = D(g)$ for some non-constant polynomial $g$. Then $D(g) \subseteq V(f)$. This means that for every maximal ideal $\fm = (x_1 - a_1, \dots,x_n - a_n)$ of $k[x_1, \dots, x_n]$, if $g \notin \fm$ then $f \in \fm$. This means that the image of $f$ in  the ring $k[x_1, \dots, x_n][1/g]$ is contained in every maximal ideal.....

Now say $\a: \A^n_k \to \A^1_k$ is a regular function. For each point $P \in \A^n_k$, let $f_P, g_P$ be polynomials and $U_p$ be an open neighborhood of $P$ in $\A^n_k$ such that $\a(P) = \frac{f_P(Q)}{g_P(Q)}$ for all $Q \in U_P$. Since $\A^n_k$ is irreducible, for any two points $P_1$ and $P_2$ we have that $V := U_{P_1} \cap U_{P_3} \ne \emptyset$. On this set, the functions $\frac{f_1}{g_1}$ and $\frac{f_2}{g_2}$ agree; i.e., $f_1 g_2 - f_2 g_1$ is identically $0$ on $V$. By what was shown above $f_1g_2 = f_2 g_1$. ....