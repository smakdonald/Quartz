### Problem 2 – Finite Group Action and p-group
Let $G$ be a [[Group|group]] of [[Order|order]] $p^n$, for some prime $p$, [[Group Action|acting]] on a finite set $X$.

(a) Suppose $p$ does not divide $|X|$. Prove that there exists some element of $X$ fixed by all elements of $G$.
(b) Suppose $G$ acts [[Faithful Action|faithfully]] on $X$. Prove that $|X| \geq np$.

##### *Proof.*
Let $G$ be a group of order $p^n$, for some prime $p$, acting on a finite set $X$.

###### Part (a)
We proceed via the contrapositive. Suppose there is no element in $X$ that is fixed by all elements of $G$. 

By Orbit-Stabilizer we know that $|\Orb_G(x)|\big||G|$ for all $x\in X$. Thus every orbit under this action has an order dividing $p^n$, so either $1$ or some positive power of $p.$ However, as no element of $X$ is fixed by every element of $G$, there exists no stabilizer which is all of $G$, and thus there exist no orbits that have order $1$. 

Recall that the orbits of this action partition $X$, and thus $|X|=\sum_{x\in X}|\Orb_G(x)|$. As every orbit is divisible by $p$, so too must be $X$.
***
###### Part (b)
Suppose $G$ acts faithfully on $X$. Thus the permutation representation homomorphism $\rho:G\to\Perm(X)$ is injective. Let $k$ denote the order of $X$. Then $\Perm(X)\cong S_k$, which as order $k!$. As $G$ is injective, we see that $|G|=|\im\rho|\leq S_k$, and thus $p^n|k!$. 

Thus $p$ must show up in the factorization of $k!$ at least $n$ times, meaning that $|X| \geq np$.
***
#qual