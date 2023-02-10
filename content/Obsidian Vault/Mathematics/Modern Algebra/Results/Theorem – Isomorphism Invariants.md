#### $\thm$ – Isomorphism Invariants
The following are [[Isomorphism|isomorphism]] [[Isomorphism Invariant|invariants]]:
1. the [[Order|order]] of the [[Group|group]],
2. the set of orders of elements in the group,
3. being [[Abelian Group|abelian]],
4. the order of the center of the group, and
5. being [[Generator|finitely generated]].

###### *Proof.* 
Let $G$ and $H$ be isomorphic groups with $f:G\to H$ a group isomorphism.

1. Since $f$ is a bijection by this [[Proposition – Isomorphism iff Bijective Homomorphism|proposition]], and two sets have the same cardinality if and only if they are in bijective correspondence to each other, we obtain that $|G|=|H|$.
2. We wish to show $\{|x| \ | \ x\in G\}= \{|y| \ | \ y\in H\}$. 
	$\subseteq$ follows by problem 2(c) of homework 1, since  $x\in G$ yields $f(x)\in H$ and $|f(x)|=|x|$. #fix
	$\supseteq$ also follows by problem 2(c) of homework 1, applied to the group isomorphism $f^{-1}$, since  $y\in G$ yields $f^{-1}(y)\in G$ and $|f^{-1}(y)|=|y|$. #fix
3. If $y_1,y_2\in H$ then there exist $x_1, x_2\in G$ such that $f(x_i)=y_i$. Then we have$$y_1y_2=f(x_1)f(x_2)=f(x_1x_2)\stackrel{*}{=}f(x_2x_1)=f(x_2)f(x_1)=y_2y_1,$$where $*$ indicates the usage of the abelian property for $G$. 
4. Exercise. The idea is to show $f$ induces an isomorphism $Z(G)\cong Z(H)$. #fix 
5. Exercise. Show that if  $S$ generates $G$ then $f(S)=\{f(s) \ | \ s\in S\}$ generates $H$. #fix
***