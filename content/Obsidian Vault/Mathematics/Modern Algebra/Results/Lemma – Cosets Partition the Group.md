#### $\lem$ – Cosets Partition the Group
For $H \leq G$[^1], the collection of left [[Coset|cosets]] of $H$ in $G$ form a partition of $G$, and similarly for the collection of right cosets. That is, 
- for all $x,y \in G$, either $xH = yH$ or $xH \cap yH = \emptyset$
- $\bigcup_{x\in G} xH=G$, and similarly for right cosets.
Moreover all left and right cosets have the same cardinality: $|xH| = |Hx|=|H|$ for any $x\in G$.

###### *Proof.* 
Every element $g$ of $G$ belongs to at least one left coset, since $g \in gH$ (since $e \in H$). If $xH$ and $yH$ share an element, then it follows from $1.\Rightarrow 6.$ of this [[Lemma – Equivalencies of Cosets|lemma]] that $xH=yH$. This proves that the left cosets partition $G$. To see that all left cosets have the same cardinality as $H$, define a function$$\rho: H \to gH$$by $\rho(h) = gh$. Let $gh\in gH$. Then $\rho(h)=gh$ so $\rho$ is onto. If $\rho(h) = \rho(h')$ then $hg = h'g$ and hence $h = h'$, so that $\rho$ is also one-to-one.
***
[^1]: See: [[Subgroup]]