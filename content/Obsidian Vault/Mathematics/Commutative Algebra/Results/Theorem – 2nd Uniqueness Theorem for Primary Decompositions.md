#### $\thm$ – 2nd Uniqueness Theorem for Primary Decompositions
If $I$ is an ideal in a [[Noetherian Ring|noetherian ring]] $R$, then the minimal components in any [[Primary Decomposition|irredundant primary decomposition]] of $I$ are unique. More precisely, if  $$I = Q_1 \cap \cdots \cap Q_t$$ is an irredundant primary decomposition, and $\sqrt{Q_i} \in \Min(I)$[^1], then $Q_i$ is given by the formula[^2] $$Q_i = I R_{\sqrt{Q_i}} \cap R,$$which does not depend on our choice of irredundant decomposition.

##### *Proof.*
Let $Q$ be a primary ideal, and let $P$ be any prime. If $Q \subseteq P$, then $\sqrt{Q} \subseteq P$. Since the associated primes of an ideal localize well, by \Cref{associated primes localize}, $Q_P$ will still have a unique associated prime. Thus, the localization $Q_P$ is either:
	\begin{itemize}
		\item the unit ideal, if $Q \not\subseteq P$, or
		\item a primary ideal, if $Q \subseteq P$.
	\end{itemize}
Finite intersections commute with localization, by \Cref{localization commutes with finite intersection}, so for any prime $P$, $$I_{P} = (Q_1)_{P} \cap \cdots \cap (Q_t)_{P}$$is a primary decomposition, although not necessarily irredundant. Fix a minimal prime $P=P_i$ of $I$, and let $Q = Q_i$. When we localize at $P$, all the other components become the unit ideal, since their radicals are not contained in $P$, and thus $I_{P} = Q_P$. We can then contract to $R$ to get $I_{P} \cap R = (Q_i)_{P_i} \cap R = Q_i$, since $Q_i$ is $P_i$-primary and we can then apply \Cref{characterization of primary} (6).

[^1]: Notation: [[Radical Ideal]], [[Minimal Prime]]
[^2]: Notation:  [[Localization]], [[Contraction]]