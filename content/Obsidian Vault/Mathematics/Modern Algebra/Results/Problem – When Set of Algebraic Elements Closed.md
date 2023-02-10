### Problem 7 – When Set of Algebraic Elements Closed
Let $L/F$ be a [[Field Extension|field extension]] and let $K := \{a\in L | a \text{ is algebraic over }F \}$[^1]. Show that if $L$ is [[Algebraically Closed|algebraically closed]], then K is algebraically closed.

##### *Proof.*
Let $L/F$ be a field extension let $K := \{a\in L | a \text{ is algebraic over }F \}$, and suppose that $L$ is algebraically closed. Thus every polynomial in $L[x]$ has a root in $L$.

Let $f\in K[x]$ and let $\a$ be a root of $f$. Thus $f=a_nx^n + \cdots + a_1 x + a_0$, where each $a_i\in K$. By definition of $K$, each $a_i$ is algebraic over $F$. Notice that $f\in F(a_0,\dots,a_n)[x]$ as well, making $\a$ algebraic over this extension as well. 

Consider the chain of extensions $$F \subseteq F(a_0) \subseteq F(a_0,a_1) \subseteq \cdots \subseteq F(a_0, a_1, \dots, a_{n-1} )\subseteq F(a_0, \dots, a_{n}, \a).$$As $a_i$ is algebraic over $F$ for all $i$ and $\a$ is algebraic over $F(a_0,\dots,a_n)[x]$ we see that each step in this chain has finite degree by Theorem. By the Degree Formula, $[F(a_0, \dots, a_{n}, \a): F]$ is finite and thus so is $[F(\a):F]$. By the Theorem again, $\a$ is algebraic over $F$. Thus $\a$ is algebraic over $F$, hence $\a\in K$, making $K$ algebraically closed.
***
#qual

[^1]: Notation: [[Algebraic Element]]