#### $\thm$ – Gauss's Lemma: Part 2
Let $R$ be a [[Principal Ideal Domain|PID]] and let $F$ be its [[Field of Fractions|field of fractions]], and assume $f(x) \in R[x]$[^1] is a non-constant polynomial with coefficients in $R$. $f(x)$ is [[Irreducible|irreducible]] in $R[x]$ if and only if it is irreducible in $F[x]$ and $\cont(f) = 1$[^2].

##### *Proof.*
($\Rightarrow$) Suppose $f(x) \in R[x]$ is irreducible.
Then $f(x) = \cont(f) g(x)$ for some $g(x) \in R[x]$. Since $f(x)$ is irreducible in $R[x]$, we must have $\cont(f) = 1$.

Suppose $f = gh$ with $g, h \in F[x]$. We can find an element $M$ of $R$ such that $M \cdot g(x) \in R[x]$. 
(We can take $M$ to be the product of all the denominators of the coefficients of $g$, for example; this is called "clearing denominators''.) Similarly, there is an $N \in R$ such that $N \cdot h(x) \in R[x]$.
Further, write $M \cdot g(x) = a \cdot l(x)$ where $a = \cont(M g(x)) \in R$, $l(x) \in R[x]$, and $\cont(l) = 1,$ and similarly $N \cdot g(x) = b \cdot m(x)$ where $b = \cont(N h(x)) \in R$, $m(x) \in R[x]$,  and $\cont(m) = 1$.We have $$abl(x)m(x) = MN f(x)$$Using Gauss's Lemma, Part 1, we have $\cont(lm) = \cont(l) \cont(m) = 1$ and hence
$$
\cont(ab l(x) m(x)) = ab \cont(l(x) m(x)) = ab.
$$
We also have $\cont(MNf(x)) = MN\cont(f) = MN$ (since we've already proven that $\cont(f) = 1$). 

So $ab = MN$ and thus by dividing we arrive at
$$
l(x) m(x) = f(x).
$$
But $f(x)$ is irreducible in $R[x]$. It follows that either $l$ or $m$ must be a unit in $R[x]$ (i.e., a unit in $R$) and it follows that either $g(x)$ or $h(x)$ is a unit in $F[x]$. This proves $f(x)$ is irreducible in $F[x]$.

($\Leftarrow$)  Say $f(x) \in R[x]$ irreducible in $F[x]$ and $\cont(f) = 1$. If $f = q(x) r(x)$ with $q,r \in R[x]$ then, since $f$ is irreducible in $F[x]$, one of $q$ or $r$ must be a constant. But since $\cont(f) = 1$, this constant must be $1$. 
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Content]]