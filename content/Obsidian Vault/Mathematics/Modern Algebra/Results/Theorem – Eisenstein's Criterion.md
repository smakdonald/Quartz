#### $\thm$ – Eisenstein's Criterion
Let $R$ be a [[Principal Ideal Domain|PID]] with [[Field of Fractions|field of fractions]] $F$ and assume $f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_0 \in R[x]$[^1] is a polynomial. Suppose there is a [[Mathematics/Modern Algebra/Definitions/Prime|prime]] element $p \in R$ such that $p \nmid a_n$, $p \mid a_i$[^2] for all $0 \leq i \leq n-1$, and $p^2 \nmid a_0$. Then $f$ is [[Irreducible|irreducible]] in $F[x]$.

##### *Proof.*
We have $f(x) = \cont(f) \cdot l(x)$ with $l(x) \in R[x]$ and $\cont(l) = 1$. Since $p$ does not divide the leading coefficient of $f$, we have $p \nmid \cont(f)$. It therefore follows that the three assumptions involving the coefficients of $f(x)$ are also satisfied by the coefficients $l(x)$. Moreover, $f$ is irreducible in $F[x]$ if and only  if $l(x)$ is irreducible in $F[x]$. We may therefore assume without loss of generality that $\cont(f) = 1$.

By Gauss's Lemma we just need to  prove it is irreducible in $R[x]$. Suppose $f(x) = g(x)h(x)$ with $g(x), h(x) \in R[x]$, where $$g(x) = b_m x^m + b_{m-1} x^{m-1} + \cdots + b_0$$and $$h(x) = c_l x^l + c_{l-1} x^{l-1} + \cdots + c_0$$where $m+l = n$ and $b_m c_l = a_n$. 

Upon modding out by $p$ we get $$\ov{f} = \ov{g} \ov{h} \in (R/p)[x].$$The assumptions on $f$ give that $$\ov{f} = \ov{a_n} x^n$$with $\ov{a_n} \ne 0$.  Since $R/p$ is a domain, it follows that $$\ov{g} = \ov{b_m} x^m \, \text{ and  } \, \ov{h} = \ov{c_l} x^l$$On the other hand, we also have $$a_0 = b_0c_0,$$and since $p^2 \nmid a_0$, we have that $p \nmid b_0$ or $p \nmid c_0$. So $\ov{b_0} \ne 0$ or $\ov{c_0} \ne 0$. This can only occur if $m = 0$ or $l = 0$.

We have shown that if $f$ factors in $R[x]$ as $f = g \cdot h$, then at least one of $g$ of $h$ must be a constant polynomial. Since $\cont(f) = 1$, this factor must be a unit. So $f$ is irreducible in $R[x]$. 
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[GCD|Divisor]]