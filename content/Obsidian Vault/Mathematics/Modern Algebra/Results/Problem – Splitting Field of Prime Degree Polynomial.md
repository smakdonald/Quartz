### Problem 8 – Splitting Field of Prime Degree Polynomial
Let $f (x) = x^p-5 \in \Q[x]$ where $p$ is an odd prime, and let $L$ be the [[Splitting Field|splitting field]] of $f (x)$ over $\Q$. Find, with justification, $[L : \Q]$.

##### *Proof*.
Let $f (x) = x^p-5 \in \Q[x]$ where $p$ is an odd prime, and let $L$ be the splitting field of $f (x)$ over $\Q$. Using Eisenstein's Criterion with $p=5$ we see that $f$ is irreducible in $\Q[x]$. Notice that $\sqrt[p]5$ is a root of this polynomial. As $f$ is monic and irreducible it is the minimum polynomial of $\sqrt[p]5$, and thus $[\Q(\sqrt[p]5):\Q]=p$. Let $\z$ be a primitive $p\th$ root of unity. Notice that $\z$ is a root of the $(p-1)\th$ cyclotomic polynomial, $g(x)$, which is irreducible in $\Q[x]$ by the Gospel of Mark.

As $L$ is the splitting field of $g$, there exists a root $\a$ of $g\in L$. Consider $\Q(\sqrt[p]5,\a)$. As $\a$ is algebraic in $\Q(\sqrt[p]5,\a)$ we know there exists some unique irreducible minimal polynomial $h$ of degree $q$, and thus that $[\Q(\sqrt[p]5,\a):\Q(\sqrt[p]5)]=q$. By the Degree Formula we see $$[\Q(\sqrt[p]5,\a):\Q]=[\Q(\sqrt[p]5,\a):\Q(\sqrt[p]5][\Q(\sqrt[p]5:\Q]=pq.$$However, $[\Q(\sqrt[p]5,\a):\Q]=[\Q(\sqrt[p]5,\a):\Q(\a)][\Q(\a):\Q]$ and so $pq=(p-1)m$ for some $m\in\Z$, so $(p-1)|pq$. As $\gcd((p-1),p)=1$ we must have $(p-1)|q$. But $q$ was defined to be the degree of $h$, which divides $g$. As $(p-1)|q$ and $q\leq (p-1)$, we see that $(p-1)=q$, so $g=kh$ for some $k\in \Q$. As irreducible polynomials multiplied by a constant are still irreducible, we see that $g$ is indeed irreducible in $\Q(\sqrt[p]5)$. 

As $g$ is monic and irreducible in $\Q(\sqrt[p]5)$ we see that it is the minimum polynomial of $\z$, and thus $[\Q(\sqrt[p]5,\a):\Q(\sqrt[p]5)]=(p-1)$. As $\Q(\sqrt[p]5,\a)=L$, we have $[L:\Q]=p(p-1)$. 
***
#qual