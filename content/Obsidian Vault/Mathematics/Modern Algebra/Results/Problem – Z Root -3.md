### Problem 4 – $\Z\sqrt{-3}$
In the [[Commutative Ring|commutative]] [[Ring|ring]] $R = \Z[\sqrt{-3}]$, show that the element $2$ is [[Irreducible|irreducible]] but not [[Mathematics/Modern Algebra/Definitions/Prime|prime]].

##### *Proof.*
First, notice that $2\cdot 2=6=(1+\sqrt{-3})(1-\sqrt{-3})$. 
Define a function $$N:\Z[\sqrt{-3}]\to\Z, N(a+b \sqrt{-3})=a^2+3b^2.$$
Let $\alpha,\beta\in\Z[i]$ and behold $$\begin{align}
N(\alpha\beta)
&=N((a+b \sqrt{-3})(c+d \sqrt{-3}))\\
&=N(ac-3bd+ad \sqrt{-3}+bc \sqrt{-3})\\
&=(ac-3bd)^2+3(ad+bc)^2\\
&=((ac)^2-6acbd+9(bd)^2)+3((ad)^2+2abcd+(bc^2))\\
&=a^2c^2+9b^2d^2+3a^2d^2+3b^2c^2\\
&=(a^2c^2+3a^2d^2)+(3b^2c^2+9b^2d^2)\\
&=a^2(c^2+3d^2)+3b^2(c^2+3d^2)\\
N(\alpha)N(\beta)&=(a^2+3b^2)(c^2+3d^2).\end{align}$$So there's that done.

Suppose by way of contradiction there exist $\a,\b$ such that $2=\a\b$. Then $\a=a+b\sqrt{-3}$ and $\b=c+d\sqrt{-3}$, and $$N(2)=4=N(\a\b)=N(\a)N(\b)=(a^2+3b^2)(c^2+3d^2).$$ Thus $(a^2+3b^2)=\pm1,\pm2,$ or $\pm4$, as these are the only integer divisors of $4$. However, there do not exist integers $a,b$ such that this is true. Thus $2$ is irreducible in $\Z[\sqrt{-3}]$. 

Suppose by way of contradiction that $2$ is prime in $\Z[\sqrt{-3}]$. Note that $2|6=(1+\sqrt{-3})(1-\sqrt{-3})$. Thus $2$ divides one of these factors.

First, suppose there exists some $a+b\sqrt{-3}$ such that $2(a+b\sqrt{-3})=(1\pm\sqrt{-3})$. Thus $2a+2b\sqrt{-5}=1\pm\sqrt{-3}$, and so $2a=\pm1$. However, $\pm\frac12$ is not an integer, and thus $2$ cannot divide either of these factors. Thus $2$ is not prime in $\Z[\sqrt{-3}]$.
***
#qual