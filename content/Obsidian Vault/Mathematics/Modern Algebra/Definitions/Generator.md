#### $\defn$ – Generator
A set $S$ is said to *generate* or be a *set of generators* for a [[Group|group]] if every element of the group can be expressed in some as a product of the elements of $S$ and their inverses (with repetitions allowed). 
***
#### $\defn$ – Finitely Generated (Group)
#### Finitely Generated
A [[Group|group]] $G$ is *finitely generated* provided that $G=\langle A \rangle$, where $A$ is a finite set.
***
#### $\defn$ – Finitely Generated (Module)
#### Finitely Generated Module
A module $M$ is *finitely generated* if there exists some finite subset $A$ of $M$ such that $M = R \cdot A$.
***
#### $\defn$ – Generated Subgroup
Given a [[Group|group]] $G$ and a subset $X$ of $G$, *the subgroup of $G$ generated by $X$* is $$\langle X \rangle := \bigcap_{H \leq G, H \supseteq X} H.$$
If $X=\{x\}$ is a set with one element then we write $\langle X \rangle=\langle x \rangle$ and we refer to this as the *cyclic subgroup generated by* $x$.
***
#### $\defn$ – Generated Normal Subgroup
Let $G$ be a [[Group|group]] and let $R \subseteq G$ be a set. The *normal subgroup* of $G$ [[Generator|generated]] by $R$, denoted $\langle R \rangle ^N$, is the set of all products of [[Conjugacy Class|conjugates]] of elements of $R$ and inverses of elements of $R$. In symbols,  $$\langle R \rangle ^N= \{ g_1r_1^{i_1}g_1^{-1} \dots g_mr_m^{i_m}g_m^{-1} \mid m \geq 0, r_j \in R, g_j \in G, i_j \in \{1,-1\}, \forall 1\leq j\leq m\}.$$
***
#### $\defn$ – Generated Ideal
If $A$ is any subset of a [[Ring|ring]] $R$, the *ideal generated by* $A$, denoted $(A)$, is the intersection of all [[Ideal|ideals]] of $R$ that contain $A$:  $$(A)=\bigcap_{I \text{ ideal of }R,  A\subseteq I} I.$$An ideal $I$ is *finitely generated* if $I = (A)$ for some finite subset $A$ of $R$.
***
#### $\defn$ – Generated Submodule
Let $M$ be an $R$-[[Module|module]] and $\Gamma \subseteq M$. The [[Submodule|submodule]] of $M$ *generated* by (also known as the submodule *spanned* by) $\Gamma$, denoted $\sum_{m \in \Gamma} R m$, is the smallest (with respect to containment) submodule of $M$ containing $\Gamma$. 

We say $\Gamma$ *generates* $M$, or is a *set of generators* for $M$, if $\sum_{m \in \Gamma} R m =~M$, meaning that every element in $M$ can be written as a finite [[Linear Combination|linear combination]] of elements in $\Gamma$. 

Another way this can be written is
$$R \cdot \Gamma = \{r_1m_1 + \dots + r_n m_n \mid n \geq 0, r_1,\dots,r_n \in R, a_1, \dots, m_n \in \Gamma\}.$$