#### $\prop$ – Automorphisms and Finite Extension Degree
If $F \subseteq L$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]], then $|\Aut(L/F)| \leq [L : F]$[^1].

##### *Proof.*
We proceed by induction on $[L:F]$. When $[L:F]=1$, we have $L = F$ and $\Aut(L/F)$ is the one element group.

For $[L: F] > 1$,  pick $\a \in L \setminus F$ and let $p(x) = m_{\a, F}(x)$. Consider the extension $F \subseteq F(\a)$.
Note that $H = \Aut(L/F(\a))$ is a subgroup of  $G = \Aut(L/F)$, by definition. By induction we have $|H| \leq [L: F(\a)]$.  Using the degree formula and the fact that $|G| = |H| \cdot [G:H]$, it suffices to prove $[G:H] \leq [F(\a):F]$. This follows from:

{\em Claim:} Let $R$ be the set of roots of $p(x)$ that belong to $L$. Then the function
$$\begin{equation}
\theta: G/H  \to R
\end{equation}$$
given by $\theta(gH) = g(\a)$ is well-defined and injective. (Note: $H$ is not necessarily normal, and so $G/H$ isn't a group. By $G/H$ I just mean the {\em set} of left cosets of $H$ in $G$.)

\begin{proof}
By Proposition \ref{prop423}, for each $g \in G$ we have $g(\a) \in R$. Moreover, by definition of $H$, for all $h \in H$, we have $h(\a) = \a$ and hence $gh(\a)=g(h(\a))=g(\a)$. This proves $\theta$ is a
well-defined function (i.e., it is independent of left coset representative). For $g_1, g_2 \in G$, if $g_1(\a) = g_2(\a)$ then $g_2^{-1}g_1(\a) = \a$ which implies $g_2^{-1}g_1 \in H$ (since if an automorphism of $L$ fixes $F$ and $\a$ then it fixes $F(\a)$). Thus $g_1(\a) = g_2(\a)$ implies $g_1H = g_2H$ and hence $\theta$ is one-to-one.
***

[^1]: For $|G|$, See: [[Order]]. For $\Aut$, See: [[Automorphism]]. For $[L:F]$, See: [[Degree of Field Extension]]
