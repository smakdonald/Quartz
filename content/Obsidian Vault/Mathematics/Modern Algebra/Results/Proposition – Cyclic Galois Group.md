#### $\prop$ – Cyclic Galois Group
Given a [[Field|field]] $E$ of [[Mathematics/Modern Algebra/Definitions/Ring Characteristic|characteristic]] zero, let $L$ be the [[Splitting Field|splitting field]] of $x^m - a$ for some $m \geq 1$ and $a \in E$ and assume that that $E$ contains all $m\th$ roots of $1$. Then $\Gal(L/E)$[^1] is a [[Cyclic|cyclic]] [[Group|group]].

##### *Proof.*
Again assume $E$ and $L$ are in $\C$ for simplicity. Let $\a$ be any one root of $x^m - a$ in $L$, then the others are $\zeta_m^i \a$ with $0 \leq i \leq m-1$. Since $E$ contains $\zeta_m^i$ for all $i$, by assumption, we have $L = E(\a)$. For $\s \in \Aut(L/E)$ we have $\s(\a) = \zeta_m^i \a$ for some $0 \leq i \leq m-1$. The result follows from the
\begin{quote}{\em Claim}:
The function $\psi: \Gal(L/E) \to \Z/m$ given by sending $\a$ to $i$ where $\s(\a) = \zeta_m^i \a$ is an injective group homomorphism.
\end{quote}

\begin{proof}[Proof of Claim]
For $\s, \tau \in \Gal(L/E)$, say $\s(\a) = \zeta_m^i \a$ and $\tau(\a) = \zeta_m^j \a$. Then $$\s(\tau(\a)) = \s(\zeta_m^j\a) = \s(\zeta_m)^j(\s(\a)) =\zeta_m^j(\s(\a)) =
\zeta_m^{j+i}(\a).$$(Note that $\s(\zeta_m) = \zeta_m$ since we are assuming $\zeta_m \in E$.) This shows that $\psi(\s \tau) = \psi(\s) \psi(\tau)$ and thus $\psi$ is a group homomorphism. It is injectice since if $\psi(\s) = 0$ then $\s(\a) = \a$ and, since $\a$ generates the field extension, we have $\s = \id$.
\end{proof}

By the Claim $\Gal(L/E)$ is isomorphic to a subgroup of a cyclic group and hence is cyclic. 
***

[^1]: See: [[Galois Extension|Galois Group]]