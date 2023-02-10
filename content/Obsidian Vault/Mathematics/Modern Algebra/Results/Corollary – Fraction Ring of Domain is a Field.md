#### $\cor$ – Fraction Ring of Domain is a Field
Let $R$ be an [[Integral Domain|integral domain]] and let $S = R \setminus \{0\}$. Then $S$ is a [[Multiplicatively Closed Set|multiplicatively closed]] subset of non-[[Zero-Divisor|zerodivisors]] and  $S^{-1}R$ is a [[Field|field]].

###### *Proof.* 
$R$ being a domain means $xy=0$ implies ($x=0$ or $y=0$). The contrapositive to this statement is: if $x\neq 0$ and $y\neq 0$ then $xy\neq 0$, which shows $S$ is a multiplicatively closed set of nonzerodivisors.
 
It remains only to show every non-zero element of $S^{-1}R$ is a unit. Given $\frac{r}{s} \ne 0$, note that $r \ne 0$ and hence $r \in S$. So
$\frac{s}{r}$ is also an element of $S^{-1}R$. We have $\frac{r}{s} \frac{s}{r} = \frac{sr}{sr} = \frac{1}{1}$, where the last equation holds by the definition
of $\sim$.
***