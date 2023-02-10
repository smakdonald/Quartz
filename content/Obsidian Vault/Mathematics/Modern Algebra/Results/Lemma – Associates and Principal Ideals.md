#### $\lem$ – Associates and Principal Ideals
Two elements $x,y$ of a [[Integral Domain|domain]] $R$ are [[Associates|associates]] if and only if $(x) = (y)$[^1].

###### *Proof.* 
If $(x) = (y)$ then $x \in (y)$ and so $x = yu$ for some $u$.  Similarly $y = xs$ and hence $y = yus$. Since $R$ is a domain, either $y = 0$ or  $su = 1$. If $y= 0$, then $x = 0 = 1 y$ and otherwise $u$ is a unit.

If $x = uy$ for a unit $u$, then $y = u^{-1}x$ and so
$x \in (y)$ and $y \in (x)$, from which is follows that $(x) \subseteq (y)$ and $(y) \subseteq (x)$.
***
[^1]: See: [[Generator]]