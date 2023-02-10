#### $\thm$ – Artin-Tate Lemma
Let $A\subseteq B \subseteq C$ be rings. Assume that
- $A$ is [[Noetherian Ring|noetherian]],
- $C$ is [[Module Finite|module-finite]] over $B$, and
- $C$ is [[Algebra Finite|algebra-finite]] over $A$.
Then, $B$ is algebra-finite over $A$.

##### *Proof.*
Let $C=A[f_1,\dots,f_r]$ and $C=B g_1 + \cdots + B g_s$. Then, 
$$f_i = \sum_j b_{ij} g_j \quad \text{and} \quad g_i g_j = \sum_k b_{ijk} g_k$$
for some $b_{ij}, b_{ijk}\in B$. Let $B_0 = A[\{b_{ij}, b_{ijk}\}] \subseteq B$. This is a finitely generated $A$-algebra; by \Cref{fg algebras over noeth rings and noeth}, since $A$ is noetherian, so is $B_0$.

We claim that $C=B_0 \, g_1 + \cdots + B_0 g_s$. Given an element $c\in C$, write $c$ as a polynomial expression in $f_1, \ldots, f_r$. Since the $f_i$ are linear combinations of the $g_i$ with coefficients in the $b_{ij}$, we have $c\in A[\{b_{ij}\}][g_1,\dots,g_s]$. Then using the equations for $g_i g_j$ repeatedly, we can rewrite $c$ as a linear combination of the $g_i$ with coefficients in $B_0$.

Since $B_0$ is noetherian and $C$ is a finitely generated $B_0$-module, $C$ is a noetherian $B_0$-module, by \Cref{noetherian fg}. Since $B\subseteq C$, then $B$ is also a finitely generated $B_0$-module. In particular, $B_0 \subseteq B$ is algebra-finite. Since $A \subseteq B_0$ is algebra-finite, we conclude that $A  \subseteq B$ is algebra-finite, as required.