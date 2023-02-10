#### $\lem$ – Spec Strong Nullstellensatz
Let $R$ be a ring, $I$ an ideal, and $W$ a [[Multiplicatively Closed Set|multiplicatively closed]] subset. If $W \cap I = \varnothing$[^1], then there is a [[Prime Ideal|prime ideal]] $P$ with $P \supseteq I$ and $P \cap W= \varnothing$.

##### *Proof.*
Consider the family of ideals $\mathcal{F} :=  \{ J \ | \ J \supseteq I, J \cap W=\varnothing\}$ ordered with inclusion. This is nonempty, since it contains $I$, and any chain $J_1 \subseteq J_2 \subseteq \cdots$ has an upper bound $\cup_i J_i$. Therefore, $\mathcal{F}$ has some maximal element $\A$ by a basic application of Zorn's Lemma. We claim $\A$ is prime. Suppose $f,g\notin \A$. By maximality, $\A+(f)$ and $\A+(g)$ both have nonempty intersection with $W$, so there exist $r_1f+a_1$, $r_2 g+a_2 \in W$, with $a_1,a_2\in \A$. If $fg\in \A$, then$$\underset{\in W}{(r_1f+a_1)}\underset{\in W}{(r_2g+a_2)} = r_1 r_2 fg + r_1 f \underset{\in \mathbb{A}}{a_2} + r_2 g \underset{\in \mathbb{A}}{a_1} + \underset{\in \mathbb{A}}{a_1 a_2} \in W \cap \A,$$

[^1]: Notation: [[Contraction]]