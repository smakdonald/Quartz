#### $\lem$ – Valuations and Base Expansions
For a positive prime $p$, the $p$-adic valuation $v_{p}(n)$ of a natural number $n$ is both:
- The largest power $k$ of $p$ such that $p^{k} | n$
- The smallest power $k$ of $p$ that appears in the base $p$ expansion of $n$.

##### *Proof.*
The first of these bullets is the definition of v_{p}(n), so we need to show that 
the two conditions are equivalent. Given p and n as in the definition, let k be the 
smallest power appearing in the base p expansion of n, so that 
n = a k p k + a k+1 p k+1 + \cdots + a m p m = p k ( 
a k + a k+1 p + \cdots + a m p m-k ) 
with a k  = 0. This immediately shows that p k | n. Further, p k+1  n, as n 
p k \mod p = 
a k  = 0. We conclude that k = v_{p}(n).