#### $\thm$ – Gauss's Lemma: Part 1
Let $f(x), g(x) \in R[x]$[^1] where $R$ is a [[Principal Ideal Domain|PID]]. Then $\cont(fg) = \cont(f) \cont(g)$[^2] (up to [[Associates|associates]]).

##### *Proof.*
We first show the following special case: If $\cont(f) = 1$ and $\cont(g) = 1$, then $\cont(fg) =1$.

To see this, pick a prime $p \in R$ and write $\overline{f} \in (R/p)[x]$ for the result of modding out the coefficients of $f$ by $p$. Then $\ov{fg} = \ov{f}\ov{g}$ (since the map $R[x] \to (R/p)[x]$ sending $f$ to $\ov{f}$ is a ring map). Since $\cont(f) =1 = \cont(g)$, we have that $\ov{f} \ne 0$ and $\ov{g} \ne 0$. Since $(R/p)[x]$ is a domain, it follows that $\ov{fg} \ne 0$. This proves $p$ does not divide all of the coefficients of $fg$. Since $p$ was arbitrary, $\cont(fg) = 1$.

For the general case, let $f  = a h(x)$ and $g = b l(x)$ where $a =\cont(f)$ and $b = \cont(g)$. Note that $\cont(h) = 1 = \cont(l)$ and $fg = (ab) hl$. By the case already proven, $\cont(lh) =1$. It follows $\cont (abhl) =ab \cont(hl) = ab = \cont(f) \cont(g)$.
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Content]]