### Problem 9 – Annihilator Ideal and Quotient Field
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]], and set $I = \{r ∈ R | rn = 0 \text{ for some integer } n\}$.  
Prove that following assertions.

(a) $I$ is an [[Ideal|ideal]] in $R$
(b) If $R/I$[^1] is a [[Field|field]], then each element of $R$ is either a [[Unit|unit]] or in $I$.

##### *Proof.*
###### Part (a) 
Let $x,y\in I$. Thus there exists integers $n,m$ such that $xn=0=ym$. Consider $(xy)(nm)=(xn)(ym)=0$. Thus $xy\in I$. Additionally, $x+y(mn)=xmn+ymn=0+0=0$, and so $x+y\in I$ as well.

We now consider $I$ as an additive group. Notice that $0n=0$ and thus the identity is in there. Let $x\in I$. We examine $x\inv$. Since $xn=0$ we have $(xn)\inv=0$ and so $x\inv n\inv=0$. So $x\inv\in I$. Perfect. We have ourselves a subring.
***
###### Part (b) 
Suppose now that $R/I$ is a field. Luckily for us, this makes $I$ a maximal ideal. 

Let $r\in R$. If $r\in I$, great. Suppose its not. Then in $R/I$ $r$ is a unit, since we're in a field now. So $ru\in I$ for some $u\in R$. Thus $run=0$ for some $n\in\Z$. Since $ru\in I$ and $I$ a maximal and thus prime ideal, we have $u\in I$ or $r\in I$, a contradiction. 
***
#qual

[^1]: Notation: [[Quotient Ring]]