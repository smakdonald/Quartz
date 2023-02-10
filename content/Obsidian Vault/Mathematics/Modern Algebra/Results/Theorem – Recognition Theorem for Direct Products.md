#### $\thm$ – Recognition Theorem for Direct Products
Suppose $G$ is a [[Group|group]] with [[Normal Subgroup|normal]] [[Subgroup|subgroups]] $H\norm G$ and $K\norm G$  such that $H\cap K=\{e\}$ Then $HK\cong H\times K$[^1] via the [[Isomorphism|isomorphism]] of groups $\theta: H \times K \to HK$ defined by $\theta(h,k) = hk$. Moreover $H\cong \theta^{-1}(H)=\{(h,e)\mid h\in H\}\leq H\times K$ and $$K\cong \theta^{-1}(K)=\{(e,k)\mid k\in K\}\leq H\times K.$$

###### *Proof.* 
Notice that the hypothesis implies $HK\leq G$. Furthermore $H\norm G, K\norm G$ and $H\cap K=\{e\}$ imply that the elements of $H$ commute with the elements of $K$. Indeed, consider $h\in H,k\in K$. Then 
since $H\norm G$, $khk^{-1} \in H$, so also $[k,h]=khk^{-1}h^{-1}\in H$. Similarly it follows that $[k,h]\in K$, but since $H \cap K = \{e\}$ it follows that $[k,h]= e$, i.e. $hk = kh$ for any $h\in H, k\in K$.

Using the above we have
$$
\begin{aligned}
\theta((h_1, k_1) (h_2, k_2))  & = 
\theta(h_1h_2, k_1k_2) \\
& = h_1h_2k_1k_2\\
& = h_1k_1h_2k_2 = \theta(h_1, k_1) \theta(h_2, k_2)
\end{aligned}
$$
and thus $\theta$ is a homomorphism. It's kernel is  $\{(k,h) \mid k = h^{-1} \}$, which is just $\{e\}$ since $H \cap K = \{e\}$. The image of $\theta$ is clearly $HK$. This proves $\theta$ is an isomorphism. 
***

[^1]: See: [[HK]], [[Direct Product, Sum]]