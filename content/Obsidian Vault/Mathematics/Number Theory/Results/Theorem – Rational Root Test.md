#### $\thm$ – Rational Root Test
If $f (x) = a_{n}x^{n} + a_{n-1}x^{n-1} + \cdots+a_{0}$ has a [[Rational Numbers|rational]] root $x = \frac{b}{c}$ , with  $\gcd(b, c) = 1$[^1], then $b | a_{0}$ and $c | a_{n}$.

##### *Proof.*
Suppose x = b  
c , with \gcd(b, c) = 1, is a rational root of f (x). Then the  
equation f ( b  
c  
) = 0 gives, after multiplying by c n , that  
a n b n + a n-1b n-1c + \cdots  + a0c n = 0.  
Organizing this equation as  
-a0c n = b(a n b n-1 + \cdots  + a1c n-1),
we see that b | a0 (since \gcd(b, c) = 1 implies \gcd(b, c n ) = 1). Similarly, organizing  
the equation as  
a n b n = -c(a n-1b n-1 + \cdots  + a0c n-1),  
we see that c | a n .

[^1]: Notation: [[GCD]]