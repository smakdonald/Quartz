#### $\thm$ – Universal Mapping Property for Free Groups
Let $A$ be a set, let $F(A)$ be the [[Free Group|free group]] on $A$, let $H$ be a [[Group|group]], and let $g:A \to H$ be a function. Then there is a unique [[Homomorphism|homomorphism]] $f:F(A) \to H$ satisfying $f(a) = g(a)$ for all $a \in A$.

###### *Proof.* 
Set $f:F(A) \to H$ to be given by $$f(a_1^{i_1}a_2^{i_2}\cdots a_m^{i_m})=g(a_1)^{i_1}g(a_2)^{i_2}\cdots g(a_m)^{a_m}$$ for any  $m\geq 0, a_j\in A, i_j\in\{-1,1\}$. One checks that $f$ is well defined by noting that
$$f(a_1^{i_1}a_2^{i_2}\cdots aa^{-1}\cdots a_m^{i_m})=g(a_1)^{i_1}g(a_2)^{i_2}\cdots g(a)g(a)^{-1}\cdots g(a_m)^{a_m}=f(a_1^{i_1}a_2^{i_2}\cdots a_m^{i_m})$$for any $a\in G$ and similarly for inserting $a^{-1}a$. The fact that $f$ is a group homomorphism and its uniqueness are left as an easy exercise. #fix
***