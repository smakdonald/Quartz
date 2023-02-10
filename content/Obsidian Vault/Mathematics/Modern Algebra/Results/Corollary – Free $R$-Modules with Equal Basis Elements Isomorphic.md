#### $\cor$ – Free Modules with Equal Basis Elements Isomorphic
If $M$ and $N$ are [[Basis and Free Module|free]] $R$-[[Module|modules]] having [[Basis and Free Module|bases]] of the same cardinality, then $M$ and $N$ are [[Isomorphism|isomorphic]] $R$-modules.

More precisely, if $A$ is a basis of $M$ and $B$ is a basis of $N$ and $j:A\to B$ is a bijection of sets, then there is a unique $R$-module isomorphism $h: M \xra{\cong} N$ such that $h|_A = j$[^1].

###### *Proof.* 
Let $h:M\to N$ and $h':N\to M$ be the $R$-module homomorphisms induced by the bijection $j:A\to B$ and its inverse $j^{-1}:B\to A$, respectively, using the UMP for free modules. We'll show that $h$ and $h'$ are mutual inverses. For this note that $h'\circ h:N\to N$ is an $R$-module homomorphism and $(h'\circ h)(b)=h'(j(b))=j^{-1}(j(b))=b$ for every $b\in B$. Since the identity map $\id_N$ is also an $R$-module homomorphism such that  $id_N(b)=b$ for every $b\in B$, by the uniqueness clause in the UMP, we have $h'\circ h=\id_n$. Similarly $h\circ h'=\id_M$.
***

[^1]: Notation: [[Restriction]]