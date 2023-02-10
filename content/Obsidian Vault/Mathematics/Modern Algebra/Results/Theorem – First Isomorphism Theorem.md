#### $\thm$ – First Isomorphism Theorem
If $f: G \to H$ is a [[Homomorphism|homomorphism]] of [[Group|groups]], then $\ker(g)\norm G$[^1] and the map $\ov{f}$ defined by the [[Theorem – UMP of a Quotient Group|UMP]]  induces an [[Isomorphism|isomorphism]]$$\ov{f}: G/\ker(f) \xra{\cong} \im(f).$$
###### *Proof.* 
By the UMP, there exists a homomorphism $\ov{f}$ such that $\ov{f} \circ \can = f$, and its kernel consists of just the one element $\ker(f)/\ker(f)$ of $G/\ker(f)$. So $\ov{f}$ is one-to-one, and the image of $\ov{f}$ is #clearly the same as the image of $f$.  
***

[^1]: For $(\ker)$, See: [[Kernel]]. For $(\nsg)$, See: [[Normal Subgroup]]

#### $\thm$ – First Isomorphism Theorem for Rings
If $f: R \to S$ is a [[Ring|ring]] [[Homomorphism|homomorphism]], then $R/\ker(f)\cong \im(f)$ via the map $\overline{f}$ given by $\ov{f}(r + \ker(f)) = f(r)$.

###### *Proof.* 
The map $\overline{f}$ is a well-defined ring homomorphism by the UMP for quotient rings. By the First Isomorphism Theorem for groups, the map $\ov{f}$ is bijective, finishing the proof.
***