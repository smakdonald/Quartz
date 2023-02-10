#### $\thm$ – Sum of Two Integer Squares
An integer $n$ can be written as a sum of two integer squares if and only if $v_{p}(n)$ 
is even for every prime $p \equiv 3 \mod 4$.

##### *Proof.*
Write n = \prod 
i p ei 
i 
\prod 
j q f j 
j where the pi are the prime divisors of n congruent 
to 1 or 2 \mod 4, and the q j are 3 \mod 4. Then each pi and q2 
j is a norm of an element 
of \Z[i], and so if each f j is even, n is the norm of the product of those elements, 
and thus is itself a sum of two squares. For the reverse direction, we proceed nearly 
identically to the prime case: suppose n = a^{2} + b^{2} and that n has at least one prime 
divisor q \equiv 3 \mod 4 for which vq (n) is odd. If q divides both a and b, then an even 
power of q divides both sides of the equation n = a^{2} + b^{2}, and canceling as many 
powers from q as possible from both sides gives a new equation n = (a )2 + (b )2 
where q | n (since vq (n) was odd) but q  a, b. Reducing this equation \mod q 
gives 0 \equiv (a )2 + (b )2, so -1 \equiv (a /b )2 (\mod q). But -1 being a square modulo 
q contradicts that q \equiv 3 \mod 4.