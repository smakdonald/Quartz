### Problem 5 – When $x^n=x$ all Prime Ideals are Maximal
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] in which every element $x$ satisfies $x^n = x$ for some $n > 1.$ Show that every [[Mathematics/Modern Algebra/Definitions/Prime|prime]] [[Ideal|ideal]] in R is [[Maximal Ideal|maximal]].

##### *Proof.*
Let $R$ be a commutative ring in which every element $x$ satisfies $x^n = x$ for some $n > 1.$ Let $P$ be a prime ideal in $R$. We examine $R/P$, which is a domain since $P$ is prime. 

Let $rP\in R/P$, meaning $r\not\in P$. Then $(rP)^n=r^nP=rP$ for some $n>1$. As $R/P$ is a domain we can cancel an $r$ to see that $r^{n-1}P=P$, and thus $rP\cdot r^{n-2}P=P$, making $rP$ a unit in $R/P$. Thus $R/P$ is a field, making $P$ maximal in $R$. 
***
#qual