#### Lemma – Algebras and Localizations
Let $R$ be a commutative ring, $r \in R$ an element of $R$, and $S = \{r^j \mid j \geq 1\}$ the multiplicatively closed subset of $R$ generated by $r$. There is an isomorphism$$\alpha:R[y]/(1 -yr) \xra{\cong} S^{-1}R$$of $R$-algebras given by $\alpha(\overline{g(y)}) =g\left(\frac{1}{r}\right).$

##### *Proof.*
There is a unique morphism of $R$-algebras $\tilde{\alpha}: R[y] \to S^{-1}R$ given by evaluation at $\frac{1}{r}$: $$\tilde{\alpha}(g(y)) = g\left(\frac{1}{r}\right).$$Since $1-yr$ is in the kernel of $\tilde{\alpha}$, it induces the ring map $\alpha$ in the statement of the lemma. 

The map $R \to R[y]/(1-yr)$ induced by the inclusion of $R$ into $R[y]$ sends $r$ to a unit whose inverse is $y$,  and thus there is an induced ring map
$$\beta: S^{-1}R \to R[y]/(1-yr)$$given by $$\beta\left(\frac{x}{r^j}\right) = xy^j.$$The composition $\alpha \circ \beta$ sends $\frac{x}{r^j}$ to $x(\frac{1}{r})^j$ and thus is the identity map. The composition $\beta \circ \alpha$ fixes elements in the image of $R \to R[y]/(1-yr)$ and sends $y$ to $y$, and hence it too is the identity.