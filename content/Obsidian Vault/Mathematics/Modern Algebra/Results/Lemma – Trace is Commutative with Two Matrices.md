#### $\lem$ – Trace is Commutative with Two Matrices
If $R$ is a [[Commutative Ring|commutative]] [[Ring|ring]] and $X \in \Mat_{m \times n}(R)$ and $Y \in \Mat_{n \times m}(R)$, then $\trace(XY) = \trace(YX)$[^1].

In particular, with the notation of the previous definition, $\trace(g)$ is well-defined.

###### *Proof.* 
The $(i,i)$ entry of $XY$ is $\sum_l x_{i,l} y_{l, i}$ and so $\trace(XY) = \sum_i \sum_l x_{i,l} y_{l,i}$. 
The $(j,j)$ entry of $YX$ is $\sum_t y_{j,t} x_{t,j}$ and so $\trace(YX) = \sum_j \sum_t y_{j,t} x_{t,j}$. Since $R$ is commutative, these are equal.

Say $B$ and $C$ are two [[Basis and Free Module|bases]] of $V$. Then $[g]_B^B = P [g]_{C}^{C} P^{-1}$ for some invertible matrix $P$ (namely, $P = [\id_V]_C^B$). 
Using the first part of the Lemma we have
$$\trace([g]_B^B) = \trace(P [g]_{C}^{C} P^{-1}) = \trace((P [g]_{C}^{C}) P^{-1}) = 
\trace(P^{-1} (P [g]_{C}^{C})) =
\trace((P^{-1} P) [g]_{C}^{C})) =
\trace([g]_{C}^{C}).$$
***

[^1]: See: [[Trace]]