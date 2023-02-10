#### $\lem$ – Equivalencies of Cosets
Let $H \leq G$[^1]. The following facts about left [[Coset|cosets]] are equivalent for $x,y \in G$:
1. $x$ and $y$ belong to the same left coset of $H$ in $G$, 
2. $x = yh$ for some $h \in H$,
3. $y = xh$ for some $h \in H$,
4. $y^{-1}x \in H$,
5. $x^{-1}y \in H$,
6. $xH = yH$.

###### *Proof.* 
$(1. \Rightarrow 2)$: if $x$ and $y$ belong to the same left coset $gH$ of $H$ in $G$ then $x=gh'$ and $y=gh''$ for some $h',h''\in H$, so  $g=y(h'')^{-1}$ and therefore $x=y(h'')^{-1}h'=yh$ where $h=(h'')^{-1}h'\in H$.

$(2 \iff 3)$: $x=yh$ for some $h \in H$ $\iff$ $y = xh^{-1}$ and $h^{-1} \in H$.

$(2 \iff 4)$: $x=yh$ for some $h \in H$ $\iff$ $y^{-1} x=h\in H$.

$(4 \iff 5)$: $y^{-1} x\in H \iff (y^{-1} x)^{-1}\in H \iff x^{-1}y\in H$.

$(2 \Rightarrow 6)$: Suppose $x = yh$ for some $h \in H$, then by $2. \Rightarrow 3.$ we also have $y = xh''$ for some $h'' \in H$. Then we have
$$xH=\{xh'\mid h'\in H\}=\{yhh'\mid h'\in H\}\subset yH \text{ and}$$
$$yH=\{yh'\mid h'\in H\}=\{xh''h'\mid h'\in H\}\subset xH,$$
thus $xH=yH$.

$(6 \Rightarrow 1)$: Since $e_G=e_H\in H$, we have $x=xe_G\in xH$ and $y=ye_G\in yH$. If $xH=yH$ then, $x$ and $y$ belong to the same left coset.
***

[^1]: See: [[Subgroup]]