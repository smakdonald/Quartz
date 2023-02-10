#### $\cor$ – Rank Nullity Theorem
Let $F$ be a [[Field|field]] and $f: V \to W$  an $F$-[[Linear Transformation|linear transformation]] between $F$-[[Vector Space|vector spaces]] $V$ and $W$, and assume $V$ is [[Dim (Vector Space)|finite dimensional]].  Then $$\dim(V) = \rank(f) + \nullity(f)$$ or equivalently $$\dim(V) = \dim(\ker(f)) + \dim(\im(f)).$$

###### *Proof.* 
By the first isomorphism theorem for modules we have $V/\ker(f)\cong\im(f)$, thus $\dim\left(V/\ker(f)\right)=\dim(\im(f))$. By the previous theorem we have $$ \dim(V)=\dim(\ker(f)) \dim\left(V/\ker(f)\right) =\dim(\ker(V))+\dim(\im(f)).$$
***