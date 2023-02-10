#### $\thm$ – Bézout’s Identity
Fix $a, b \in\Z$[^1] not both zero. Then there exist [[Integers|integers]] $x$ and $y$ such that $\gcd(a, b) = ax + by$[^2]; i.e., $\gcd(a, b)$ can be written as a [[Linear Combination|linear combination]] of $a$ and $b$.

##### *Proof.*
Without loss of generality, suppose a and b are integers with a  = 0. Let S be  
the set of positive linear combinations of a and b:  
S = {ax + by : x, y \in\Z and ax + by > 0}.  
Then S is non-empty as ax + b(0) \in S for x = +1 or x = -1. By the Well-Ordering  
Principle, since S is a non-empty subset of N, it has a smallest element d = ax + by  
for some x, y \in\Z. Let c be an arbitrary common divisor of a and b. By the Linear  
Combination Lemma, c | d.  
We employ a standard technique to show that d is a common divisor of a and b:  
we divide each by d and show that the remainders are 0. By the Division Algorithm,  
there exist integers q and r such that a = dq + r and 0 \leq  r < d. Since ax + by = d  
it follows that axq + byq = dq = a - r and r = a(1 - q x) + b(-qy) \geq  0. If  
r were positive, then it would be a positive linear combination of a and b less than  
d, contradicting our assumption that d was the least such linear combination. Thus,  
r = 0 and d | a. A similar argument shows d | b. Since d is a common divisor  
of a and b, and is itself divisible by every common divisor, it must be the greatest  
common divisor of a and b.

[^1]: Notation: [[Integers]]
[^2]: Notation: [[GCD]]