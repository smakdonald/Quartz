#### $\lem$ – Reduction Lemma
For all $a, b \in\N$[^1], we have[^2]
$$\gcd(a, b) = \gcd(b, a \mod b).$$

##### *Proof.*
Let a and b be arbitrary natural numbers and let a = r \mod b, so a = qb + r  
for some q \in\Z. By the Linear Combination Lemma (3.2.4), any common divisor of a and b is also a common divisor of a and a - bq = r . Similarly, any divisor of  
b and r is also a common divisor of b and a = bq + r . Thus, since the finite set of  
common divisors of a and b is equal to the finite set of common divisors of b and  
r = a \mod b, the greatest elements of the two sets must be equal.

[^1]: Notation: [[Mathematics/Number Theory/Definitions/Natural Numbers]]
[^2]: Notation: [[GCD]], [[Mod]]