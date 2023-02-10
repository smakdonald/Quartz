#### $\thm$ – Prime iff Irreducible in UFD
An element of a UFD is prime if and only if it is irreducible.

##### *Proof.*
Since UFDs are integral domains, we already know that prime elements are 
irreducible, so it only remains to show that irreducible elements are also prime. 
Accordingly, assume that p is irreducible, and suppose that p | ab for some a, b \in\R. 
Then there exists some c \in\R such that pc = ab, and since R is a UFD, the elements 
a and b have unique factorizations into irreducible elements: say 
a = a1 \cdots a k and b = b1 \cdots b. 
Then pc = ab = a1 \cdots a k b1 \cdots b. Because p is irreducible and the factor- 
ization is unique, p (or an associate of p) must appear among the irreducibles 
a1, \dots, a k, b1, \dots, b. That is,  p = a j or  p = b j for some unit  and some 
j. Therefore, either p | a or p | b, so p is prime.