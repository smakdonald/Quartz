#### $\thm$ – Rational Canonical Form
Given a [[Dim (Vector Space)|finite]] [[Dim (Vector Space)|dimensional]] $F$-[[Vector Space|vector space]] $V$ and an $F$-[[Linear Operator|linear operator]] $g: V \to V$, there is a [[Basis and Free Module|basis]] $B$ of $V$ such that the matrix [[Homomorphism Matrix|representing]] $g$ relative to $B$ is $$[g]_B^B = C(f_1) \oplus \cdots \oplus C(f_s)$$for monic polynomials $f_1, \dots, f_s$ of [[Polynomial Degree|degree]] at least one such that $f_1 | f_2 | \cdots | f_s$[^1]. Moreover, this matrix is unique, and is known as the *rational canonical form* of the operator $g$.  

###### *Proof.* 
We know by the Fundamental Theorem of modules over $F[x]$ (i.e., Corollary \ref{cor310}) that there is a $F[x]$-module isomorphism
$$
V_{g} \cong F[x]/(f_1)\oplus \cdots \oplus F[x]/(f_s)
$$
for some unique list of  monic, non-constant polynomials $f_1, \cdots, f_s$ with $f_i \mid f_{i+1}$ for all $i$. 
Recall that the operator $g$ on $V$ is given as $\lx$ (multiplication by $x$) on $V_g$. Since this is a $F[x]$-module isomorphism, $g$ corresponds to multiplication by $x$ on each summand $F[x]/(f_i)$.  As we have seen before, for each $i$, the matrix representing $\lx$ on $F[x]/f_i$ relative to the basis $B_i := \{1, x, x^2, \dots, x^{\deg(f_i)-1}\}$ of $F[x]/f_i$ is the companion matrix $C(f_i)$ of $f_i$. Let $B$ be the $F$-basis of $F[x]/(f_1)\oplus \cdots \oplus F[x]/(f_s)$ given by tuples $$B = \{(b_1, 0, \dots, 0) \mid b_1 \in B_1\} \cup \{(0, b_2, 0, \dots, 0) \mid b_2 \in B_{2\} \cup}\cdots \cup \{(0, 0, \dots, 0, b_s) \mid b_s \in B_s\}$$(in that order). Then the matrix of $\lx$ on $F[x]/(f_1)\oplus \cdots \oplus F[x]/(f_k)$ for $B$ is $C(f_1) \oplus \cdots \oplus C(f_s)$.

This gives existence. Uniqueness is a consequence of the uniqueness of the list $f_1, \dots, f_s$, but I will omit the details.
***

[^1]: See: [[GCD|Divisor]]