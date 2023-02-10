### Problem 1 – Normal p-Subgroup in Sylow Subgroups
Let $G$ be a [[Order|finite]] [[Group|group]], $p$ a prime dividing the order of $G$, and $H$ a [[Normal Subgroup|normal subgroup]] of order $p^m$ for some $m > 0$. Prove the following statements.

(a) $H$ is contained in every [[Sylow p-Subgroup|Sylow]] $p$-subgroup of $G$.
(b) $H$ contains a nontrivial [[Abelian Group|abelian]] [[Subgroup|subgroup]] that is normal in $G$.

##### *Proof.*
Let $G$ be a finite group, $p$ a prime dividing the order of $G$, and $H$ a normal  
subgroup of order $pm$ for some $m > 0$. 

###### Part (a)
As $H$ is normal we have $gHg\inv=H$ for all $g\in G$. As it is a $p$ group it is contained in some Sylow $p$-subgroup. All Sylow $p$-subgroups are conjugate to each other, but $H$ is fixed by conjugation so its actually in all of them.
***
###### Part (b)
Consider $Z(H)$, which is abelian in $H$. The center of $p$-groups are nontrivial so that's good. 
Let $g\in G$, $h\in Z(H)$, and consider $ghg\inv$. As $H\nsg G$ we know $ghg\inv\in H$. Let $h'\in H$. We see  $ghg\inv h'=ghh''g\inv$, since $H$ is still normal. $h\in Z(G)$ so we have $gh''hg\inv$. 

Notice that $h''g\inv=g\inv h'$, and thus $h'=gh''g\inv$. Thus $gh''=h'g$, and so we can substitute the last line in the previous paragraph to see $h'ghg'\inv$. Thus we have normality!
***
#qual