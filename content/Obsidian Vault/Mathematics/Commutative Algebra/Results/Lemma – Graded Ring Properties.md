#### $\lem$ – Graded Ring Properties
Let $R$ be a $T$-[[Graded Ring|graded]] ring. 

(a) $1$ is [[Homogeneous Element|homogeneous]] of [[Homogeneous Element|degree]] $0 \in T$ (the identity of $T$).
(b) $R_0$ is a subring of $R$.
(c) Each $R_a$ is an $R_0$-module.

##### *Proof.*
(a) Write $1=\sum_a r_a$ with $r_a$ homogeneous of degree $a$. Then $r_0 = r_0 (\sum_a r_a) = \sum_a r_0 r_a$ implies $r_0 r_a = 0$ for $a\neq 0$. Similarly, for any other $a$ we have $r_a = r_a (\sum_b r_b)$, and thus $r_a = r_a r_0$ (here is where we use the cancellative assumption). Thus $r_a =0$ for $a\neq 0$, so $1\in R_0$.
(b) We have shown that $1 \in R_0$. Moreover, $R_0$ is a subgroup under addition, and $r,s\in R_0$ implies $rs\in R_0$.
(c) By assumption, $R_a$ is a subgroup under addition. Given $r\in R_0$ and $s\in R_a$ we must have $rs\in R_a$.