#### $\lem$ – Every Ann Contained in Ass Prime
If $R$ is [[Noetherian Ring|noetherian]], and $M$ is an arbitrary $R$-module, then for any nonzero $m \in M$, $\ann_R(m)$[^1] is contained in an [[Associated Prime|associated prime]] of $M$. If $R$ and $M$ are [[Graded Ring|graded]] and $m$ is a [[Homogeneous Element|homogeneous]] element, then $\ann_R(m)$ is contained in a [[Homogeneous Ideal|homogeneous]] [[Prime Ideal|prime]].

##### *Proof.*
The set of ideals $S :=  \{ \ann_R(m) \ | \ m\in M, m \neq0\}$ is nonempty, and any element in $S$ is contained in a maximal element, by noetherianity. Note in fact that any element in $S$ must be contained in a maximal element of $S$. Let $I=\ann(m)$ be any maximal element, and let $rs\in I$, $s\notin I$. We always have $\ann(sm)\supseteq \ann(m)$, and equality holds by the maximality of $\ann(m)$ in $S$. Then $r(sm)=(rs)m=0$, so $r\in \ann(sm)=\ann(m)=I$. We conclude that $I$ is prime, and therefore it is an associated prime of $M$.

The same argument above works if we take $\{ \ann_R(m) \ | \ m\in M, m \neq 0 \ \text{homogeneous} \}$, using \Cref{graded primes}.

[^1]: Notation: [[Annihilator]]