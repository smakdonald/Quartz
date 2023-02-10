#### $\cor$ – GCD and Coefficients
For every [[Integers|integer]] $k > 0, \gcd(ka, kb) = k \gcd(a, b)$[^1].

##### *Proof.*
The proof follows directly from the Euclidean Algorithm. Given for each  
i > 0, r i-1 = r i qi+1 + r i+1 , it follows that kr i-1 = kr i qi+1 + kr i+1 . Thus,  
\gcd(ka, kb) = \gcd(kb, kr1) = \cdots  = \gcd(kr n-1, 0) = kr n-1 = k \gcd(a, b),  
as desired.

[^1]: Notation: [[GCD]]