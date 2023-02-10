#### $\thm$ – Solvability and Galois
Let $F$ be a [[Field|field]] of [[Mathematics/Modern Algebra/Definitions/Ring Characteristic|characteristic]] $0$, $f(x) \in F[x]$[^1], and let $K$ be the [[Splitting Field|splitting field]] of $f(x)$. Then $f(x)$ is [[Solvable by Radicals|solvable by radicals]] if and only if $\Gal(K/F)$[^2] is a [[Solvable Group|solvable]] [[Group|group]].

##### *Proof.*
$(\Rightarrow)$ Say $K \subseteq F_n$ with $F = F_0 \subseteq F_1 \subseteq \cdots \subseteq  F_n$ such that $F_i$ is the splitting field of $x^{m_i} - a_i$ over $F_{i-1}$ with $a_i \in F_{i-1}$ Form a new chain $$F = F_0 \subseteq F_0' \subseteq F'_1 \subseteq \cdots \subseteq  F'_n$$by letting $F_0'$ be the splitting field of $x^M - 1$ with $M = m_1 \cdots m_n$. and letting $F_1'$ be the splitting field over $F_0'$ of $x^{m_1} - a_1$ etc. So $K \subseteq F_n \subseteq F'_n$ To simplify notation, let's just assume $F_0 \subseteq F_1$ is the splitting field of $x^M - 1$ and that $m_i \mid M$ for all $i \geq 2$. Thus $F_i'$ contains all $m_i$-th roots of unity for all $i \geq 2$. 

Since $F \subseteq K$ is Galois, part of the Fundamental Theorem gives that $\Gal(K/F)$ is a quotient of $\Gal(F_n/F)$ (by the normal subgroup $\Gal(F_n/K)$.) It is well-known (and not that hard to prove just from the definition) that any quotient of a solvable groups is solvable. So, it suffices to show $\Gal(F_n/K)$ is solvable. Inspecting the definition we see that it suffices to prove $\Gal(L/E)$ is abelian whenever $L$ is the splitting field over $E$ of a polynomial of the form $x^M -1$ or when $L$ is the splitting field over $E$ of a polynomial of the form $x^m - a$ with $a \in E$ under the assumption that $E$ contains all $m$-th roots of unity. These facts are given by the two propositions just proven.
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Galois Extension|Galois Group]]