#### $\lem$ – GCD $\times$ LCM
For all [[Mathematics/Number Theory/Definitions/Natural Numbers|natural numbers]] $a$ and $b$, we have  $\gcd(a, b) \cdot  \lcm(a, b) = ab$[^1].

##### *Proof.*
By Lemma 3.4.4, we have  
vp(\gcd(a, b) \cdot  \lcm(a, b)) = min(v_{p}(a), v_{p}(b)) + max(v_{p}(a), v_{p}(b))  
= v_{p}(a) + v_{p}(b) = vp(ab)  
for all primes p, and so the result follows from Lemma 3.4.3.

[^1]: Notation: [[GCD]]