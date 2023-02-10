#### $\thm$ – Principal Counting Mechanism
For a [[natural number|natural number]] $n$, we have[^1]
$$\sum_{d|n}\varphi(d) = n,  $$
where the sum runs over all [[Divides|divisors]] $d$ of $n$.

##### *Proof.*
We partition the integers from 1 to n into sets Sd defined, for each d | n, by k \in  
Sd if and only if \gcd(k, n) = d. Then since \gcd(k, n) = d ⇐⇒ \gcd(k/d, n/d)=1,  
we see that Sd has the same number of elements as integers up to n  
d that are relatively  
prime to n  
d , that is, |Sd | = \varphi(n/d). Since the sets Sd partition {1, \dots  , n}, the union of the Sd contains exactly n elements, so  
n = \sum   
d|n  
\varphi  
( n  
d  
)  
= \sum   
d|n  
\varphi(d),  
the last equality following since n  
d runs through all divisors of n as d does.

[^1]: Notation: [[Euler's Totient Function]]