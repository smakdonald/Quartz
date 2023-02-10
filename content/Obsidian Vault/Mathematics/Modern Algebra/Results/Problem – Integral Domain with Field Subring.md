### Problem 4 – Integral Domain with Field Subring
(a) Suppose that $A$ is an [[Integral Domain|integral domain]] that contains a [[Field|field]] $F$ as a [[Subring|subring]], and that moreover $A$ is [[Dim (Vector Space)|finite dimensional]] as an $F$-[[Vector Space|vector space]]. Prove that $A$ is a field.
(b) Give an example to show that the finite dimension condition is necessary.

##### *Proof.*
###### Part (a)
Let $A$ be an integral domain that contains a field $F$ as a subring, and that moreover $A$ is finite dimensional as an $F$-vector space. 

Say 𝐴 has dimension $n$ over $K$. Let $x\in A,x\neq0$. Consider elements $1,x,x^2,x^{3,\dots,}$ which cannot be independent because of the finite dimension. So we may choose $m$ so that $1,x,\dots,x^m$ is linearly dependent over $K$ and  is as small as possible. This means that we may find $c_0,c_1,\dots,c^{m}\in K$, not all equal to $0$, such that $c_0+c_1x+\dots+c_mx^m=0$. Note that $c_0\neq0$, as this would contradict the minimality of $m$. Then $x(c_1+\dots+c)_mx^{m-1})$ is invertible, so 𝑥 is invertible as well, making $A$ a field.
***
###### Part (b)
Consider $\Q[x]$, which contains the subring $\Q$. However, this is not a finite dimensional vector space over $F$, and $\Q[x]$ is not a field, as $x$ has no inverse. 
***
#qual