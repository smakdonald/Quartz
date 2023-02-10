## Section I: Group theory
Solve two of the following three problems.  
### Problem 1 – Order $2^{m}\cdot 5$ Not Simple
[[Problem – Order $2{m}cdot 5$ Not Simple]]
### Problem 2 – $p$-group and Subgroups of Every Order
[[Problem – p-group and Subgroups of Every Order]]
### Problem 3 – Classify Groups of Order $3p$
[[Problem – Classify Groups of Order $3p$]]
## Section II: Field Theory and Galois theory  
Solve two of the following three problems.  
### Problem 4 – Unique Intermediate Field of Degree 5
[[Problem – Unique Intermediate Field of Degree 5]]
### Problem 5 #unfinished 
Let $L$ be the splitting field of the polynomial $x^7-18$ over $\Q$. Give, with full justification, a presentation for the Galois group $\Gal(L/\Q)$ that has two generators.

##### *Proof*.
Let $L$ be the splitting field of the polynomial $f(x)=x^7-18$ over $\Q$.
First, note that $f$ is irreducible in $\Q[x]$ by Eisenstein's Criterion ($p=2$). 
The roots of $f$ are the following:
- $a_1=\sqrt[7]{18}e^{\frac{2\pi i}{7}}$,
- $a_2=\sqrt[7]{18}e^{\frac{4\pi i}{7}}$,
- $a_3=\sqrt[7]{18}e^{\frac{6\pi i}{7}}$,
- $a_4=\sqrt[7]{18}e^{\frac{8\pi i}{7}}$,
- $a_5=\sqrt[7]{18}e^{\frac{10\pi i}{7}}$,
- $a_6=\sqrt[7]{18}e^{\frac{12\pi i}{7}}$, and
- $a_7=\sqrt[7]{18}e^{\frac{14\pi i}{7}}=\sqrt[7]{18}$.
Let $\z=e^{\frac{2\pi i}{7}}$, which is the root of the $7\th$ cyclotomic polynomial (which has degree $6,$ and thus irreducible in $\Q[x]$. Let $F=\Q(\z)$ and $E=\Q(\sqrt[7]{18})$. Thus we have $[F:\Q]=6$ and $[E:\Q]=7$. By the $\gcd$ irreducible argument we see that $[L:\Q]=42$. Yeesh.

Let $G=\Gal(L/\Q)$. 
From Sylow's Theorem we have the following:
$n_7=1$, as $7\not\mid6$,
$n_3|14$ and $n_3\equiv1\mod3$, so $n_3$ is either $1$ or $7$. 
***
### Problem 6 – Strict Inequality of Automorphism Group
[[Problem – Strict Inequality of Automorphism Group]]
## Section III: Ring theory and Linear Algebra
Solve two of the following three problems.
### Problem 7 #unfinished 
Let $R$ be a PID and $S$ a multiplicatively closed subset of $R$ such that $0 \not\in S$. Prove that $S\inv R$ is also a PID. Tip: Given an ideal $I$ of $S\inv R$, consider $I \cap R$.

##### *Proof*.
Let $R$ be a PID, $S$ a multiplicatively closed subset of $R$ such that $0 \not\in S$, and $I$ an ideal in $S\inv R$. Consider $I \cap R$, which is an ideal in $R$ and is thus generated by some $x\in R$. 
***
### Problem 8 #unfinished 
Find, with justification, all the ideals of the ring $\Z[x]$ that contain the ideal $I = (3, x^3 + x + 1)$.

##### *Proof*.
First, notice that $x^3+x+1$ is irreducible in $\Z[x]$ by the Rational Root Test. Thus the possibilities are the following:
- $I=(3,x^3+x+1)$,
- $\Z[x]$.
Let $J$ be an ideal containing $I$.
*** 
### Problem 9 – January 2016 (7)
[[Problem – January 2016 (7)]]