## Section I: Group theory
Solve two of the following three problems.  
### Problem 1 – Characteristic Subgroup and Normality
[[Problem – Characteristic Subgroup and Normality]]
### Problem 2 – June 2014 (3a)
[[Problem – June 2014 (3a)]]
### Problem 3 – Groups of Order 60 and 30
[[Problem – Groups of Order 60 and 30]]
## Section II: Rings, Modules and Linear Algebra  
Solve two of the following three problems.  
### Problem 4 #unfinished
Let $d$ be a square-free integer. The ring $\Q(\sqrt d)$ is the subring of $\C$ defined by
$$\Q(\sqrt d) = \{a + b\sqrt d | a, b \in \Q\}.$$Show that there is a ring isomorphism $\Q[x]/(x^2-d)\cong\Q(\sqrt d)$.

##### *Proof.*
Let $f:\Q[x]\to\Q[\sqrt d]$ such that $f(x)=\sqrt{d}$. 

Let $a+b\sqrt d\in$$\Q(\sqrt d)$, and notice that $f(a+bx)=a+b\sqrt d$, giving us surjectivity. Also,
$$f((a+b\sqrt d)(p+q\sqrt d))=(a+bx)(p+qx)=f(a+b\sqrt d)f(p+q\sqrt d)$$ and $$f((a+b\sqrt d)+(p+q\sqrt d))=(a+bx)+(p+qx)=f(a+b\sqrt d)+f(p+q\sqrt d),$$making $f$ a homomorphism as well. 

Let $K=\Ker(f)$, and let $p=a+bx\in K$. As $\Q[x]$ is a division ring we can write $p(x)=(x^2-d)q(x)+r(x)$ for some $p(x),r(x)$ such that $r(x)=0$ or $\deg r(x)<\deg (x^2-d)$. Thus $r(x)$ has degree $1$, making $r(x)=sx+t$. 
***
### Problem 5 #unfinished
Let $A$ be a $\Z$–module and let $n$ be any integer. Show that there is a $\Z$-module isomorphism
$$\Hom_\Z(\Z/n\Z, A)\cong A_n, \text{ where }A_n = \{a \in A | na = 0\}$$
is a submodule of $A$. (Note: You may use the fact that $A_n$ is a $\Z$–module without proof.)

##### *Proof*.

***
### Problem 6 – Similarity Classes and CharPoly
[[Problem – Similarity Classes and CharPoly]]
## Section III: Fields and Galois Theory
Solve two of the following three problems.
### Problem 7 #unfinished 
Let $p$ be a prime integer and let $\a$ be a root of the polynomial $x^3-p$.

(a) Find, with justification, the degree of the field extension $\Q(\a, i)$ over $\Q$.
(b) Deduce that the polynomial $x^3-p$ is irreducible in $\Q(i)[x]$.

##### *Proof*.
Let $p$ be a prime integer and let $\a$ be a root of the polynomial  $f(x)=x^3-p$.

###### Part (a)
First, notice that by Eisenstein's Criterion ($p=p$) we have $f$ irreducible in $\Q[x]$. 

Let $\z$ be a primitive $3^{\text {rd}}$ root of unity. The roots of $f$ are the following:
$\a_1=\sqrt[3]p\cdot\z$
$\a_2=\sqrt[3]p\cdot\z^2$
$\a_3=\sqrt[3]p\cdot\z^3=\sqrt[3]p$

$[\Q(\sqrt[3]p):\Q]=3$.
$[\Q(\sqrt[3]p,i):\Q\sqrt[3]p]=2$
Total is $6$ by degree formula.

***
###### Part (b)
***
### Problem 8 – Algebraic but not Finite Extension
[[Problem – Algebraic but not Finite Extension]]
### Problem 9 – Galois Extensions of Degree 5 and 10
[[Problem – Galois Extensions of Degree 5 and 10]]