#### $\thm$ – Zerodivisors Associated Primes
If $R$ is [[Noetherian Ring|noetherian]], and $M$ is an arbitrary $R$-module, then $$\bigcup\limits_{P \in \Ass(M)} P = \mathcal{Z}(M).$$[^1]
##### *Proof.*
If $r \in \mathcal{Z}(M)$, then by definition we have $r \in \ann(m)$ for some nonzero $m \in M$. Since $\ann(m)$ is contained in some associated prime of $M$, by \Cref{every ann contained in ass prime}, then $r$ is also contained in some associated prime of $M$. On the other hand, if $P$ is an associated prime of $M$, then by definition all elements in $P$ are zerodivisors on $M$.

For the graded case, replace the set of zerodivisors with the annihilators of homogeneous elements. Such annihilator is homogeneous, since if $m$ is homogeneous, and $fm=0$, writing $f=f_{a_1}+\dots+f_{a_b}$ as a sum of homogeneous elements of different degrees $a_i$, then $0=fm=f_{a_1}m+\dots+f_{a_b}m$ is a sum of homogeneous elements of different degrees, so $f_{a_i}m=0$ for each $i$.

[^1]: Notation: [[Associated Prime]], [[Module Zerodivisor]]