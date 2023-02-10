#### $\thm$ – Decimal Expansions and $\Z/(n)$
Let $n \in\N$[^1] with $\gcd(n, 10) = 1$[^2]. Then the period length of the decimal expansion of $\frac{1}{n}$ is precisely the [[Order|order]] of $[10]$ in $\Z/(n)^\times$[^3].

##### *Proof.*
We leave it to the reader to argue that if \gcd(n,10)=1, then there is no pre-periodic part of the decimal expansion of 1/n. So write 1  
n = 0.a1...a k , where k is  
the period length, so that 10k (1/n) = a1...a k .a1...a k and thus (10k - 1)(1/n) =  
a1...a k \in\Z. This shows that n divides 10k - 1, so 10k \equiv 1 (\mod n). As k is the least power of 10 for which (10k - 1)/n would be an integer, it is precisely the order  
of 10 \mod n.

[^1]: Notation: [[Mathematics/Number Theory/Definitions/Natural Numbers]]
[^2]: Notation: [[GCD]]
[^3]: Notation: [[Z(n)]], [[Group of Units]]