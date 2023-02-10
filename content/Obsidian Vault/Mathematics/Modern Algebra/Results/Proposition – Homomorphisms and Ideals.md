#### $\prop$ – Homomorphisms and Ideals
If $f: R \to S$ is a [[Ring|ring]] [[Homomorphism|homomorphism]], then
1. the image of $f$ is a [[Subring|subring]] of $S$ and
2. the [[Kernel|kernel]] of $f$ is an [[Ideal|ideal]] of $R$.
3. $f$ is injective if and only if $\ker(f)=\{0\}$.
4. if $I$ is an ideal of $R$ then $f(I)$ is an ideal of $f(R)$.
5. if $J$ is an ideal of $S$ then $f^{-1}(J)$ is an ideal of $R$.

###### *Proof.* 
(2) Since $f$ is a ring homomorphism, it is in particular a group homomorphism $(R,+)\to (S,+)$. We know the kernel of a group homomorphism is a subgroup, so $\ker(f)\leq (S,+)$. All that remains to be shown is that for any $r\in R$ $r\ker(f)\subseteq \ker(f)$ and $\ker(f)r\subseteq \ker(f)$. Let $x\in \ker(f)$; then $f(x)=0$ and $f(rx)=f(r)f(x)=0$,  $f(xr)=f(x)f(r)=0$ show $rx,xr\in \ker(f)$.
***