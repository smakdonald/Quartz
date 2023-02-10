#### $\defn{Definition}$ – Solvable by Radicals
Suppose $f(x) \in F[x]$[^1] where $F$ is a [[Field|field]] of [[Mathematics/Modern Algebra/Definitions/Ring Characteristic|characteristic]] $0$. We say that $f(x)$ is *solvable by radicals* over $F$ if there exists a finite chain of field [[Field Extension|extensions]] $$F = F_0 \subseteq F_1\subseteq F_2 \subseteq\cdots \subseteq F_m
$$ for some $m \geq 0$, such that 
1. $f(x)$ splits completely in $F_m$ (in other words, $F_m$ contains a [[Splitting Field|splitting field]] of $f(x)$) and 
2. for each $i$ such that $1 \leq i \leq m$ the field extension $F_{i-1} \subseteq F_{i}$ is the splitting field of a polynomial of the form $x^{n_i} - a_i$ for some positive integer $n_i$ and some element $a_i \in F_{i-1}$.
***

[^1]: See: [[Polynomial Ring]]