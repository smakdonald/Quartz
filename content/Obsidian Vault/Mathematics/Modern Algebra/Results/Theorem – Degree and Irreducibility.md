#### $\thm$ – Degree and Irreducibility
Let $F$ be a [[Field|field]] and $p(x) \in F[x]$[^1].
1. If $p$ has [[Polynomial Degree|degree]] one, it is [[Irreducible|irreducible]]. 
2. If $p$ has a root $a \in F$ and $\deg(p) \geq 2$, then $p(x)$ is not irreducible (since it factors as $p = (x-a)q$ for some $q$ of degree at least $1$).
3. If $2 \leq \deg(p) \leq 3$, then $p(x)$ is irreducible if and only if $p(x)$ has no roots.
4. (Rational Root Test) If $p(x) \in \Q[x]$ and all the coefficients of $p = a_n x^n + \cdots + a_0$ are integers and $\frac{i}{j}$ is a root of $p$ with $i,j \in \Z$, then $j$ [[GCD|divides]] $a_n$ and $i$ divides $a_0$. More generally, the same holds with $\Z$ replaced by any PID and $\Q$ replaced by its [[Field of Fractions|field of fractions]].

##### *Proof.*
***

[^1]: See: [[Polynomial Ring]]