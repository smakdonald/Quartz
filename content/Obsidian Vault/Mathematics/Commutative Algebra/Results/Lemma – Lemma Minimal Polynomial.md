#### $\lem$ – Lemma Minimal Polynomial
Let $R$ be a [[Normal Domain|normal domain]] and let $x$ be an element in some larger domain that is [[Integral Element|integral]] over $R$. Let $k$ be the [[Field of Fractions|fraction field]] of $R$, and $f(t)\in k[t]$ be the [[Minimum Polynomial|minimal polynomial]] of $x$ over $k$. #eltypo 
(a) If  $x$ is integral over $R$, then $f(t) \in R[t]\subseteq k[t]$.
(b) If $x$ is integral over a [[Prime Ideal|prime]] $P$, then $f(t)$ has all of its nonleading coefficients in $P$.

##### *Proof.*
Let $x$ be integral over $R$. Fix an algebraic closure of $k$ containing $x$, and let $x_1~=~x$, $x_2,\ldots,x_u$ be the roots of $f$. Since $f(t)$ divides any polynomial with coefficients in $k$ that $x$ satisfies, it also divides a monic equation of integral dependance for $x$ over $R$. Therefore, each $x_i$ is a solution to such an equation of integral dependence, and thus must be integral over $R$.

Let $S=R[x_1,\dots,x_u] \subseteq \overline{k}$. This is a module-finite extension of $R$, so all of its elements are integral over $R$. The leading coefficient of $f(t)$ is 1, and the remaining coefficients of $f(t)$ are polynomials in the $x_i$, hence they lie in $S$. On the other hand, $R$ is normal, so $S \cap k = R$. We conclude that all the coefficients of $f$ are in $R$, and $f \in R[t]$.

Now let $x$ be integral over $P$. By the same argument as above, all of the $x_i$ are integral over $P$. Since each $x_i \in \overline{P}^S$, any polynomial in the $x_i$ lies in $\overline{P}^S$. So the nonleading coefficients of $f$ lie in $\overline{P}^S \cap R = P$, by \Cref{lying over}.