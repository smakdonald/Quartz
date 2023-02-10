### Problem 8 – $R[x]$ a PID iff $R$ a Field
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] and $x$ an indeterminant. Prove that $R[x]$[^1] is a [[Principal Ideal Domain|PID]] if and only if R is a [[Field|field]].

##### *Proof*.
Let $R$ be a commutative ring and $x$ an indeterminant.

First, suppose $R[x]$ is a PID. Let $I$ be a nonzero [[Ideal|ideal]] in $R$, and consider the ideal $(I,x)\in R[x]$. As $R[x]$ is a PID we see $(I,x)=(z)$ for some $z\in R[x]$. Then $z|x$, but $x$ is an indeterminant and thus [[Irreducible|irreducible]], so $z$ must be a [[Unit|unit]] or $x$ itself. But $z$ also [[Generator|generates]] $I$, so $z$ can't be $x$, so $z$ is a unit, meaning $z\in R$ and so $I=(R)$. Thus the only ideals of $R$ are $(0)$ and $R$, making $R$ a field.

Next, suppose $R$ is a field. Let $J$ be an ideal in $R[x]$. If $J\in R$ then $J=R$ or $J=(0)$, both of which are [[Principal Ideal|principal]]. Thus $x\in J$, and so $J=(x)$, making $J$ principal as well. Hence $R[x]$ is a PID.  
***
#qual

[^1]: Notation: [[Polynomial Ring]]