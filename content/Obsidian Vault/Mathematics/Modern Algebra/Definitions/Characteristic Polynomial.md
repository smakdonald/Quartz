#### $\defn$ – Characteristic Polynomial
Let $A \in \Mat_{n \times n}(F)$ where $F$ is a [[Field|field]]. The *characteristic polynomial* of $A$ is[^1]
$$\cp_A(x) := \det(x I_n - A) \in F[x].$$
Note that $\cp_A(x)$ is a monic polynomial of [[Polynomial Degree|degree]] $n$ with coefficients in $F$.
More generally, if $V$ is a [[Dim (Vector Space)|finite dimensional]] $F$-[[Vector Space|vector space]] and $g: V \to V$ is an $F$-[[Linear Operator|linear operator]] on $V$, then
$$\cp_g(x) := \cp_A(x)$$
where $A$ is the matrix [[Homomorphism Matrix|representing]] $g$ with respect to a choice of [[Basis and Free Module|basis]] of $V$.
***

[^1]: For $\det$, See: [[Determinant]]