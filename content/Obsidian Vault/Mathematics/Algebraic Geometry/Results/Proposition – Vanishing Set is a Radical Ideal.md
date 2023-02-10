#### Proposition – Vanishing Set is a Radical Ideal
For any subset $W$ of $\A^n_k$[^1], $I(W)$[^2] is a [[Radical Ideal|radical]] ideal in $k[x_1,\dots,x_n]$[^3].

##### *Proof.*
If $g\in I(W)$ and $f\in k[x_1,\dots,x_n]$ then for all $P\in I(W)$ we have $$(fg)(P) = f(P)g(P) =  f(P)0 = 0$$and hence $fg\in I(W)$. Similarly one shows $I(W)$ is closed under addition. Since $0\in I(W)$, $I(W)$ is an ideal. If $f^{n}\in I(W)$ for some $n\geq1$, then for all $P\in W$ we have $0=(fn)(P)=(f(P))^{n}$ and hence $f(P) = 0$. So $f\in I(W)$, and this proves $I(W)$ is radical.

[^1]: Notation: [[Affine Space]]
[^2]: Notation: [[Vanishing Set]]
[^3]: Notation: [[Polynomial Ring]]