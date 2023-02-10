### Problem 4 – Irreducible but not Prime in $\Z[\sqrt{10}]$
Consider the [[Subring|subring]] $\Z[\sqrt{10}] = \{a + b\sqrt{10} | a, b \in \Z\}$ of $\R$. Show that $2$ is [[Irreducible|irreducible]] but not [[Mathematics/Modern Algebra/Definitions/Prime|prime]] in $\Z[\sqrt{10}].$ Hint: Consider the function $N : \Z[\sqrt{10}]\to \Z, N (a + b\sqrt{10}) = a^2-10b^2$.

##### *Proof.*
Consider $2\in\Z[\sqrt{10}]$ and  the function $N : \Z[\sqrt{10}]\to \Z, N (a + b\sqrt{10}) = a^2-10b^2$. 

Let $\alpha,\beta\in\Z[\sqrt{10}]$ and behold $$\begin{align}N(\alpha\beta)&=N((a+b\sqrt{10})(c+d\sqrt{10}))\\
&=N(ac+10bd+(ad+bc)(\sqrt{10}))\\
&=(ac+10bd)^2-10(ad+bc)^2\\
&=((ac)^2+20acbd+100(bd)^2)+(-10(ad)^2-20abcd-10(bc)^2)\\
&=a^2c^2+100b^2d^2-10a^2d^2-10b^2c^2\\
&=(a^2c^2-10a^2d^2)+(-10b^2c^2-100b^2d^2)\\
&=a^2(c^2-10d^2)-10b^2(c^2-10d^2)\\
N(\alpha)N(\beta)&=(a^2-10b^2)(c^2-10d^2).\end{align}$$
So there's that done.

Suppose by way of contradiction there exist $\a,\b$ such that $2=\a\b$. Then $\a=a+b\sqrt{10}$ and $\b=c+d\sqrt{10}$, and $$N(2)=4=N(\a\b)=N(\a)N(\b)=(a^2-10b^2)(c^2-10d^2).$$ Thus $(a^2-10b^2)=\pm1,\pm2,$ or $\pm4$, as these are the only integer divisors of $4$. However, there do not exist integers $a,b$ such that this is true. Thus $2$ is irreducible in $\Z[\sqrt{10}]$. 

Suppose by way of contradiction that $2$ is prime in $\Z[\sqrt{10}]$. Note that $2|6=(4+\sqrt{10})(4-\sqrt{10})$. Thus $2$ divides one of these factors.

First, suppose there exists some $a+b\sqrt{10}$ such that $2(a+b\sqrt{10})=(4\pm\sqrt{10})$. Thus $2a+2b\sqrt{10}=4\pm\sqrt{10}$, and so $2b=\pm1$. However, $\pm\frac12$ is not an integer, and thus $2$ cannot divide either of these factors. Thus $2$ is not prime in $\Z[\sqrt{10}]$. 

#qual