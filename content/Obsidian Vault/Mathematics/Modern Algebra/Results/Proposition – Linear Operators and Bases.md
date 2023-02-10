#### $\prop$ – Linear Operators and Bases
Let $R$ be a non-zero [[Commutative Ring|commutative]] [[Ring|ring]]. Given a [[Linear Operator|linear operator]] $g: V \to V$ on a [[Basis and Free Module|free]] $R$-[[Module|module]] $V$ of finite [[Dim (Vector Space)|rank]] $n$, we have:
1. The matrices [[Homomorphism Matrix|representing]] $g$ with respect to any two choices of [[Basis and Free Module|bases]] of $V$ are [[Similar Matrices|similar]]
2. If $X$ represents $g$ with respect to a basis $B$ of $V$ and if $Y$ is similar to $X$, then there is a basis $C$ of $V$ such that the matrix representing $g$ with respect to $C$ is $Y$.
3. 
###### *Proof.* 
We proved the first assertion above.

Say $X = [g]_B^B$ and $Y = PXP^{-1}$ for some invertible matrix $P$. By Proposition \ref{prop210} above, $P = [\id_V]_B^C$ for a (unique) new basis $C$. So $Y = [\id]^C_{B} [g]_B^B [\id_V]_C^{B} = [g]_{C}^C$. 
***