### Problem 8 – Algebraic Elements Closed
Let $F \sse L$ be a [[Field Extension|field extension]] with $L$ [[Algebraically Closed|algebraically closed]]. Consider the set
$$K = \{\a\in L : f (α) = 0 \text{ for some monic polynomial }f (x) \in F [x]\}.$$(a) Show that $K$ is a [[Field|field]].
(b) Show that $K$ is algebraically closed.

##### *Proof*.
###### Part (a) 
Let $a,b\in K$. Notice that $a\inv, ab,$ and $a+b$ are contained in $F(a,b)$. As $b\in K$, there exists some polynomial with coefficients in $F$ such that $b$ is a root. However, this polynomial also lives in $F(a)$, so we have $[F(a,b):F(a)]$ algebraic. As $[F(a):F]$ is also algebraic, we have $F[a,b]$ algebraic as well, as it is a finite extension by the [[Proposition – The Degree Formula|Degree Formula]]. Thus $a+b, a\inv,$ and $ab$ are algebraic over $F$ as well, making $K$ a field. 
***
###### Part (b) 
Let $\a\in K$. Thus $\a$ is the root of a polynomial $f(x)=a_nx^n+\dots+a_0$, where $a_{i}\in F$. Notice that $f$ is a polynomial in $F(a_n,\dots,a_0)$ as well, and thus $\a$ is algebraic over this extension as well. Consider the chain of extensions $$F \subseteq F(a_0) \subseteq F(a_0,a_1) \subseteq \cdots \subseteq F(a_0, a_1, \dots, a_{n-1} )\subseteq F(a_0, \dots, a_{n}, \a).$$As $a_i$ is algebraic over $F$ for all $i$ and $\a$ is algebraic over $F(a_0,\dots,a_n)[x]$ we see that each step in this chain has finite degree by. By the Degree Formula, $[F(a_0, \dots, a_{n}, \a): F]$ is finite and thus so is $[F(\a):F]$. Thus $\a$ is algebraic over $F$, hence $\a\in K$, making $K$ algebraically closed.
***
#qual