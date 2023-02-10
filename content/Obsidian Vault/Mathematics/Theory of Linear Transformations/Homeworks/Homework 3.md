#### Problem 3
Let $V$ be a vector space, and let $\v_{1}, \v_{2},\v_{3}\in V$.
(a) Suppose the vectors $\v_{1}-2\v_{2}+\v_{3},v_{1}+\v_{3},\v_{2}+\v_{3}$ span $V$. Show that the vectors $\v_{1}, \v_{2},\v_{3}$ span $V$.
(b) Suppose the vectors $\v_{1}, \v_{2},\v_{3}$ are linearly independent. Show that the vectors $\v_{1}-2\v_{2}+\v_{3},v_{1}+\v_{3},\v_{2}+\v_{3}$ are linearly independent.

##### *Proof.*
Let $V$ be a vector space, and let $\v_{1}, \v_{2},\v_{3}\in V$.
###### Part (a)
Suppose the vectors $\v_{1}-2\v_{2}+\v_{3},v_{1}+\v_{3},\v_{2}+\v_{3}$ span $V$. Thus any $x\in V$ can be written in the form $$\begin{align*}
x&=\l_{1}(\v_{1}-2\v_{2}+\v_{3})+\l_2(\v_{1}+\v_{3})+\l_{3}(\v_{2}+\v_{3})\\
&= \l_1\v_1-2\l\v_{2}+\l_{1}\v_{3}+\l_{2}\v_{1}+\l_{2}\v_{3}+\l_{3}\v_{2}+\l_{3}\v_{3}\\
&=(\l_{1}+\l_{2})\v_{1}+(-2\l_{2}+\l_{3})\v_{2}+(\l_{1}+\l_{2}+\l_{3})\v_{3},
\end{align*}$$and so $x$ can also be expressed as a linear combination of $\v_{1},\v_{2},\v_{3}$. Thus these vectors span $V$. 

###### Part (b)
Suppose the vectors $\v_{1}, \v_{2},\v_{3}$ are linearly independent. Consider $x=\l_{1}(\v_{1}-2\v_{2}+\v_{3})+\l_{2}(v_{1}+\v_{3})+\l_{3}(\v_{2}+\v_{3})$, and observe $$\begin{align*}
x&=(\l_{1}\v_{1}-2\l_{1}\v_{2}+\l_{1}\v_{3})+(\l_{2}\v_{1}+\l_{2}\v_{3})+(\l_{3}\v_{2}+\l_{3}\v_{3})\\
&=(\l_{1}+\l_{2})\v_{1}+(-2\l_{1}+\l_{3})\v_{2}+(\l_{1}+\l_{2}+\l_{3})\v_{3}.
\end{align*}$$As $\v_{1},\v_{2},\v_{3}$ are linearly independent, we have the following:
- $\l_{1}+\l_{2}=0$
- $-2\l_{1}+\l_{3}=0$
- $\l_{1}+\l_{2}+\l_{3}=0$
From the first and third equations we see $\l_{3}=0$, which gives us $\l_{1}=0$ from the middle equation. Thus $\l_{2}=0$ as well. Thus we have our linear independence.  

#### Problem 4
Let $U$ and $V$ be subspaces of a [[Vector Space|vector space]] $W$.
(a) Prove that $U\cap V$ is a subspace of $W$.
(b) Prove that $U+ V$ is a subspace of $W$.
(c) Prove by means of an explicit example that $U\cup V$ may not be a subspace of $W$. 
(d) Show that $U\cup V$ is a subspace of $W$ if and only if either $U\sse V$ or $V\sse U$. 

##### *Proof.*
Let $U$ and $V$ be subspaces of a vector space $W$.

###### Part (a)
First note $0\in U$ and $0\in V$, and so $0\in U\cap V$ as well.

Let $x,y\in U\cap V$ and $\l,\mu$ be scalars. As both $U,V$ are subspaces of $W$ and $x,y\in U,V$, we see $\l x+\mu y$ is contained in $U,V$ by the definition of a subspace. Thus $\l x+\mu y\in U\cap V$, completing the proof.

###### Part (b)
First note $0=0+0$ where the first $0\in U$ and the second $0\in V$. Thus $0\in U+V$. 

Let $x,y\in U+V$ and $\l,\mu$ be scalars. Thus $x=a+b$ and $y=c+d$, where $a,c\in U$ and $b,d\in V$. Consider $$\begin{align*}
\l x+\mu y&=\l a+\l b+\mu c+\mu d\\
&= \l a+\mu c +\l b+\mu d.
\end{align*}$$Since $U,V$ are subspaces, we see $\l a+\mu c\in U$ and $\l b+\mu d\in V$. Thus we have expressed $\l x+\mu y$ as a sum of an element in $U$ and an element in $V$. Thus we have our subspace. 

###### Part (c)
Define $$U=\{(x, y, z) \in \R^3 : x + y + z = 0 \}  \quad\text{and}\quad V=\{(x, y, z) \in \R^3 : 2x + y + z = 0 \}$$ over $\R$, both of which are subspaces of $\R^{3}$ by the last homework. Notice  $$(-2,1,1)+(-1,1,1)=(-3,1,1),$$where $(-2,1,1)\in U$ and $(-1,1,1)\in V$. However, $-3+1+1\neq 0$ and $-6+1+1\neq 0$. Thus $(-3,1,1)$ is not in $U\cup V$, meaning it cannot be a subspace of $W$. 

###### Part (d)
($\Longleftarrow$) Assume without loss of generality $U\sse V$. Then $U\cup V=V$, which is a subspace by supposition. 

($\Longrightarrow$) Suppose $U\cup V$ is a subspace. If $U=V$ then we're in good shape. Suppose by way of contradiction $v\in V\setminus U$ and  $u\in U\setminus V$. As $U\cup V$ is a subspace, $u+v\in U\cup V$. Assume without loss of generality $u+v\in U$. But since $U$ is a subspace there exists some $-u$ that we can add to find $v\in U$ after all, which is a problem. As no generality was removed we see that either all $u\in V$ or all $v\in U$, completing the proof.

#### Problem 5
Let $V$ be a vector space and let $v_1,\dots,\v_{n}\in V$. Show that the set $\{v_1,\dots,\v_{n+1}\}$ is linearly independent if and only if $\{v_1,\dots,\v_{n}\}$ is linearly independent and $v_{n+1}\not\in\Span(\{v_1,\dots,\v_{n}\}).$

##### *Proof.*
($\Longrightarrow$) Suppose $\{v_1,\dots,\v_{n+1}\}$ is linearly independent. By Part (a) of the Linear Independence Lemma we see $\{v_1,\dots,\v_{n}\}$ is linearly independent as well, given $\{v_1,\dots,\v_{n}\}\sse\{v_1,\dots,\v_{n+1}\}$. Suppose that $v_{n+1}\in\Span(\{v_1,\dots,\v_{n}\})$. Thus $\v_{n+1}=\l_{1}\v_{1}+\dots+\l_{n}\v_{n}$, with some $\l_i\neq0$. But then $0=\l_{1}\v_{1}+\dots+\l_{n}\v_{n}-\v_{n+1}$, contradicting the linear independence of $\{v_1,\dots,\v_{n+1}\}$. Thus $v_{n+1}\not\in\Span(\{v_1,\dots,\v_{n}\}),$ completing this direction of the proof.
($\Longleftarrow$) Suppose $\{v_1,\dots,\v_{n}\}$ is linearly independent and $v_{n+1}\not\in\Span(\{v_1,\dots,\v_{n}\}).$ Let $0=\l_{1}\v_{1}+\dots+\l_{n}\v_{n}+\l_{n+1}\v_{n+1}$. Suppose there exists some $\l_{i}\neq0$. But then $$\begin{align*}
0&=\l_{1}\v_{1}+\dots+\l_{n}\v_{n}\\
-\l_{n+1}\v_{n+1}&=\l_{1}\v_{1}+\dots+\l_{n}\v_{n}\\
\v_{n+1}&=\frac{-\l_{1}}{\l_{n+1}}\v_{1}+\dots+ \frac{-\l_{n}}{\l_{n+1}}\v_{n},
\end{align*}$$where $\frac{-\l_{i}}{\l_{n+1}}\neq0$. This would mean $\v_{n+1}\in\Span(\{v_1,\dots,\v_{n}\})$, which we said could not happen. Thus $\l_{i}=0$ for all $i$, making $\{v_1,\dots,\v_{n+1}\}$ is linearly independent.

#### Problem 6
Let $\F$ be a field. Fix $n\geq 0$ and let $V_{n}\sse\F[x]$ be the vector space of polynomials of degree $\leq n$. Show that if $p_{0},\dots,p_{n}\in\F[x]$ are polynomials with $\deg(f_{i})=i$, then they span $V_{n}$.

##### *Proof.*
Let $\F$ be a field. Fix $n\geq 0$ and let $V_{n}\sse\F[x]$ be the vector space of polynomials of degree $\leq n$. Suppose $p_{0},\dots,p_{n}\in\F[x]$ are polynomials with $\deg(p_{i})=i$. 

First, since $\F$ is a field and all elements of $\F$ are units we have $1=\l p_{0}$ for some $\l\in\F$. Note that by appropriate multiplication by inverses we can make each $p_{i}$ monic and by appropriate addition and subtraction we can remove all constant terms. Thus we can write $p_{1}=x$. Assume inductively $x^{k}$ can be generated by the $p_{i}$. Take $p_{k+1}$ and, using each lower power of $x$ and appropriate inverses in $\F$, we can remove all the terms of $p_{k+1}$ of degree less than $k+1$. As we already made $p_{k+1}$ monic, this leaves $x^{k+1}$. Thus the $p_i$'s generate the set $\{x,x^{2},\dots,x^{n}\}$. Thus any polynomial in $V_{n}$ can be written by multiplying $x^{i}$ be an appropriate coefficient in $\F$. Thus the $p_{i}$'s span $V_{n}$.