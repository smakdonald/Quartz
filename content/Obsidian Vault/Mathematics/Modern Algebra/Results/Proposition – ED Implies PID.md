#### $\prop$ – ED Implies PID
If $R$ is a [[Euclidean Domain|Euclidean domain]], then $R$ is a [[Principal Ideal Domain|PID]].

###### *Proof.* 
Let $N$ be the norm function making $R$ into a Euclidean domain. Pick an ideal $I$. If $I$ is the zero ideal, $I = (0)$. Otherwise pick a non-zero element $b$ of $I$ with $N(b)$ as small as possible. (Such a $b$ exists by the well-ordering of $\Z_{\geq 0}$.) I claim $I = (b)$. It
is clear that $(b) \subseteq I$. Pick $a \in I$. Then
$$
a = bq + r
$$
and either $r = 0$ or $N(r) < N(b)$. But note that $r = a - bq \in I$, and we cannot have both  $r \ne 0$ and $N(r) < N(b)$ by our choice of $b$. So it must be that $r = 0$, and hence  $a\in (b)$.
***