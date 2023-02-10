#### $\prop$ – Characteristic in Local Rings
Let $(R,\m,k)$ be a [[Local Ring|local ring]]. Then one of the following holds:
(a) $\Char(R)=\Char(k)=0$[^1]. We say that $R$ has *equal characteristic zero*.
(b) $\Char(R)=0$, $\Char(k)=p$ for a prime $p$, so $R$ has *mixed characteristic* $(0,p)$
(c) $\Char(R)=\Char(k)=p$ for a prime $p$, so $R$ has *equal characteristic* $p$.
(d) $\Char(R)=p^n$, $\Char(k)=p$ for a prime $p$ and an integer $n>1$.
If $R$ is [[Reduced Ring|reduced]], then one of the first three cases holds.

##### *Proof.*
Since $k$ is a quotient of $R$, the characteristic of $R$ must be a multiple of the characteristic of $k$, since the map $\Z\longrightarrow k$ factors through $R$. We must think of $0$ as a multiple of any integer for this to make sense. Now $k$ is a field, so its characteristic is $0$ or $p$ for a prime $p$. If $\Char(k)=0$, then necessarily $\Char(R)=0$. If $\Char(k)=p$, we claim that $\Char(R)$ must be either $0$ or a power of $p$. Indeed, if we write $\Char(R)=p^n \cdot a$ with $a$ coprime to $p$, note that $p\in \m$, so if $a \in \m$, we have $1\in (p,a)\subseteq \m$, which is a contradiction. Since $R$ is local, this means that $a$ is a unit. But then, $p^n a=0$ implies $p^n=0$, so the characteristic must be $p^n$.

[^1]: Notation: [[Ring Characteristic]]