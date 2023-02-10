#### $\prop$ – Affine Varieties are Compact
Every [[Affine Variety|affine variety]] $X$ is compact for the [[Zariski Topology|Zariski topology]] – that is, every open cover of $X$ by Zariski open subsets admits a finite subcover or, equivalently, if $\{C_\a\}$ is a collection of closed subsets of $X$ such that $\bigcap_\a C_\a = \emptyset$ then $C_{\a_1} \cap \cdots \cap C_{\a_m}  = \emptyset$ for some finite list $\a_1, \dots, \a_m$ of indices.

In fact, every open subset of $X$ is compact.

##### *Proof.*
We may translate[^1] the first assertion into a statement about ideals in the ring $R = A(X)$[^2]: We need to prove that if $\{I_\a\}$ is a collection of ideals such that $\sum_{\a} I_\a = R$ then $$I_{\a_1} + \cdots + I_{\a_m} = R$$for some finite sub-collection. This holds since $\sum_{\a} I_\a = R$ iff $1 \in \sum_{\a} I_\a$ iff $1 \in I_{\a_1} + \cdots + I_{\a_m}$ for some $\a_1, \dots, \a_m$.

I'll just sketch the proof of the second assertion: Let  $U$ be an open subset of an affine variety $X$, say $U = X\setminus V(J)$ for an ideal $J$. We have $J = \igen{g_1, \dots, g_m}$ ([[Theorem – Hilbert’s Basis Theorem|Hilbert Basis Theorem]]), and so   $U = \bigcup_{i=1}^m X \setminus V(g_i)$. Since this is a finite union, it suffices to show each $X \setminus V(g_i)$ is quasi-compact. So, without loss, we may assume $U = X \setminus V(g)$ for some $g$. The points of $U$ are in bijective correspondence with the maximal ideals of the ring $A(X)[1/g]$ and the closed subsets are given by ideals of this ring. So the same proof as in the first part applies.

[^1]: This comes from the [[Corollary – Relative Nullstellensatz|Relative Nullstellensatz]].
[^2]: Notation: [[Coordinate Ring]]