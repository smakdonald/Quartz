#### $\prop$ – $g(A)=0$ iff $g(x)$ Annihilates  $F^n_A$
Given an $n \times n$ matrix $A$ and polynomial $g(x)\in F[x]$[^2], we have $g(A) = 0$ if and only if $g(x)$ annihilates the $F[x]$-[[Module|module]] $F^n_A$. 

In particular, $\mp_A(x)$[^1] is the unique monic [[Generator|generator]] of the annihilator [[Ideal|ideal]] $$
\ann_{F[x]}(F^n_A) := \{ g(x) \in F[x] \mid g(x) \cdot v = 0 \text{ for all $v \in F^n_A$}\}.$$
###### *Proof.* 
If $g(A) = 0$, then for each $v \in F^n$, by definition of the action of $F[x]$ on $F^n_A$ we have
$$
g(x) \cdot v = g(A) v = 0
$$
and so $g(x)$ annihilates $F^n_A$. Conversely, if $g(x)$ annihilates $F^n_A$, then $g(A) \cdot v = 0$ for all $v \in F^n$. Taking $v = e_i$ for each $i$, this says that each column of $g(A)$ is $0$ and hence $g(A)$ is the zero matrix.
***

[^1]: See: [[Minimum Polynomial]]
[^2]: See: [[Polynomial Ring]]