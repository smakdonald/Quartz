#### $\lem$ – Power Lemma
Let $a$ and $b$ be relatively prime [[Mathematics/Number Theory/Definitions/Natural Numbers|natural numbers]]. If $ab$ is a square, then $a$ and $b$ are themselves squares. More generally, if $ab$ is an $n\th$ power, then so are $a$ and $b$.

##### *Proof.*
Suppose ab = k2 with \gcd(a, b) = 1. Then for any prime p, v_{p}(a)+v_{p}(b) =  
vp(ab) = 2vp(k) is even, but either v_{p}(a) = 0 or v_{p}(b) = 0 since \gcd(a, b) = 1,  
so both must be even. That is, for each prime p, both v_{p}(a) and v_{p}(b) are even, so a  
and b are squares by Lemma 3.4.6. For the general argument, we need only replace  
“even” with “multiple of n.”