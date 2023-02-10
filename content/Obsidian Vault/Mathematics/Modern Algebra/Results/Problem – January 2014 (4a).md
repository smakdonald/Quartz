### Problem 5 – January 2014 (4a)
Let $F$ be a [[Field|field]] and $G$ a [[Order|finite]] [[Subgroup|subgroup]] of $F^*$, the multiplicative [[Group of Units|group of units]] of $F$ . Prove that $G$ is [[Cyclic|cyclic]].

##### *Proof*.
Let $G$ be a finite subgroup of $F^*$. Let $|G|=n$. 

Let $k$ be the LCM of all orders of elements in $G$. Then $g^k=1$ and thus $g$ is a root of the polynomial $x^k-1$ for all $g\in G$. By Lagrange's Theorem every element divides $n$, and so we have $k\leq n$. However, by the Factor Theorem the polynomial $x^k-1$ can have at most $k$ roots, and we have $n$ distinct elements, and thus we have $k=n$. Thus there must exist an element of order $n$ in $G$, making $G$ cyclic, as desired.
***
#qual