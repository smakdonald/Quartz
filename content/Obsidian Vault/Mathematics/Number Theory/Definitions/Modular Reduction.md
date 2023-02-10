#### $\defn$ – Modular Reduction
Given a polynomial $f \in\Z[x]$[^1], we obtain the *mod-$n$ reduction* of that polynomial $f \in\Z/(n)[x]$ by reducing all of its coefficients [[Mod|modulo]] $n$. 

[^1]: Notation: [[Integers]], [[Polynomial Ring]]

#### $\defn$ – Modular Reduction (2)
Given a $p$-adic integer 
$$\a = a_{0} + a_{1} p + a_{2} p^{2} + \cdots \in\Z_{p},$$
we define mod-$p$ reduction of $\a$ by $\a \mod p = a_{0}$ and more generally 
$$\a \mod p^{k} = a_{0} + a_{1} p + a_{2} p^{2} + \cdots + a_{k-1} p^{k-1}.$$
We will often abbreviate this, the truncation of $\a$ after $k$ terms, as simply $\a_{k}$. 
(Note that $\a_{k}$ does not have a $p^{k}$ term.) As we will see, it is not unreasonable to 
think of $\a$ as a limit, as in $\a = \lim_{k\to\infty} \a_{k}$.