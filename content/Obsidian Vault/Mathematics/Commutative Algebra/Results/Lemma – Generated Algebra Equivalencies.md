#### $\lem$ – Generated Algebra Equivalencies #ask
The following are equivalent:
(a) $\Lambda$ [[Generated Algebra|generates]] $S$ as an $R$-[[Algebra|algebra]].
(b) Every element in $S$ admits a polynomial expression in $\Lambda$ with coefficients in $\phi(R)$, i.e.
$$S = \left\{\sum_{\mathrm{finite}} \phi(r_{i_1, \ldots, i_n}) \lambda_1^{i_1} \cdots \lambda_n^{i_n} \mid r_l \in R, \lambda_j\in\Lambda, i_j \geqslant 0 \right\}.$$
(c) If $R[X]$ is a [[Polynomial Ring|polynomial ring]] on a set of indeterminates $X$ in bijection with $\Lambda$, then the $R$-algebra homomorphism$$
\begin{CD}
R[X]^{n}@>\pi>> S\\\\
x_{i}@>>> \l_{i}
\end{CD}$$is surjective.

##### *Proof.*
Let $S= \left\{\sum_{\mathrm{finite}} \phi(a) \lambda_1^{i_1} \cdots \lambda_n^{i_n} \mid a\in A, \lambda_j\in\Lambda, i_j\in \N\right\}$.

###### (b $\Longleftrightarrow$ c)

For the equivalence between b) and c), we note that $S$ is the [[Image|image]] of $\pi$. In particular, $S$ is a subring of $R$. It then follows from the definition that a) implies b). Conversely, any subring of $R$ containing $\phi(A)$ and $\Lambda$ certainly must contain $S$, so b) implies a).