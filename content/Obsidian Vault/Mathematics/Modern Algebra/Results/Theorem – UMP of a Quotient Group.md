#### $\thm$ – Universal Mapping Property of a Quotient Group
Let $G$ be a [[Group|group]] and $N$ a [[Normal Subgroup|normal]] [[Subgroup|subgroup]]. If $f: G \to H$ is a [[Homomorphism|homomorphism]] of groups such that $N \subseteq \ker(f)$[^1], then
1. there exists a unique group homomorphism $\overline{f}: G/N \to H$ such that the composition of $\overline{f}$ and the quotient map $\pi: G  \onto G/N$ is $f$. 
2. If $f$ is onto, then $\overline{f}$ is onto. 
3. Moreover, $\ker(\overline{f}) = \ker(f)/N = \{ g N \mid f(g) = e_H\}.$

###### *Proof.* 
1.  If such a $\ov{f}$ exists, it is necessarily unique since $G \onto G/N$ is onto. In fact, if $f=\pi\circ \ov f$ then $\ov{f}$  has to be given by the formula$$\ov{f}(gN) = f(g).$$We now need to show that this formula determines a well-defined homomorphism: If $xN = yN$, then $y^{-1}x \in N \subseteq \ker(f)$ and so $f(y)^{-1} f(x) = e$, whence $f(y) = f(x)$. For any $x,y$ we have$$\ov{f}(xNyN) = \ov{f}(xyN) = f(xy) = f(x)f(y) =\ov{f}(xN) \ov{f}(yN).$$
2. The formula for $\ov f$ given above ensures that $\im f=\im \ov f$ hence $f$ is surjective if and only if  $\ov f$ is surjective.

3. We have $\ov{f}(xN) = e_H$ iff $f(x) = e_H$ iff  $x \in \ker(f)$ iff $xN \in\ker(f)/N$. If $xN \in \ker(f)/N$ for some $x \in G$, then $xN = yN$ for some $y \in \ker(f)$ and hence $x = yz$ for some $z \in N$. Since $N \subseteq \ker(f)$, we have $x \in \ker(f)$.
***

[^1]: See: [[Kernel]]