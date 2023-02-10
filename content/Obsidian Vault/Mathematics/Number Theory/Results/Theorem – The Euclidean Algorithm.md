#### $\thm$ – The Euclidean Algorithm
For [[Mathematics/Number Theory/Definitions/Natural Numbers|natural numbers]] $a$ and $b$, let $r_{-1} = a, r_{0} = b$, and for $i \geq  0$ set $r_{i+1} = r_{i-1} \mod r_{i}$[^1]. Then for some $n \geq  1$, the process terminates with $r_{n} = 0$ and $r_{n-1} = \gcd(a, b)$[^2].

##### *Proof.*
To prove this process terminates, note that by the Division Algorithm we  
have 0 \leq  r i+1 < r i for each i \geq  0, and so the remainders form a strictly decreasing  
sequence of integers bounded below by 0:  
0 \leq  \cdots  < r i+1 < r i < \cdots  < r1 < r0.  
Thus, we must have that r n = 0 for some n, and we obtain  
\gcd(a, b) = \gcd(b, r1) = \gcd(r1, r2) = \cdots  = \gcd(r n-1, r n ) = \gcd(r n-1, 0),  
so \gcd(a, b) = r n-1.

[^1]: Notation: [[Mod]]
[^2]: Notation: [[GCD]]