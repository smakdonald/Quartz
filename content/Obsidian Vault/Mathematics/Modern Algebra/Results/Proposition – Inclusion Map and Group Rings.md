#### $\prop$ – Inclusion Map and Group Rings
For any [[Commutative Ring|commutative]] [[Ring|ring]] $R$, the inclusion $i:G \into R[G]$[^1] given by $i(g)= 1_Rg$ lands in $R[G]^\times$[^2] and induces a [[Homomorphism|homomorphism]] of [[Abelian Group|abelian]] [[Group|groups]] $G \to R[G]^{\times}$.

###### *Proof.* 
Note that $(1_R g)(1_R h) = 1_R (gh)$ by definition of multiplication in $R[G]$. 

This gives that for any $g\in G$ we have $$(1_R g)(1_R g^{-1}) =(1_R g^{-1})(1_R g) =1_R e_G=1_{R[G]},$$thus $i(g)$ is a unit in $R[G]$ with inverse $i(g^{-1})$. This shows that $\im(i)\subseteq R[G]^\times$.
The formula $(1_R g)(1_R h) = 1_R (gh)$ also gives that the map $g\mapsto 1_Rg$ is group homomorphism.
***

[^1]: See: [[Group Ring]]
[^2]: See: [[Group of Units]]