#### $\lem$ – Integral Preserved by Localization
Let $R \to S$ be [[Integral Element|integral]], and let $W$ be a [[Multiplicatively Closed Set|multiplicatively closed]] subset of $R$. Then $W^{-1}R \to W^{-1}S$ is integral.

##### *Proof.*
Since $W$ is a multiplicatively closed subset of $R$, its image in $S$ is also multiplicatively closed.
Given $x\in S$ and $w\in W$, then we have equations of the form
$$x^n + r_1 x^{n-1} + \cdots + r_n = 0 \implies \left( \frac{x}{w} \right)^n + \frac{r_1}{w} \left( \frac{x}{w} \right)^{n-1} + \cdots + \frac{r_n}{w^n}  =0.$$
Thus $\frac{x}{w}$ is integral over $W^{-1}S$, and $S$ is integral over $R$.