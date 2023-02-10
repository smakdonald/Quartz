#### $\thm$ – The Fundamental Meta-Theorem of Arithmetic
A ring with a Division Algorithm has a Fundamental Theorem of Arithmetic.

##### *Proof.*



#### $\thm$ – The Fundamental Meta-Theorem of Arithmetic
Every Euclidean Domain is a Unique Factorization Domain.

##### *Proof.*
We prove existence and uniqueness of factorizations into 
irreducibles. For existence, note that any unit can be written in the desired form (using 
that unit and an empty product of irreducibles), and every unit has the same norm 
as 1. Now we proceed as in Z or \Z[i], by strong induction on the Euclidean norm: 
Fix n > N (1) and suppose each element of R with Euclidean norm less than n is expressible as a product of irreducible elements. Now suppose d \in\R has Euclidean 
norm N (d) = n. We need to show that d can be written as a product of irreducible 
elements. If d is irreducible, then we are done. Else, d = ab with neither a nor b 
a unit. By Lemma 6.5.5, we have N (a) < n and N (b) < n, so by the induction 
hypothesis, both a and b can be written as products of irreducibles. Multiplying these 
products together shows that d can be so written as well. 
For uniqueness, we proceed identically to Theorem 5.5.9. Suppose 
a1 \cdots a k = d = b1 \cdots b 
are two factorizations of an element of d into irreducibles a1, \dots a k and b1, \dots, b. 
Since R is a Euclidean Domain, the Prime Divisor Property (Theorem 6.4.12) tells 
us that each of the ai and b j is also a prime element. Since each ai divides the product 
b1 \cdots b, we must have ai | b j for some j, and since b j is irreducible, it must be that 
ai and b j are associates. This shows that, up to associates, the irreducibles in each 
of the two factorizations are the same.