#### $\lem$ – Properties of Dimension and Height
Let $R$ be a ring.
(a) A [[Prime Ideal|prime]] has [[Height of an Ideal|height]] zero if and only if it is a [[Minimal Prime|minimal prime]] of $R$.
(b) An ideal has height zero if and only if it is contained in a minimal prime of $R$. In particular, in a domain, every nonzero ideal has positive height.
(c) $\dim(R) = \sup \{ \dim(R/P) \mid P \in \Spec(R) \} = \sup\{ \dim(R/P) \mid P \in \Min(R) \}$[^1].
(d) $\dim(R) = \sup \{ \height(P) \mid P \in \Spec(R) \}=\sup\{ \mathrm{height}(Q) \mid Q \in \mSpec(R) \}$.
(e) If $I$ is an ideal, then $\dim(R/I) = \sup \{ n \mid \exists P_0 \subsetneq P_1  \subsetneq \cdots \subsetneq P_n, P_i \in V(I) \}$.
(f) If $P$ is prime, $$\dim(R/P) + \height(P) \leqslant \dim(R).$$
(g) If $I$ is an ideal, $$\dim(R/I) + \height(I) \leqslant \dim(R).$$
(h) If $W$ is a [[Multiplicatively Closed Set|multiplicative set]], then $\dim(W^{-1}R) \leqslant \dim(R)$[^2].
(i) If $P$ is prime, then $\height(P)=\dim(R_P)$.
(j) If $P \subseteq Q$ are primes, then $\dim(R_Q/ P R_Q)$ is the supremum of the lengths of [[Saturated Chain of Primes|saturated chains of primes]] in $R$ of the form $P = P_0 \subsetneq P_1  \subsetneq \cdots \subsetneq P_n = Q$.

##### *Proof.*
We will prove some of these and leave the rest as an exercise.
\begin{enumerate}[(1)]
	\item A prime has height $0$ if and only if it contains no other prime, which is equivalent being a minimal prime of $R$.

\item If $I$ is contained in a minimal prime $Q$ of $R$, then $\height(Q)=0$ by (1), so $\height(I)=0$ by definition. Conversely, if $\height(I)=0$, by definition, there is a minimal prime of $I$ of height $0$, so some minimal prime of $I$ is a minimal prime of $R$, so $I$ is contained in a minimal prime of $R$.

\setcounter{enumi}{5}

\item It suffices to show that if $\dim(R/P) \geqslant a$ and $\height(P) \geqslant b$ then $\dim(R) \geqslant a+b$. By definition, $\height(P) \geqslant b$ means that there is a chain of primes 
$$Q_0 \subsetneq Q_1 \subsetneq \cdots \subsetneq Q_b = P.$$ 
By (5), $\dim(R/P) \geqslant a$ means that there is a chain of primes 
$$\mathfrak{a}_0 \subsetneq \mathfrak{a}_1 \subsetneq \cdots \subsetneq \mathfrak{a}_a$$
with $\mathfrak{a}_0 \supseteq P$. We can assume without loss of generality that $\mathfrak{a}_0 = P$, since if not, we can add it to the bottom of the chain. Putting these chains together, we get a chain of length $a+b$ in $\Spec(R)$, so $\dim(R) \geqslant a+b$.

\item Let $\dim(R/I) \geqslant a$ and $\height(I) \geqslant b$. The inequality $\height(I) \geqslant b$ means that for every minimal prime $P$ of $I$, $\height(P) \geqslant b$. The inequality $\dim(R/I) \geqslant a$ implies that there exists a minimal prime of $P$ of $I$ such that $\dim(R/P) \geqslant a$. For such a minimal prime as in the latter statement, using (5), we get the desired conclusion.

[^1]: Notation: [[Krull Dimension of a Ring]], [[Prime Spectrum]]
[^2]: Notation: [[Localization]]