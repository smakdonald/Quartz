#### $\thm$ – Bézout's Identity (ED)
Suppose $R$ is a Euclidean domain with Euclidean norm $N$. Let $a, b \in R$ not 
both be zero, and let $g$ be any $\gcd$ of $a$ and $b$. Then there exist $m, n \in R$ such 
that $$am + bn = g.$$
##### *Proof.*
This is trivial if a is a unit, since then a(a-1g) + b(0) = g, so assume without 
loss of generality that a is not a unit. Then N (a) > 0 by the lemma, and we mimic 
prior proofs of Bézout’s Identity: let S = {as + bt : s, t \in\R and N (as + bt) > 0}, 
and let c = as + bt \in S be any element of least norm (since a = a(1) + b(0) \in S, 
S is non-empty). We will show c | g, which is enough to imply g also lies in S. 
By the Division Algorithm, we can write a = qc + r with either r = 0 or 
N (r ) < N (c). But since 
r = a - qc = a - q(as + bt) = a(1 - qs) + b(-qt) 
is a linear combination of a and b, r \in S unless r = 0; thus we cannot have 
N (r ) < N (c) by minimality of N (c). Hence r = 0 and so c | a. The analogous 
argument proves that c | b. 
Now write g = cq + r for some q, r \in\R with r = 0 or N (r ) < N (c). Then 
r = g - cq = g - (as + bt)q, and since g divides g, a, and b, g | r as well, which 
in turn implies N (g) \leq N (r ). But N (r ) < N (c) \leq N (g) since g is a \gcd of a and 
b, so we have a contradiction unless r = 0. Therefore, c | g, as desired.