#### $\defn$ – Group Ring
Let $G = (G, \cdot)$ be a [[Group|group]] and let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] with $1\neq 0$ (often $R$ is taken to be a [[Field|field]]). Let $R[G]$ be the collection of formal expressions of the form indicated below, where the $+$ [[Binary Operation|operation]] is assumed to be commutative:
$$R[G]=\left\{r_1 g_1 + r_2 g_2 + \dots + r_n g_n, n \geq 0, r_i \in R, g_i \in G\right\}.$$
Equivalently, a typical element of $R[G]$ can be written as $\sum_{g \in G} r_g g$, where $r_g \in R$ for all $g$ and $r_g = 0$ for all but a finite number of $g$'s.

We can make $R[G]$ into a [[Ring|ring]] by defining
$$\left(\sum_{g \in G} r_g g\right) +\left(\sum_{g \in G} s_g g\right) = \sum_{g \in G}  (r_g+ s_g) g$$
and
$$\left(\sum_{g \in G}  r_g g\right) \cdot \left(\sum_{h \in G}  s_h h\right) = \sum_{z \in G}  \sum_{(g,h), gh = z} r_g s_h z.$$
With these definitions, $R[G]$ is a ring, called the *group ring* of $G$ with coefficients in $R$. It is a [[Unital Ring|unital]] ring with identity $1_Re_G$. If $R=F$ is a field then $F[G]$ is an $F$-[[Vector Space|vector space]].
***