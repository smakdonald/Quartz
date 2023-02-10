#### $\prop$ – Every Cyclic $R$-module $\cong$ to $R/I$ for some $I$
Every [[Cyclic|cyclic]] $R$-[[Module|module]] is [[Isomorphism|isomorphic]] to $R/I$[^1] for some left [[Ideal|ideal]] $I$.

###### *Proof.* 
Say $M$ is cyclic and $m \in M$ is a generator of $M$, so that $M = \{rm \mid r \in R\}$. Define $f: R \to M$ to be the unique $R$-map with $f(1) = m$. Here I am applying the UMP for bases, using that $\{1\}$ is a basis of $R$ as a left $R$-modules. More explicitly, $$f(r) = f(r\cdot 1) = r f(1) = rm$$ for all $r \in R$. Then $f$ is onto, since $m$ generates $M$. Its kernel is a left ideal $I$ of $R$, since submodules of $R$ are the same thing as left ideals. By the FIT, there is an isomorphism $R/I \xra{\cong} M$ sending $r + I$ to $rm$.
***

[^1]: See: [[Quotient Ring]]