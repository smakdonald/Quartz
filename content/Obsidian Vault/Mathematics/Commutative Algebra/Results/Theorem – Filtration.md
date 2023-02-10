#### $\thm$ – Filtration
Let $R$ be a [[Noetherian Ring|noetherian ring]], and $M$ is a finitely generated module. There exists a *filtration* of $M$  $$M=M_t \supsetneq M_{t-1} \supsetneq M_{t-2} \supsetneq \cdots \supsetneq  M_1 \supsetneq M_0 = 0$$ such that $M_i / M_{i-1} \cong R/P_i$ for [[Prime Ideal|primes]] $P_i\in \Spec(R)$[^1]. This is a *prime filtration* of $M$.

If $R$ and $M$ are $\Z$-[[Graded Ring|graded]], there exists a prime filtration of $M$ where the [[Quotient Module|quotients]] $M_i / M_{i-1} \cong (R/P_i)(t_i)$ are [[Graded Module|graded modules]], the $P_i$ are [[Homogeneous Ideal|homogeneous]] primes, and $t_i \in \Z$.

##### *Proof.*
If $M\neq 0$, then $M$ has at least one associated prime, by \Cref{associated primes nonzero}, so there is an inclusion $R/P_1 \subseteq M$. Let $M_1$ be the image of this inclusion. If $M/M_1\neq 0$, it has an associated prime, so there is an $M_2 \subseteq M$ such that $R/P_2 \cong M_2/M_1 \subseteq R/M_1$. Continuing this process, we get a strictly ascending chain of submodules of $M$ where the successive quotients are of the form $R/P_i$. If we do not have $M_t=M$ for some $t$, then we get an infinite strictly ascending chain of submodules of $M$, which contradicts that $M$ is a noetherian module.

In the graded case, if $P_i$ is the annihilator of an element $m_i$ of degree $t_i$, we have a degree-preserving map $(R/P_i)(t_i)\cong R m_i$ sending the class of $1$ to $m_i$.

[^1]: Notation: [[Prime Spectrum]]