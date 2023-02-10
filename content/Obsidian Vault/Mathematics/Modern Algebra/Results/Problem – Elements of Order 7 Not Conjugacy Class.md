### Problem 1 – Elements of Order 7 Not Conjugacy Class
Let $G = A_7$[^1] and $S$ be the set of elements of $G$ of [[Order|order]] $7$. Prove that $S$ is not a [[Conjugacy Class|conjugacy class]] of $G$.

###### *Proof*.
Elements of order $7$ in $G$ must permute all $7$ elements, making them of the form $(abcdefg)$. There are $6!$ such permutations, given that we can always reorder them so that $a$ is first, leaving $6$ remaining spots without replacement. Let $S$ denote the set of these $6!$ elements.

Suppose by way of contradiction there existed some $s\in G$ such that $S=C_s(G)$. Let $G$ act on itself through conjugation, making $S=C_s(G)=\Orb(s)$ by the definition of [[Conjugacy Class|conjugacy class]]. The [[Corollary – Orbit-Stabilizer Theorem|Orbit-Stabilizer Theorem]] tells us that $|G|=|\Orb(s)|\cdot|\Stab(s)|$, meaning that the order of $S$ must divide the order of $G$. However, $|G|=\frac{7!}{2}$ and $|S|=6!$, so this is a contradiction. Thus $S$ is not a conjugacy class of $G$.

#qual

[^1]: Notation: [[Alternating Group]]