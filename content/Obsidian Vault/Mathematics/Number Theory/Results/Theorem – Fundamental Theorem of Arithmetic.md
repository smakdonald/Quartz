#### $\thm$ – Fundamental Theorem of Arithmetic
Every non-zero [[Integers|integer]] $n \in\Z$ can be written in the form $n = up_{1} p_{2} \dots  p_{k}$ , where $k$ is a non-negative integer, $u$ is a [[Unit|unit]] of $\Z$, and each $p_{k}$ is a [[Prime|prime]] of $\Z$; moreover, this form is unique up to reordering and [[Associates|associates]]. Note that the $k = 0$ case corresponds precisely to the units.

##### *Proof.*
Let n be a non-zero integer. First, let’s dispense with the case that n is a unit  
(i.e., n = \pm1). In this case, n = n is an expression for n in the form n = up1 p2 \dots  p k ,  
where k = 0.  
Notice that any non-zero integer n has a unique prime factorization up to re-  
ordering and associates if and only if -n does, so for the remainder of the proof,  
we consider the case n is positive, assume u = 1, and suppose that any prime p  
appearing in the factorization is positive. We break the proof into the existence and  
uniqueness of a factorization for such an integer.  
First, we argue existence by strong induction. If n = 2, then n is prime, and  
taking u = 1, k = 1, p1 = 2 provides a prime factorization. Now suppose t can  
be written as a product of primes for all natural numbers 2 \leq  t < n, and consider  
n itself. If n is prime we are done. If not, n = ab for some 2 \leq  a, b < n in N.  
By our strong induction hypothesis, a and b can each be expressed as a product of  
primes, a = p1 p2 \cdots  pl and b = q1q2 \cdots  q m . Thus, n = p1 p2 \cdots  pl q1q2 \cdots  q m is  
an expression for n as a product of primes.  
It remains to prove uniqueness. We show that any time we have two prime fac-  
torizations of an integer n \geq  2 into a product of positive primes, then those two  
products are in fact simply rearrangements of one another. That is, suppose that, for some positive primes pi and qi , we have  
p1 \cdots  p k = q1 \cdots  q .  
After canceling off any factors in common to both sides, we can assume that no  
pi is equal to any q j . Now pick any prime pi you want. The equality of the two  
products implies pi | q1 \cdots  q. Thus, by Corollary 3.3.9, we have pi | q j for some  
j. However, the only divisors of q j are \pm1 and \pmq j , and we reach the contradiction  
pi = q j for some j.