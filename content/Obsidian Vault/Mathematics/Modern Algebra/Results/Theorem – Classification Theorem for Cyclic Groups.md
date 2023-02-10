#### $\thm$ – Classification Theorem for Cyclic Groups
Every infinite [[Cyclic|cyclic]] [[Group|group]] is [[Isomorphism|isomorphic]] to $C_\infty$. Every cyclic group of [[Order|order]] $n$ is isomorphic to $C_n$.

###### *Proof.* 
Suppose $G = \langle x \rangle$ with $|x| = n$ or $|x| = \infty$ and set $H=C_n$ in the first case and $H=C_\infty$ in the second case. Then by the [[Proposition – Universal Mapping Property of a Cyclic Group|UMP]] for cyclic groups there exist homomorphisms $f: G \to H$ and $g: G \to H$ such that $f(x) = a$ and $g(a) =x$. So $g \circ f$ is an endomorphism of $G$ mapping $x$ to $x$. But the identity map also has this property, and so the uniqueness clause gives $g \circ f = \id_G$. Similarly, $f \circ g = \id_H$. 
***