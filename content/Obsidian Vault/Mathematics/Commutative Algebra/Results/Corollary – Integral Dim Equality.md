#### $\cor$ – Integral Dim Equality
If $R\subseteq S$ is [[Integral Element|integral]], then $\dim(R)=\dim(S)$[^1].

##### *Proof.*
We have already shown that $\dim(S) \leqslant \dim(R)$ in \Cref{integral dim inequality}, so we just need to show that $\dim(R) \leqslant \dim(S)$. Fix a chain of primes $P_0 \subsetneq \cdots \subsetneq P_n$ in $\Spec(R)$. By Lying Over, \Cref{lying over}, there is a prime $Q_0 \in \Spec(S)$ contracting to $P_0$. Then by Going up, \Cref{going up}, we have $Q_0 \subsetneq Q_1$ with $Q_1 \cap R = P_1$. Continuing, we can build a chain of distinct primes in $S$ of length $n$. So $\dim(R) \leqslant \dim(S)$, and equality follows.

[^1]: Notation: [[Krull Dimension of a Ring]]