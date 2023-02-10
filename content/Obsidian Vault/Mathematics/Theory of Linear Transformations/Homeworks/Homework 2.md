#### Problem 1
Let $V$ be a vector space over the field $\F$. Using only the axioms given in class for fields and vector spaces (no properties, lemmas, etc.) prove the following:

(a) for all $\v\in V$ we have $\v+(-1)\v=\0$.
(b) given any $\v\in V$ we have $-(-\v)=\v$.

#### Problem 2
For each of the following, sat whether it is a subspace of the indicated vector space (over the indicated field). For each example that is $not$ a subspace, give a proof of that fact. For at least one of the examples that $is$ a subspace prove that fact. 
(a) $\{(x, y, z) \in \R^3 : x + y + z = 1 \}$ over $\F^5$ 
(b) $\{p \in \R[x] : p'(1) = 0 \}$ over $\R$
(c) $\{f \in \R^\R : \exists c \in \R^+ \text{ such that } \forall x \in \R, \abs{f(x)} \leq c\abs{x} \}$
(d) $\{\v \in \R^3 : v_i \geq 0 \text{for} 1 \leq i \leq 3 \}$ over $\R$
(e) $\{f \in (\R^3)^* : f((1,3,-1)) = 0 \}$ over $\R$
(f) $\{f \in \Q^\Q : f \text{ is injective or } f = 0\}$ over $\Q$

##### *Proof:*
###### Part (a)
Let $V_{1}=\{(x, y, z) \in \R^3 : x + y + z = 1 \}$ over $\F^5$.
This is not a subspace as it would contradict Problem 4 (see proof below.)

###### Part (b)
Let $V_{2}=\{p \in \R[x] : p'(1) = 0 \}$ over $\R$.
Let $f,g\in V_{2}$ and $\l,\mu\in\R$. Observe $$(\l f+\mu g)'(1)=\l f'(1)+\mu g'(1)=\l(0)+\mu(0)=0,$$most of which comes from the properties of a derivative. Thus $V_{2}$ is indeed a subspace. Also the derivative of zero is zero so zero is in here. I forgot to show $0$ was in there for the rest, but since I only had to prove that one of these was a subspace I'm just not going to.

###### Part (c)
Let $V_{3}=\{f \in \R^\R : \exists c \in \R^+ \text{ such that } \forall x \in \R, \abs{f(x)} \leq c\abs{x} \}$.
Let $f,g\in V_{3}$ and $\l,\mu\in\R$. Thus there exists $d,e\in\R^{+}$ such that $|f(x)|\leq d|x|$ and $|g(x)|\leq e|x|$. Consider $c=de|\l\mu|$, and Observe $$|(\l f+\mu g)(x)|=|\l f(x)+\mu g(x)|\leq |\l f(x)|+|\mu g(x)|\leq d|\l x|+e|\mu x|\leq c|x|.$$Thus $V_{3}$ is indeed a subspace. 

###### Part (d)
Let $V_{4}=\{\v \in \R^3 : v_i \geq 0 \text{ for } 1 \leq i \leq 3 \}$ over $\R$.
Let $\v=(2,2,2)$, $\w=(1,1,1)$, $\l=-1$, and $\mu=1$. Thus $$\l\v+\mu\w=(-2,-2,-2)+(1,1,1)=(-1,-1,-1),$$which is not contained in $V_{4}$. Hence $V_{4}$ is not a subspace.

###### Part (e)
Let $V_{5}=\{f \in (\R^3)^* : f((1,3,-1)) = 0 \}$ over $\R$.

Let $f,g\in V_{5}$ and $\l,\mu\in\R$. Consider $\l f+\mu g$ and observe that for any $x,y\in\R^3$ and $\g\in\R$, we have $$\begin{align*}
(\l f+\mu g)(x+y)&=\l f(x+y)+\mu g(x+y)\\
&= \l (f(x)+f(y))+\mu (g(x)+g(y))\\
&= \l f(x)+\mu g(x)+\l f(x)+\mu g(x)\\
&= (\l f+\mu g)(x)+(\l f+\mu g)(y)
\end{align*}$$and $$\begin{align*}
\g(f+g)(x)&=\g((f(x)+g(x))\\
&= \g f(x)+\g g(x)\\
&= f(\g x)+g(\g x)\\
&= (f+g)(\g x),
\end{align*}$$making $f+g$ indeed a linear map. Now all that remains is to see $(f+g)(1,3,-1)=0$. Once more unto the breach: $$\begin{align*}
(f+g)(1,3,-1)&=f((1,3,-1))+g((1,3,-1))\\
&= 0+0\\
&= 0,
\end{align*}$$given that $f,g\in V_{5}$. Thus this is indeed a subspace. 

###### Part (f)
Let $V_{6}=\{f \in \Q^\Q : f \text{ is injective or } f = 0\}$ over $\Q$.
Let $f,g\in V_{6}$ and $\l,\mu\in\Q$. Suppose $(\l f+\mu g)(x)=(\l f+\mu g)(y)$ for some $x,y\in\Q.$ Then $\l f(x)+\mu g(x)=\l f(y)+\mu g(y)$.

$f=x^3$ and $g(x)=-x$, both of which have inverses and are thus in $V_{6}$. However $(f+g)(x)=x^{3}-x$ has three zeros, making it not longer injective. Thus we have a problem. :(

#### Problem 3
For each of the following say whether it is a linear map. In each case prove your answer.
(a) $N:\R^{3}\to\R$, $\v\to\v\cdot\v$
(b) $E_{3}:\F_{7}[X]\to\F_{7}$, $p\to p(3)$

##### *Proof.*
###### Part (a)
Let $\u=(2,2,2),\v=(3,3,3)\in\R^{3}$. Observe $$\begin{align*}
N(\u+\v)&=(\u+\v)\cdot(\u+\v)\\
&=((2,2,2)+(3,3,3))\cdot((2,2,2)+(3,3,3))\\
&=(5,5,5)\cdot(5,5,5)\\
&=75,
\end{align*}$$where as $$\begin{align*}
N(\u)+N(\v)&=N(3,3,3)+N(2,2,2)\\
&=((3,3,3)\cdot(3,3,3))+((2,2,2)\cdot(2,2,2))\\
&=27+12\\
&= 39.
\end{align*}$$As these are not equal, we see that $N$ is not a linear map, given that there exist $\u,\v\in\R^{3}$ such that $N(\u+\v)\neq N(\u)+N(\v)$. 

###### Part (b) 
Let $p,q\in\F_{7}[X]$ and $\l\in\F_{7}.$ Thus $$E_{3}(p+q)=(p+q)(3)=p(3)+q(3)=E_{3}(p)+E_{3}(q).$$This is basically just properties of functions and how the addition of functions is defined. Let me know if more justification is needed!

Now consider $E_{3}(\l p)=\l p(3)=\l E_{3}(p)$. Thus $E_{3}$ is indeed a linear map.

#### Problem 4
Let $a,b,c\in\F$ be scalars, not all zero. Let $d\in \F$ and consider the subset of $\F^{3}$ $$V=\{(x,y,z)\in\F^{3}|ax+by+cz=d\}$$Prove that $V$ is a subspace of $\F^{3}$ if and only if $d=0$.

##### *Proof.*
First, suppose that $V$ is indeed a subspace of $\F^{3}$. Then $V$ contains the additive identity element $(0,0,0)$. We know that this is the additive identity as $(x,y,z)+(0,0,0)=(x,y,z)$ for any vector $(x,y,z)\in V$. Let $a,b,c\in\F$ as given.. As $(0,0,0)\in V$ we see $a(0)+b(0)+c(0)=d$, and thus $d=0$. 

Now suppose $d=0$. Let $(x,y,z),(u,v,w)\in V$ and $\l,\mu\in\F$. Consider $$\begin{align*}
\l(x,y,z)+\mu(u,v,w)&=(\l x,\l y,\l z)+(\mu u, \mu v, \mu w)\\
&= (\l x+\mu u, \l y+\mu v,\l z+\mu w)
\end{align*}$$and observe $$\begin{align*}
a(\l x+\mu u)+b(\l y+\mu v)+c(\l z+\mu w)&=(a\l x+a\mu u)+(b\l y+b\mu v)+(c\l z+c\mu w)\\
&= \l ax+\mu au+\l by+\mu bv+\l cz+\mu cw\\
&= \l(ax+by+cz)+\mu(au+bv+cw)\\
&= \l(d)+\mu(d)\\
&= 0,
\end{align*}$$placing $\l(x,y,z)+\mu(u,v,w)\in V$. Thus $V$ is indeed a subspace of $\F^{3}$.

#### Problem 5
A function $f:\R\to\R$ is periodic if there is a positive real number $p$ such that $f(x+p)=f(x)$ for all $x\in\R$. Two real numbers are *commensurable* if their ratio is a rational number. Fix a positive real number $p$, and consider the following three subsets of $\R^{\R}$:
(a) $V_{1}=\{f:\R\to\R|f\text{ is periodic of period }p\}$
(b) $V_{2}=\{f:\R\to\R|f\text{ is periodic, with period commensurable with }p\}$
(c) $V_{3}=\{f:\R\to\R|f\text{ is periodic of some period}\}$
Determine, with proof, which of these sets are subspaces of $\R^{\R}.$

##### *Proof.*
###### Part (a) 
Let $f,g\in V_{1}$ and $\l,\mu\in\R$. Observe $$\begin{align*}
(\l f+\mu g)(x+p)&= \l f(x+p)+\mu g(x+p)\\
&= \l f(x)+\mu g(x)\\
&= (\l f+\mu g)(x),
\end{align*}$$ making $V_{1}$ a subspace of $\R^{\R}$.

###### Part (b)
Let $f,g\in V_{3}$. As $f,g$ are periodic, there exist positive real numbers $q,r$ such that $f(x+q)=f(x)$ and $g(x+r)=g(x)$, where $\frac{p}{q}$ and $\frac{p}{r}$ are rational. First, note that if $p$ is irrational, then both $q$ and $r$ must be a scalar multiple of $p$. Let $s=pqr$. Thus $s$ is commensurate with $p$, and we have $$f(x+s)=f(x+q(pr))=f(x)\quad\text{and}\quad g(x+s)=g(x+r(pq))=g(x).$$The proof is now identical to that of Part (a).

Suppose then that $p\in\Q$. Let $s=qr$. Notice that $\frac{s}{p}=\frac{qr}{p}=\frac{q}{p}\cdot \frac{r}{p}$. As The product of rational numbers is rational, we see $s$ and $p$ are commensurable. Notice then $$f(x+s)=f(x+qr)=f(x) \quad\text{and}\quad g(x+s)=g(x+qr)=g(x).$$ The proof is now identical to that of Part (a), and so $V_{2}$ is indeed a subspace of $\R^{\R}$.

###### Part (c)
Let $f,g:\R\to\R$ be defined such that $$
f=\begin{cases}
1,\quad x\in[0,\frac{1}{2}) \\
2,\quad x\in(\frac{1}{2},1)
\end{cases}\quad\text{and}\quad g=\begin{cases}
10,\quad x\in[0,1] \\
20,\quad x\in(1,\sqrt{2}),
\end{cases}$$
where $f(x)=f(x+1)$ and $g(x)=g(x+\sqrt{2})$. Make them both even functions as well so the periodic-ness extends in the negative direction as well.

Suppose by way of contradiction that $f+g$ is periodic. Then there exists some $p\in\R$ such that $(f+g)(x+p)=(f+g)(x)$. Thus $$f(x+p)+g(x+p)=f(x)+g(x).$$ If $f(x)\neq f(x+p),$ assume without loss of generality that $f(x)=1$ and $f(x+p)=10$. Then we have $1+g(x)=10+g(x+p)$. But there are no values of $g$ that satisfy this equation, so we must have $f(x)=f(x+p)$. A similar argument shows $g(x)=g(x+p)$. As the smallest period of $f$ is $1$, this means that $p$ is a multiple of $1$, making $p$ an integer. However, $\sqrt{2}$ is the smallest period of $g$, and thus $p$ must be a multiple of $\sqrt{2}$, making $p$ both an integer and irrational, which is a contradiction. Thus $f+g$ is not periodic, and so $V_{3}$ cannot be a subspace of $\R^{\R}$.





