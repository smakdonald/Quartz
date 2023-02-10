#### $\prop$ – Recognition Theorem: Internal Semidirect Products
For a [[Group|group]] $G$, suppose we are given $H$ and $K$ so that
- $H \nsg G$[^1],
- $K \leq G$[^2], 
- $HK = G$[^3], and
- $H \cap K = \{e\}$.
Let $\rho: K \to \Aut(H)$[^4] be the [[Proposition – Permutation Representation|permutation representation]] of the [[Group Action|action]] of $K$ on $H$ via [[Automorphism|automorphisms]] given by conjugation in $G$. (This means that for any $k\in K$ $\rho(k)=c_k$, where $c_k\in \Aut(H)$ is the function $c_k(h)=khk^{-1}$ for all $h\in H$.) Then the function
$$\theta: H \sdp_\rho K \to G$$
defined by $\theta(y,x) = yx$ is an [[Isomorphism|isomorphism]] of groups. 
Moreover, under this isomorphism, $K$ corresponds to $K'$ and $H$ corresponds to $H'$ (referring to the notation in Theorem \ref{thm:sdp} above). #fix 

###### *Proof.* 
We have
$$
\begin{aligned}
\theta((y_1, x_1) (y_2, x_2))  & = 
\theta(y_1 c_{x_1}(y_2), x_1 x_2) \\
& = y_1x_1y_2x_1^{-1} x_1 x_2 \\
& = y_1x_1y_2x_2 = \theta(y_1, x_1) \theta(y_2, x_2)
\end{aligned}
$$
and thus $\theta$ is a homomorphism. It's kernel is  $\{(y,x) \mid y = x^{-1}, y\in H, x\in K \}$, which is just $\{e\}$ since $H \cap K = \{e\}$. 

The image of $\theta$ is clearly $KH = G$. This proves $\theta$ is an isomorphism. It is obvious that $\theta(K') = K$ and $\theta(H')= H$. 
***

[^1]: See: [[Normal Subgroup]]
[^2]: See: [[Subgroup]]
[^3]: See: [[HK]]
[^4]: See: [[Automorphism]]