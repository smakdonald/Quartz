#### $\thm$ – Existence of SOPs
Let $(R,\m)$ be a [[Noetherian Ring|noetherian]] [[Local Ring|local ring]] of [[Krull Dimension of a Ring|dimension]] $d$. There there exist $x_1,\dots,x_d\in \m$ such that $\m = \sqrt{(x_1,\dots,x_d)}$[^1].

##### *Proof.*
Let $d :=  \dim(R)$. If $d=0$, then $\m=\sqrt{(0)}$, so the statement holds.

In general, we will show that we can choose $x_1,\dots, x_i\in \m$ inductively such that every minimal prime of $J_i= (x_1,\dots,x_i)$ has height $i$. The case $i=0$ is clear from the comment above. Say that we have chosen the first $i$ elements. If $i<d$, note that $\m$ is not a minimal prime of $J_i$, as this would contradict \hyperref[Krull height theorem]{Krull's height theorem}. Note that $R$ is noetherian and thus $J_i$ has finitely many minimal primes, by \Cref{min primes finite}. Thus, by \hyperref[prime avoidance]{Prime Avoidance}, we can choose $x_{i+1} \in \m$ not in any minimal prime of $J_i$. Then by \hyperref[Krull height theorem]{Krull's height theorem} every minimal prime of $J_{i+1} :=  J_i +(x_{i+1})$ has height at most $i+1$. On the other hand, every $Q \in \Min(J_{i+1})$ contains some $P \in \Min(J_i)$, and in fact we must have $Q \supsetneq P$, since $x_{i+1}\in Q \smallsetminus P$. Since $P$ has height $i$ and $P \supsetneq Q$, then $Q$ must have height at least $i+1$. Therefore, $Q$ must have height exactly $i+1$, completing the induction.

Since every minimal prime of $J_d = (x_1,\dots,x_d)$ has height $d$, its unique minimal prime must be $\m$. It follows that $\sqrt{J_d}=\m$.

[^1]: Notation: [[Radical Ideal]]