#### $\prop$ – GCDs and Units in PIDs
If $R$ is a [[Principal Ideal Domain|PID]] and $a,b\in R$, then 
1. $(a,b)=(g)$[^1] for some $g\in R$ and any such $g$ is a [[GCD|gcd]] of $a$ and $b$
2. the gcd of $a$ and $b$ is unique up to multiplication by a [[Unit|unit]].

###### *Proof.* 
1. The existence of $g$ is granted by definition in a PID. Now $a,b\in (g)$ gives that $g\mid a$ and $g\mid b$. If $g'\mid a$ and $g'\mid b$ we have that $a,b\in (g')$, so $(g)=(a,b)\subseteq (g')$ by minimality. This gives $g\in(g')$, hence $g'\mid g$.
***

[^1]: See: [[Ideal]], [[Generator]]