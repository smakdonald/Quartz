#### $\lem$ – Matrix Invertible iff Columns Span $F^n$
Let $F$ be a [[Field|field]] and let $A$ be an $n \times n$ matrix for $n \geq 1$. $A$ is invertible if and only if its columns span $F^n$.

###### *Proof.* 
$A$ is invertible if and only if the associated linear map $g: F^n \to F^n$ given by $g(v) = Av$ is an isomorphism. By the rank-nullity Theorem, $\rank(g) = n$ if and only if $\ker(g) = \{0\}$ if and only if $g$ is an isomorphism. The result follows, since $\rank(g) = \dim_F \im(g)$ and $\im(g)$ is the span of the columns of $A$. 
***