#### $\prop$ – Permutation Representation
Assume $(G, \cdot)$ is a [[Group|group]] and $S$ is a set. 
1. If $\cdot$ is an [[Group Action|action]] of $G$ on $S$, then the function $\rho: G \to \Perm(S)$[^1] defined as $\rho(g) = \sigma_g$, where $\sigma_g:S\to S$ is the function given by $\sigma_g(s)=g \cdot s$, is a well defined [[Homomorphism|homomorphism]] of groups. 
2. Conversely, if $\rho: G \to \Perm(S)$ is a group homomorphism,  the rule $g \cdot s := \rho(g)(s)$ defines an action of $G$ on $S$. 

###### *Proof.*
Assume we are given an action $\cdot$ of $G$ on $S$. We need to check that for all $g$, $\sigma_g$ really is a permutation of $S$. We'll show this by proving that $\sigma_g$ has a two-sided inverse and that inverse is $\sigma_{g^{-1}}$.

We have
$$\begin{align*}
(\sigma_g\circ\sigma_{g^{-1}})(s) &=\sigma_g(\sigma_{g^{-1}}(s)) & \text{ (def of composition)}\\
&=g\cdot (g^{-1} \cdot s) & \text{ (def for } \sigma_g \text{ and } \sigma_{g^{-1}})\\
&=(gg^{-1})\cdot s & \text{ (first property of a group action)}\\
&=e_G\cdot s & \text{ (group axiom)}\\
&= s &\text{ (second property of a group action)}
\end{align*}$$
thus $\sigma_g\circ\sigma_{g^{-1}}=\id_S$ and a similar argument shows that $\sigma_{g^{-1}}\circ\sigma_{g}=\id_S$

Finally, we wish to show $\rho(gg')=\rho(g) \circ \rho(g')$, equivalently $\sigma_{gg'}=\sigma_g\circ\sigma_{g'}$. Since
$$\sigma_{gg'}(s) = (gg')\cdot s = g\cdot(g'\cdots) =\sigma_g\left(\sigma_{g'}(s)\right) = (\sigma_g\circ\sigma_{g'})(s)$$
holds for all $s$, this proves $\rho$ is a homomorphism.

Given a homomorphism $\rho$, the function $G \times S \to S$ defined as $g \cdot s = \rho(g)(s)$ is an action because $$g'(gs) = \rho(g')(\rho(g)(s)) = (\rho(g') \circ\rho(g))(s) = \rho(gg')(s) = (gg')s,$$and $e_G s = \rho(e_G)(s) = \id(s) = s$. 
***

[^1]: Notation: $\Perm(S)$ is the [[Permutation Group]] on $S$