#### $\thm$ – Irreducible is Prime in PID
Let $R$ be a [[Integral Domain|domain]] and let $r\in R$. 
1. If $r$ is a [[Mathematics/Modern Algebra/Definitions/Prime|prime]] element, then $r$ is [[Irreducible|irreducible]]. 
2. If $R$ is a [[Principal Ideal Domain|PID]] and $r$ is irreducible, then $r$ is a prime element.

###### *Proof.* 
Suppose $R$ is an integral domain and that $r$ is prime. Then $r \ne 0$ and $r$ is not a unit. Suppose $r = yz$. Then $yz \in (r)$ and hence by definition either $y \in (r)$ or $z \in (r)$. If $y \in (r)$, we have $y = rt$ for some $t$ and so $y = yzt$. Since $r \ne 0$, $y \ne 0$, and $R$ is an integral domain, we must have $zt = 1$, showing that $z$ is a unit.

Assume $R$ is a PID and that $r$ is irreducible. Since $r$ is not a unit, $(r)$ is a proper ideal and hence is contained in a maximal ideal $M$ by Theorem \ref{thm:maxexists}. We show $(r)= M$ and hence $(r)$ is prime.
Since $R$ is a PID, $M = (y)$ for some $y$. So $x = yt$ for some $t$. But $x$ is irreducible and $y$ is not a unit, which forces $t$ to be a unit and hence $(x) = (y) = M$.
***