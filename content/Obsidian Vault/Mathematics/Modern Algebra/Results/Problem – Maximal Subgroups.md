### Problem 1 – Maximal Subgroups
Let $G$ be a [[Group|group]]. A [[Subgroup|subgroup]] $H$ of $G$ is called *maximal* if $H\neq G$ (that is, $H$ is a proper subgroup of $G$) and whenever $K$ is another subgroup of $G$ containing $H$, either $K = H$ or $K = G$.  Show that every nontrivial finitely generated group $G$ possesses maximal subgroups.

##### *Proof.*
Let $G$ be a group.

Let $S$ be the poset of all proper subgroups of $G$ ordered in terms of inclusion. Consider a string of these. Consider the union of them all. Luckily, unions of subgroups are subgroups if and only if there is containment, which there is, since everything is in the union. Thus its a subgroup. Since union in $S$ and yields an upper bound, by Zorn's Lemma we a maximal element. Thus $G$ possesses maximal subgroups. 
***
#qual