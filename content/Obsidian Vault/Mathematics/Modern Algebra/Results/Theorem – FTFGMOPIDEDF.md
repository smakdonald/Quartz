#### $\thm$ – FTFGMOPIDEDF
Let $R$ be a [[Principal Ideal Domain|PID]] and let $M$ be a [[Generator|finitely generated]] $R$-[[Module|module]]. Then there exist integers $r \geq 0, k \geq 0$, prime elements $p_1,\ldots,p_s$ of $R$ (not necessarily distinct), and integers $e_1,\ldots ,e_s \geq 1$, such that $$M \cong R^r \oplus R/(p_1^{e_1}) \oplus \cdots \oplus R/(p_s^{e_s}).$$Moreover $r$ and $k$ are uniquely determined by $M$, and the list $p_1^{e_1},\ldots, p_s^{e_s}$ is unique up to [[Associates|associates]] and reordering. 
 
###### *Proof.* 
First write $M$ in invariant factor form $M \cong R^r \oplus R/(d_1) \oplus \dots \oplus R/(d_k)$. For any non-zero, non-unit element $d$ of $R$, we have $d = p_1^{e_1} \cdots p_m^{e_m}$ for some distinct (non-associate) prime elements $p_j$ and integers $e_j \geq 1$. By the Chinese remainder theorem (applied over and over again) we have $$R/(d)\cong R/(p_1^{e_1})  \oplus \cdots \oplus R/(p_m^{e_m})$$ Doing this for each fact $R/(d_i)$ in the invariant factor form of $M$ we obtain the existence of an elementary divisor form of $M$.
   
Uniqueness follows from the uniqueness of the invariant factor form and of the prime factorizations of the $d_i$'s.
***