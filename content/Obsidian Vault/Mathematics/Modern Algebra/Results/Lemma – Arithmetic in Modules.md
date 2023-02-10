#### $\lem$ – Arithmetic in Modules
Let $R$ be a [[Ring|ring]] and let $M$ be a (left) $R$-[[Module|module]]. Then for all $r \in R$ and $m \in M$ we have
1.  $0_Rm = 0_M$,
2. $r 0_M = 0_M$, 
3. $(-1_R)m = -m$, and
4. $(-r)m = -(rm)$ .
###### *Proof.*  
1.  For the first, $0m = (0+0)m = 0m + 0m$ and hence $0m = 0$.
2. For the second, $0_Rm = (0_R + 0_R)m = 0_Rm + 0_Rm$ and hence $0_Rm = 0_M$ since $M$ is an [[Abelian Group|abelian]] [[Group|group]]. 
3. For the third, $m + (-1)m = 1 m + (-1)m = (1 + (-1))m = (1 - 1)m = 0_Rm = 0_M$ (using the second) and hence $(-1)m$ is the additive inverse of $m$. 
4. Finally, $(-r)m = ((-1)r)(m) = (-1)(rm) = -(rm)$ (using the fact that $(-1)r = -r$ holds in any ring and the previous result).  
***