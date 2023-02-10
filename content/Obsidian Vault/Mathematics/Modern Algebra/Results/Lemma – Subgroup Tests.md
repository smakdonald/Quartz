#### $\lem$ – Subgroup Tests
1. (Two-Step Test) If a subset $H$ of a [[Group|group]] $G$ is nonempty and closed under multiplication[^1] and inversion[^2], then $H$ is a [[Subgroup|subgroup]].
2. (One-Step Test) If a subset $H$ of a group $G$ is nonempty and satisfies for all $x,y \in H$, $xy^{-1} \in H$, then $H$ is a subgroup.

###### *Proof.* 

2. We prove the one-step test first.
	Assume $H$ is non-empty and for all $x,y \in H$, $xy^{-1} \in H$. Since $H$ is non-empty, there is an $h \in H$ and hence $e_G = hh^{-1} \in H$. Since $e_Gx=x=xe_G$ for any $x\in H$, $e_G$ is an identity element for $H$. For any $h \in H$, $h^{-1} = eh^{-1}  \in H$, and so every element of $H$ has an inverse inside $H$. For $x,y  \in H$ we have $y^{-1} \in H$ and thus $xy = x(y^{-1})^{-1} \in H$ and hence $H$ is closed under $\cdot$. This means that the restriction of the group [[Binary Operation|operation]] of $G$ to $H$ is a well-defined group operation. This operation is associative by the [[Group|axioms]] for the group $G$. The axioms of a group have now been established for $(H, \cdot)$.

1. We prove the two-step test.

	Assume $H$ is non-empty and closed under multiplication and inversion. Then, for $x,y\in H$ we have $y^{-1}\in H$ and $xy^{-1}\in H$. Since the hypothesis of the one-step test is satisfied, $H$ is a subgroup of $G$.
***

[^1]: If $g,h\in H$, then $gh\in H$.
[^2]: If $g\in H$, then $g\inv\in H$.
