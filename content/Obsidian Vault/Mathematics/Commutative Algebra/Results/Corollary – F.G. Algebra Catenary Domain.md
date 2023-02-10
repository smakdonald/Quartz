#### $\cor$ – F.G. Algebra Catenary Domain
Let $R$ be a [[Algebra Finite|finitely generated]] algebra or a quotient of a power series ring over a field.
(a) $R$ is [[Catenary Ring|catenary]].
If additionally $R$ is a domain, then
(b) $R$ is [[Equidimensional Ring|equidimensional]], and
(c) $\height(I)=\dim(R)-\dim(R/I)$ for all ideals $I$.[^1]

##### *Proof.*
\begin{enumerate}[1)]
	\item Let $P \subseteq Q$ be primes in $R$. After quotient out by $P$, we can assume that $R$ is a domain and $P=0$. Fix a saturated chain $C$ from $Q$ to a maximal ideal $\m$. Given two saturated chains $C'$, $C''$ from $0$ to $Q$, the concatenations $C'|C$ and $C''|C$ are saturated chains from $0$ to $\m$, so by \Cref{Noether normalization height and dimension} they must have the same length. It follows that $C'$ and $C''$ have the same length.
	\item Equidimensionality is immediate from \Cref{Noether normalization height and dimension}.
	\item We have 
	$$\height(I) = \min\{\height(P) \mid P\in \Min(I)\}$$ 
	and 
	$$\dim(R/I) = \max\{\dim(R/P) \mid P \in \Min(I)\}.$$ 
	Therefore, it suffices to show the equality for prime ideals, since if $P \in \Min(I)$ attains $\height(I)$, which is the minimal value of $\height(Q)$ for $Q \in \Min(I)$, then it also attains the maximal value of $\dim(R/Q)$ for $Q \in \Min(I)$. Now, take a saturated chain of primes $C$ from $0$ to $P$, and a saturated chain $C'$ from $P$ to a maximal ideal $\m$. Since $R$ is catenary, $C$ has length $\height(P)$. Moreover, $C'$ has length $\dim(R/P)$ by \Cref{Noether normalization height and dimension}, and $C|C'$ has length $\dim(R)$ by \Cref{Noether normalization height and dimension}.\qedhere
\end{enumerate}

[^1]: Notation: [[Krull Dimension of a Ring]], [[Height of an Ideal]]