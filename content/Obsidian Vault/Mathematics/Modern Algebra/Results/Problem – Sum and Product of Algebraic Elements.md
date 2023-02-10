### Problem 8 – Sum and Product of Algebraic Elements
Let $F\subseteq L$ be [[Field|fields]] and let $x, y \in L$ be [[Algebraic Element|algebraic]] elements over $F$. Prove that $x + y$ and $xy$ are also algebraic elements of $L$ over $F$.

##### *Proof.*
Let $F\subseteq L$ be fields and let $x, y \in L$ be algebraic elements over $F$ First, notice that $xy$ and $x+y$ are contained in $F(x,y)$. As $y$ is algebraic over $F$, it is the root of some polynomial $f$ with coefficients in $f$. But $f$ is also contained in $F(x)$, and thus the extension $[F(x,y):F(x)]$ is algebraic. As $[F(x):F]$ is algebraic as well, we see that $[F(x,y):F]$ is an algebraic extension of fields. Thus $xy$ and $x+y$ are algebraic over $F$.
***
#qual