#### $\cor$ – Cubes and $\Z/(p)$
If $p$ is a [[Prime|prime]] with $p \mod 3 = 2$[^1], then every element of the ring $\Z/( p)$[^2] is a cube.

##### *Proof.*
Define $\varphi : \Z/( p) \to \Z/( p)$ by $\varphi(x) = x^{3}$. We claim that $\varphi$ is a [[Bijective|bijection]], for which it suffices, since $\Z/( p)$ is finite, to show it is an injection. Suppose $a, b \in  \Z/( p)$ satisfy $a^3 = b^3$ . Since $\Z/( p)$ is a [[Field|field]] (and hence has no zero divisors), if  $a^3 = b^3 = [0]$, then $a = b = [0]$. More interestingly, if $a^3 = b^3 = [0]$, then $a, b= [0]$ and so each is a [[Unit|unit]]$\mod p$, and we can write $(ab-1)^3 = [1]$. Now if $a= b$, then $ab-1$ has order $3$, and so [[Theorem – Lagrange’s Lemma|Lagrange’s Theorem]] implies that $3 | |\Z/( p)| = p - 1$. But this contradicts that $p \equiv 2 \mod 3$. So $a = b$, proving injectivity, hence bijectivity, hence surjectivity.

[^1]: Notation: [[Mod]]
[^2]: Notation: [[Z(n)]]