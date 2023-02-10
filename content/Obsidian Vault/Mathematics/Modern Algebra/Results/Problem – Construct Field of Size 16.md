### Problem 9 – Construct Field of Size 16
(a) Let $F$ be a [[Field|field]] and $f\subseteq F [x]$[^1] be [[Irreducible|irreducible]]. Prove the $F [x]/(f )$[^2] is a field.
(b) Give an explicit construction (with justification) of a field of size $16$. (You may use without proof that the unique irreducible quadratic in $\F_2[x]$ is $x^2 + x + 1.)$

##### *Proof*.
###### Part (a)
Let $F$ be a field and $f\subseteq F [x]$ be irreducible. Thus $f$ is prime, making $(f)$ a prime ideal in $F[x]$ and $F[x]/(f)$ a domain. Suppose that there existed a proper ideal $I$ such that $(f)\subseteq I$. However, as $F$ is a field we know that $F[x]$ is a PID, meaning $I=(g)$ for some $g\in F[x]$. If $f\in(g)$ then $g|f$, meaning that $f=g$. Thus $(f)$ is a maximal ideal and we have $F[x]/(f)$ a field. 
***
###### Part (b)
Let $F=\F_2$. Let $f=x^4+x+1$. Suppose $f=gh$ with $g,h$ irreducible. Thus either both $g$ and $h$ have degree $2$ or one of them has degree $1$. As $f\neq (x^2+x+1)^2$, we see that without loss of generality $\deg g=1$. Then $g=x$ or $x+1$, but neither divide $f$. Thus $f$ is irreducible, making $F[x]/(f)$ a field, the elements of which are:
1. 0
2. 1
3. $x$
4. $x+1$
5. $x^2$
6. $x^2+1$
7. $x^2+x$
8. $x^2+x+1$
9. $x^3$
10. $x^3+1$
11. $x^3+x$
12. $x^3+x^2$
13. $x^3+x+1$
14. $x^3+x^2+1$
15. $x^3+x^2+x$
16. $x^3+x^2+x+1$,
making it a field of order $16$. 
***
#qual

[^1]: Notation: [[Polynomial Ring]]
[^2]: Notation: [[Principal Ideal]], [[Quotient Ring]]