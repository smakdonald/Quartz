#### $\thm$ – Universal Mapping Property of a Presentation
Let A be a set, let F(A) be the [[Free Group|free group]] on A, let R be a subset of F(A), let H be a [[Group|group]], and let $g:A \to H$ be a function satisfying the property that whenever $r = a_1^{i1} \cdots a_m^{i_m} \in R$, with each $a_j \in A, g_j \in G$ and $i_j \in \{1,-1\}$, then $$(g(a_1))^{i_1} \cdots (g(a_m))^{i_m} = e_H.$$Then there is a unique [[Homomorphism|homomorphism]] $\ov f: \langle A | R \rangle \to H$ satisfying $\ov f(a\langle R\rangle ^N) = g(a)$ for all $a \in A$.

###### *Proof.* 
By the [[Theorem – UMP for Free Groups|UMP]] of the free group there is a unique group homomorphism $\tilde f:F(A)\to H$ such that $f(a)=g(a)$ for all $a\in A$. Then for $r = a_1^{i1} \cdots a_m^{i_m} \in R$, we have $$f(r)=(g(a_1))^{i_1} \cdots (g(a_m))^{i_m} = e_H,$$showing that $R\subseteq \ker(f)$[^1]. Since $\ker(f)\norm F(A)$ and $\langle R\rangle ^N$[^2] is the smallest [[Normal Subgroup|normal]] [[Subgroup|subgroup]] containing $R$, it follows that $\langle R\rangle ^N\subseteq \ker(f)$. By the [[Theorem – UMP of a Quotient Group|UMP]] of the quotient, $f$ induces a group homomorphism $\ov f: G/\langle R\rangle ^N\to H$. Moreover, for each $a\in A$ we have  $g(a)=f(a)=\ov f(a\langle R\rangle ^N)$.
***

[^1]: See: [[Kernel]]
[^2]: See: [[Generator]]