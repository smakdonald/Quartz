#### $\prop$ – Compatibility and Normality
Let $G$ be a [[Group|group]]. An equivalence relation $\sim$ on $G$ is [[Compatible with Addition & Multiplication|compatible with multiplication]] if and only if $\sim \,=  \,\sim_N$ for some [[Normal Subgroup|normal]] [[Subgroup|subgroup]] $N \norm G$.

###### *Proof.* 
$(\Leftarrow)$ If $\sim$ is compatible with multiplication then setting $N := \{g \in G | g \sim e\}$ gives $N\norm G$ and $\sim=\sim_N$.

To see that $N\leq G$ we use the [[Lemma – Subgroup Tests|2-step test]]. Let $x,y\in N$. Then $y\sim e$ implies $e=yy^{-1}\sim ey^{-1}=y^{-1}$ so $y^{-1}\in N$. Moreover $x\sim e$ implies $xy\sim ey=y\sim e$ so $xy\sim e$ says $xy\in N$.

To see that $N\norm G$, let $n\in N$ and $g\in G$. Since $n\in N$, $n\sim e$, thus $gng^{-1}\sim geg^{-1}\sim e$, which shows that $gng^{-1}\in N$. We have shown that $gNg^{-1} \subseteq N$ for any $g\in G$. To show the opposite containment, notice that for $n\in N$ we can write $n=g(g^{-1}ng)g^{-1}=gn'g^{-1}$ for $n'=g^{-1}ng\in N$.

To see that $\sim=\sim_N$ note that $x\sim y \iff xy^{-1}\sim e \iff xy^{-1}=n$ for some $n\in N$ $\iff x=ny\iff x\sim_N y$. 

$(\Rightarrow)$ If $\sim \,=  \,\sim_N$ then $\sim$ is compatible with multiplication. Let $x,y,z\in G$ such that $x\sim_N y$. Then $y=nx$ for some $n\in N$, so $yz=nxz$ and $$zy=znx=zn(z^{-1}z)x=(znz^{-1})zx=n'zx$$for some $n'\in N$, where the last equality uses the normal subgroup property. We deduce that $yz\sim_N xz$ and $zy\sim_N zx$.
***