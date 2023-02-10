#### $\thm$ – The Division Algorithm
Given [[Integers|integers]] $a$ and $b$ with $b > 0$, there exist unique integers $q$ and $r$ (the quotient and remainder, respectively) such that  $a = bq + r$ and $0 \leq  r < b$.

##### *Proof.*
Let a and b be integers with b > 0, and consider the set  
of non-negative integers  
S = {a - bq : q \in\Z and a - bq \geq  0}.  
We begin by observing that  
(i) S consists of non-negative integers (by the a - bq \geq  0 clause of its definition);  
and  
(ii) S is non-empty (since if a \geq  0, then a - b(0) = a \in S, and if a < 0, then  
a - b(a) = -a(b - 1) \in S).  
Since S is a non-empty set of non-negative integers, the Well-Ordering Principle thus  
tells us that there is a least element r of S. That is, r is the least non-negative integer  
of the form r = a - bq for some q \in\Z. Note that r < b since if r \geq  b, then r - b =  
a-b(q +1) is an element of S smaller than r , contradicting the fact that r was the least  
such number. This establishes the existence of the numbers q and r in the theorem.  
Finally, we check that r and q are unique. Suppose to the contrary that we simul-  
taneously had a = bq1 +r1 and a = bq2 +r2 , where q1, q2, r1, r2 are all integers and 0 \leq  r1, r2 < b. Without loss of generality, suppose r1 \leq  r2 . Thus 0 \leq  r2 - r1 < b.  
Substituting, we find 0 \leq  (a - bq2) - (a - bq1) = b(q1 - q2) < b, which implies  
0 \leq  q1 - q2 < 1 for integers q1 and q2 . Thus, q1 = q2 , and solving for r1 and r2  
gives that r1 = r2 .