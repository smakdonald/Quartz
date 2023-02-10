#### $\prop$ – Algebraic Extensions are Transitive
If $F \subseteq L$ and $L \subseteq E$ are both [[Algebraic Extension|algebraic]] [[Field|field]] [[Field Extension|extensions]], then so is $F \subseteq E$.

##### *Proof.*
Pick $\a \in E$. We need to prove $\a$ is a root of some polynomial with coefficients in $F$. This is surprisingly hard to prove directly and indeed the proof is rather non-constructive.

Since $\a$ is [[Algebraic Element|algebraic]] over $L$, it is the root of some polynomial[^1] $$a_nx^n + \cdots + a_1 x + a_0 \in L[x].$$Note that this polynomial belongs to $F(a_0,\dots, a_{n})[x]$[^2] too, and so $\a$ is algebraic over $F(a_0, \dots, a_{n})$.

We consider the chain of field extensions
$$F \subseteq F(a_0) \subseteq F(a_0,a_1) \subseteq \cdots \subseteq F(a_0, a_1, \dots, a_{n-1} )\subseteq F(a_0, \dots, a_{n}, \a)$$
Since $a_i$ is algebraic over $F$ for all $i$ and $\a$ is algebraic over $F(a_0, a_1, \dots, a_{n})$, by this [[Theorem – Properties of Algebraic Elements|Theorem]] each step in this chain has finite [[Degree of Field Extension|degree]]. By the [[Proposition – The Degree Formula|Degree Formula]], $[F(a_0, \dots, a_{n}, \a): F]$ is finite and thus so is $[F(\a):F]$. By the Theorem again, $\a$ is algebraic over $F$.
***

[^1]: For $L[x]$, See: [[Polynomial Ring]]
[^2]: See: [[Field Extension]]