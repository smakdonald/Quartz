#### $\lem$ – Elements of $\langle X \rangle$
For a subset $X$ of a [[Group|group]] $G$, the elements of $\langle X \rangle$[^1] can be described as:
$$\langle X \rangle = \left\{x_1^{j_1} \cdots x_m^{j_m} \mid m \geq 0, j_1, \dots, j_m \in \Z \text{ and }x_1, \dots, x_m \in X \right\}.$$

###### *Proof.* 
Let $S= \left\{x_1^{j_1} \cdots x_m^{j_m} \mid m \geq 0, j_1, \dots, j_m \in \Z \text{ and }x_1, \dots, x_m \in X \right\}$. Since $\langle X \rangle$ is a [[Subgroup|subgroup]] that contains $X$, it is closed under products and inverses, and thus must contain all elements of $S$.

For the opposite containment, we need to show the set $S$ really is a subgroup. We use the [[Lemma – Subgroup Tests|one step test]]:

- $S \ne \emptyset$ since we allow $m = 0$ and declare the empty product to be $e_G$. 
- If  $x_1^{j_1} \cdots x_m^{j_m}$ and $y_1^{i_1} \cdots y_n^{i_m}$ are in $S$ then $$
x_1^{j_1} \cdots x_m^{j_m}(y_1^{i_1} \cdots y_n^{i_m})^{-1}=
x_1^{j_1} \cdots x_m^{j_m} y_n^{-i_m} \cdots y_1^{-i_1}
$$is also in $S$.

Therefore $S\leq G$[^2] and $X\subseteq S$ (by taking $m=1$ and $j_1=1$) and by the minimality of $\langle X \rangle$[^3] we obtain $\langle X \rangle\subseteq S$. 
***

[^1]: Notation: $\langle X \rangle$ denotes the [[Subgroup|subgroup]] of $G$ [[Generator|generated]] by $X$.
[^2]: Notation: $S\leq G$ means that $S$ is a subgroup of $G$.
[^3]: By the definition of generated subgroups, $\langle X \rangle$ is the intersection of all subgroups of $G$ containing $G$. 