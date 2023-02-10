#### $\thm$ – LOIS
Let $G$ be a [[Group|group]] that [[Group Action|acts]] on a finite set $S$ via $\cdot$. For any $s \in S$ we have[^1] $$|\Orb_G(s)| = [G: \Stab_G(s)]$$
###### *Proof.* 
Let $\cL$ be the collection of left [[Coset|cosets]] of $\Stab_G(s)$ in $G$. Define a function $$\a: \cL \to \Orb_G(s)$$by $\a(x \Stab_G(s)) = x \cdot s$. This function is well defined and one-to-one: $$x \Stab_G(s) = y \Stab_G(s)\iff x^{-1}y \in \Stab_G(s) \iff x^{-1}y \cdot s = s \iff 
y \cdot s = x \cdot s.$$ The function $\alpha$ is onto by definition of $\Orb_G(s)$. Thus $\a$ is a bijection and it yields equalities 
$$[G: \Stab_G(s)]=|\cL|=|\Orb_G(s)|.$$

***

[^1]: See: [[Order]], [[Orbit]], [[Index]],