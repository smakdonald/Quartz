### Problem 4 – Prime in UFD, $\Z[\sqrt{-5}]$ not UFD

(a) Prove that in a [[Unique Factorization Domain|UFD]] an element $p$ is [[Irreducible|irreducible]] if and only if the [[Ideal|ideal]] $(p)$[^1] is prime.
(b) Prove that $\Z[\sqrt{-5}]$ is not a UFD.

##### *Proof.*
###### Part (a) 
Let $R$ be a UFD. 

First, suppose $p$ is irreducible, and consider the ideal $(p)$. Let $a,b\in R$ such that $ab\in(p)$. 
Thus $p|ab$, so there exists some $k\in R$ such that $pk=ab$. As we are in a UFD the elements $a,b,$ and $k$ all have unique (up to associates) factorizations of irreducible elements. Thus $p$ must be an associate of one of the irreducible elements in the factorization of $a$ or $b$, and so $a\in(p)$ or $b\in(p)$,  making $(p)$ prime.

Now suppose that $(p)$ is prime and that $p=ab$ for some $ab\in R$. Thus $p|ab$ and $ab\in(p)$, so either $a\in(p)$ or $b\in(p)$, as $(p)$ is a prime ideal. Assume without loss of generality that $a|p$. Thus $ak=p$ for some $k\in R$. Thus $ab=pkb$ and $p=pkb$ As UFDs are integral domains we see $kb=1$, making $b$ a unit. Thus $p$ is irreducible.
***
###### Part (b) 
First, notice that $2\cdot 3=6=(1+\sqrt{-5})(1-\sqrt{-5})$. 
Define a function $$N:\Z[\sqrt{-5}]\to\Z, N(a+b \sqrt{-5})=a^2+5b^2.$$
Let $\alpha,\beta\in\Z[\sqrt{-5}]$ and behold $$\begin{align}
N(\alpha\beta)
&=N((a+b \sqrt{-5})(c+d \sqrt{-5}))\\
&=N(ac-5bd+ad \sqrt{-5}+bc \sqrt{-5})\\
&=(ac-5bd)^2+5(ad+bc)^2\\
&=((ac)^2-10acbd+25(bd)^2)+5((ad)^2+2abcd+(bc^2))\\
&=a^2c^2+25b^2d^2+5a^2d^2+5b^2c^2\\
&=(a^2c^2+5a^2d^2)+(5b^2c^2+25b^2d^2)\\
&=a^2(c^2+5d^2)+5b^2(c^2+5d^2)\\
N(\alpha)N(\beta)&=(a^2+5b^2)(c^2+5d^2).\end{align}$$So there's that done.

Suppose by way of contradiction there exist $\a,\b$ such that $2=\a\b$. Then $\a=a+b\sqrt{-5}$ and $\b=c+d\sqrt{-5}$, and $$N(2)=4=N(\a\b)=N(\a)N(\b)=(a^2+5b^2)(c^2+5d^2).$$ Thus $(a^2+5b^2)=\pm1,\pm2,$ or $\pm4$, as these are the only integer divisors of $4$. However, there do not exist integers $a,b$ such that this is true. Thus $2$ is irreducible in $\Z[\sqrt{-5}]$. 

Suppose by way of contradiction that $2$ is prime in $\Z[\sqrt{-5}]$. Note that $2|6=(1+\sqrt{-5})(1-\sqrt{-5})$. Thus $2$ divides one of these factors.

First, suppose there exists some $a+b\sqrt{-5}$ such that $2(a+b\sqrt{-5})=(1\pm\sqrt{-5})$. Thus $2a+2b\sqrt{-5}=1\pm\sqrt{-5}$, and so $2a=\pm1$. However, $\pm\frac12$ is not an integer, and thus $2$ cannot divide either of these factors. Thus $2$ is not prime in $\Z[\sqrt{-5}]$. By Part (a), this is not a UFD.

#qual

[^1]: Notation: [[Principal Ideal]]