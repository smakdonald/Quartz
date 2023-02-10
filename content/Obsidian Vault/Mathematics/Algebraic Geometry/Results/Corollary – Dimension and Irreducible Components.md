#### $\cor$ – Dimension and Irreducible Components
For any (not necessarily irreducible) [[Affine Variety|affine variety]] $X$ and $f \in A(X)$, suppose that for each irreducible component $Y$ of $X$ we have $\emptyset \subsetneq V_X(f) \cap Y \subsetneq Y$. (In words, $f$ vanishes at at least one point, and not at every point, of each irreducible component.) Then $\dm V_X(f) = \dm(X) - 1$.

##### *Proof.*
Since $V_X(f) = \bigcup_i (V_X(f) \cap X_i)$ we have $$\begin{equation} \dm V_X(f) = \max \{ \dm V_X(f) \cap X_i\}.\end{equation}$$For any $i$ such that $\emptyset \subsetneq V_X(f) \cap X_i  \subsetneq X_i$ the Theorem applies (using that  $V_X(f) \cap X_i = V_{X_i}(f)$) to give that  $V_X(f) \cap X_i$ is equidimensional of dimension equal to $\dm(X_i) -1$. If $1 \leq i \leq k$, then by assumption we have $\dm(X_i) = \dm(X)$ and either (a) $V_X(f) \cap X_i = \emptyset$ or (b) $\emptyset \subsetneq V_X(f) \cap X_i  \subsetneq X_i$, and moreover condition (b) holds for at least one such $i$.

It follows that $\max \{ \dm V_X(f) \cap X_i \mid 1 \leq i \leq k\} =\dm(X) - 1$. If $i > k$, then $\dm (V_X(f) \cap X_i) \leq \dm(X_i) \leq \dm(X) - 1$. The first assertion thus follows from the equation above.

If $k = m$, then for each $i$ we have that $V_X(f) \cap X_i$ is either empty or is equidimensional of dimension $\dm(X) -1$, and it is non-empty for at least one $i$. The second assertion follows.