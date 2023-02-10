### Problem 9 – Separable, Factorization, and Irreducibility
Assume $F$ is [[Field|field]] and let $f(x)\in F [x]$. Recall that $f (x)$ is [[Separable|separable]] if $f (x)$ has no repeated roots in an [[Algebraic Closure|algebraic closure]] of $F$.

(a) Assume $\char(F) = 0$[^1]. Prove that $f(x)$ is separable if and only if the [[Irreducible|irreducible]] factorization of $f(x)$ in $F[x]$ has no repeated factors.
(b) Fix a prime integer $p$, let $\F_p$ be the field with $p$ elements, and let $F$ be the [[Field of Fractions|field of fractions]] of the [[Polynomial Ring|polynomial ring]] $\F_{p}[y]$. Prove $x^p-y$ is irreducible in $F[x]$ but not separable.

##### *Proof.*

###### Part (a)
$(\Rightarrow)$ Suppose that $f$ is not separable, so $f$ has a repeated root in $\overline{F}$, which we denote $\alpha$. So $x-\alpha$ is a factor of $f(x)$. By Corollary 2.96, $F(\alpha)$ is separable, so the minimal polynomial of $\alpha$ in $F[x]$ has no repeated root in $\overline{F}$. As $f$ does have a repeated root (by supposition) it cannot be the minimum polynomial of $\alpha$. Thus $f(x)=\mp_{\alpha,F[x]}(x)g(x)$ for some $g(x)\in F[x]$ such that $g(x)$ has $\alpha$ as a root, otherwise $f$ would not obtain its repeated root. However, this means that $\mp_{\alpha,F[x]}(x)\big|g(x)$, meaning that $g(x)$ has $x-\alpha$ as a factor as well. Thus we see that $x-\alpha$ is a repeated factor of $f(x)$, one from the minimum polynomial, one from $g(x)$.

$(\Leftarrow)$ Suppose that the prime factorization of $f(x)$ in $F[x]$ admits a repeated factor. Thus there exists some prime (and thus irreducible) $g(x)$ such that $g(x)g(x)|f(x)$. However, $g$ has a root $\alpha$ in $\overline{F}$, so in $F(\alpha)$ we see that $f(x)$ has $\alpha$ as a root as well, as $g(a)=0$. But since $g(x)$ has factor $x-\alpha$, it shows up twice in the factorization of $f$ because $g(x)g(x)|f(x)$. So $\alpha$ has multiplicity at least 2, so $f$ is not separable. 
***
###### Part (b)
Let $y,z$ be indeterminants, $F=\F_{p}[y]$, and $L=\F_{p}[z]$ such that $z^3=y$ (as seen in Example 2.78). Note then that $z^3$ is a root of the polynomial $x^p-y\in F[x]$.

Moreover, since $F$ is the field of fractions of the PID $R=\F_{p}[y]$ and $y$ is a prime element of $R$, we may apply Eisenstein's Criterion (using $p=y$) to conclude that $x^p-y$ is irreducible in $F[x]$. Thus $x^p-y$ is the minimum polynomial of $z$ in $F[x]$.

However, as the derivative of this polynomial is $0$, we see that the $\mp_{z,F[x]}(x)$ is not separable by Proposition 2.72. However, by the Freshman's Dream, we see that $x^3-y=x^p-z^p=(x-z)^p\in L$. But as $z\not\in F$, we see that the prime factorization of $x^p-y$ admits no repeated factor.
***
#qual

[^1]: Notation: [[Ring Characteristic]]