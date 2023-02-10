#### $\prop$ – Abelian Galois Group
Given a [[Field|field]] $E$ of [[Mathematics/Modern Algebra/Definitions/Ring Characteristic|characteristic]] zero, let $L$ be the [[Splitting Field|splitting]] field of $x^m - 1$ for some $m \geq 1$. Then $\Gal(L/E)$[^1] is [[Abelian Group|abelian]].

##### *Proof.*
For simplicity, assume $E \subseteq \C$. Then $L = E(\zeta_m)$ where $\zeta_m = e^{2\pi i/m}$. Note that for each $\s \in \Gal(L/E)$ we have $\s(\zeta_m) = \zeta_m^j$ for some $0 \leq j \leq m-1$. Moreover, since $\zeta_m^j$ must also be a primitive $m$-th root of unity, we have  $\gcd(j, m) = 1$.

The result follows from the \begin{quote}
\em Claim}: The function $\phi: \Gal(L/E) \to (\Z/m)^\times$ given by $\phi(\s) = j$ where $j$ is the unique integer such that $1 \leq j \leq m$ and $\s(\zeta_m) = \zeta_m^j$  is an injective group homomorphism.\end{quote}

\begin{proof}[Proof of Claim] As noted above, $\phi$ is well-defined, since if     $\s(\zeta_m) = \zeta_m^j$  then $\gcd(j,n)$ must be $1$. For $\s, \tau \in \Gal(L/E)$, say $\s(\zeta_m) = \zeta_m^i$ and $\tau(\zeta_m) = \zeta_m^j$. Then $$\s(\tau(\zeta_m)) =\s(\zeta_m^{j})= \s(\zeta_m)^j = \zeta_m^{ij}$$and hence $\phi(\s \tau) = ij = \phi(\s) \phi(\tau)$. This proves $\phi$ is a group homomorphism. It is injective since if $\phi(\s) = 1$ then $\s(\zeta_m) = \zeta_m$ and, since $\zeta_m$ generates the field extension, we have $\s = \id.$
\end{proof}

This proves the Claim and it follows that $\Gal(L/E)$ is isomorphic to a subgroup of an abelian group and hence is abelian. 
***

[^1]: See: [[Galois Extension|Galois Group]]