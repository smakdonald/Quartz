#### $\prop$ – Examples of Subgroups
1. $\{e_G\}$ and $G$ are the trivial [[Subgroup|subgroups]] of $G$.
2. If $H$ is a subgroup of $G$ and $K$ is a subgroup of $H$, then $K$ is a subgroup of $G$.
3. If $H_\alpha$ is a subgroup of $G$ for all $\alpha$ in an index set $J$, then $H=\bigcap_{\alpha\in J} H_\alpha$ is a subgroup of $G$.
4. If $f: G \to H$ is a [[Homomorphism|homomorphism]] of groups, then the set-theoretic image of $f$, $$\im(f) := \{f(g) \mid g \in G\}$$ is a subgroup of $H$.
5. If $f: G \to H$ is a homomorphism of groups, then the [[Kernel|kernel]] of $f$, $$\ker(f) := \{g\in G \mid f(g)=e_H\},$$ is a subgroup of $G$.

###### *Proof.*[^1] 
1. Exercise. #fix 

2.  $H$ is not empty since $e_G \in H_\alpha$ for all $\alpha\in J$. If $x,y\in G$, then for each $\alpha$, $x,y \in H_\alpha$ and hence $xy^{-1} \in H_\alpha$. It follows that $xy^{-1} \in H$. 

3. To see this, note that $\im(f) \ne \emptyset$ since $G$ is non-empty. If $x,y \in \im(f)$, then $x = f(a)$ and $y = f(b)$ for some $a,b \in G$ and hence $$xy^{-1} =f(a)f(b)^{-1} = f(ab^{-1}) \in \im(f).$$
4. To see this, using the one-step subgroup test note that if $f(x)=f(y)=e_G$ then $f(xy^{-1})=f(x)f(y)^{-1}=e_G$. So, if $x,y\in \ker(f)$ then $xy^{-1}\in \ker(f)$.

5. The center $Z(G)$ is the kernel of the [[Proposition – Permutation Representation|permutation representation]] $G\to \Perm(G)$ for the conjugation [[Group Action|action]], so by part 4. $Z(G)$ is a subgroup of $G$. 
***

[^1]: For all the following proofs, we will be appealing to the [[Lemma – Subgroup Tests|Subgroup Test]]. So if we can show $xy\inv$ is contained within our subsets for any $x,y\in G$, we will have proved that our subsets are indeed subgroups.