#### $\thm$ – Gauss's Lemma
Let $R$ be a [[Unique Factorization Domain|UFD]]  with [[Field of Fractions|field of fractions]] $F$. Regard $R$ as a [[Subring|subring]] of $F$ and view elements in $R[x]$[^1] as also being elements of $F[x]$ via the induced map $R[x]\hookrightarrow F[x]$.
1. If $f(x) \in R[x]$ is [[Irreducible|irreducible]] in $R[x]$, then $f(x)$ remains irreducible as an element of $F[x]$.
2. If $f(x) \in R[x]$ is irreducible in $F[x]$ and the $\gcd$[^2] of the coefficients of $f(x)$ is a [[Unit|unit]], then $f(x)$ remains irreducible as an element of $R[x]$.

###### *Proof.* 
We will prove the contrapositive:  if $f(x) \in R[x]$ is reducible  in $F[x]$,  then it is also reducible in $R[x]$. Say $f(x)$ factors nontrivially as $f(x) = A(x)B(x)$ in $F[x]$. Since $F$ is a field, the units of $F[x]$ are the non-zero constant polynomials, and so having a nontrivial factorization means $\deg(A(x)), \deg(B(x)) > 0$. Each coefficient of $A$ and $B$ is a fraction, and so it is clear we can find a non-zero $d \in R$ such that $d f(x) = a(x) b(x)$ where $a(x), b(x) \in R[x]$ have positive degree.
  

If $d$ is a unit in $R$, then
$$
f(x) = (d^{-1}a(x)) b(x)
$$
is a non-trivial factorization in $R[x]$ (since $R[x]^\times = R^\times$).

If $d$ is not a unit, let $d = p_1 \cdots p_m$, $m \geq 1$, be an irreducible factorization of $d$. Since $p_1$ is irreducbile and $R$ is a
UFD, it is a prime element. We thus mod out by $p_1$ to get an equation
$$
0 \cdot \ov{p}(x) = \ov{a}(x) \ov{b}(x)
$$
in $(R/(p_1))[x]$ (where overlines denote applying the canonical map
$R \onto R/p_1$ to the coefficient of a poylnomial). Since $p_1$ is irreducible it is prime by the first bullet point on p.92 and thus $R/(p_1)$ is an integral domain. Hence $R/(p_1)[x]$ is also an integral domain.  We must therefore have $\ov{a}(x) = 0$ or
$\ov{b}(x) = 0$. That is, either $p_1$ divides every coefficient of $a(x)$ or every coefficient of $b(x)$. Either way, we may divide
$d f(x) = a(x) b(x)$ through by $p_1$ to obtain
$$
d' f(x) = a'(x) b'(x)
$$
in which $d'$ has one fewer irreducible factors than $d$. Repeating the argument, we arrive at an equation of the form $u f(x) = a''(x)b''(x)$ in $R[x]$ where $u$ is a unit, and this case was already handled.

2. Again, we prove the contrapositive: if $f(x)$ is reducible in $R[x]$ then it is also reducible in $F[x]$. Suppose $f(x)$ factors nontrivially   in $R[x]$ as $f(x) = g(x) h(x)$ with $g(x), h(x)$ non-units.
If both $g$ and $h$ have positive degree, then they remain non-units in $F[x]$ and so $f(x)$  is reducible in that ring too. Otherwise, without loss, suppose $g(x)$ is the constant polynomial $r$.
Then $r$ must not be a unit in $R$ and, since $f(x) = rh(x)$, the coefficients of $f(x)$ have a common factor of $r$, contrary to the
assumption.
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[GCD|gcd]]