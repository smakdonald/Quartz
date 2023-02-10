#### $\cor$ – p-Adic Integers are a UFD
The ring $\Z_{p}$ is a unique factorization domain with $p$ its unique irreducible element (up to associates). Further, $\Q_{p}$ is a field, and equals the field of fractions of $p$-adic integers.

##### *Proof.*
First, since we have not made the point explicitly yet, note that Zp and Qp 
are both integral domains (neither the product of powers of p nor of two units can 
be zero) and Qp is further a field (\a -1 = p-vp (\a )u-1 ). The irreducibility of p in Zp 
follows from a valuation calculation: if p = \a \beta, then 
1 = vp( p) = vp(\a \beta ) = vp(\a ) + vp(\beta ), 
and since both vp(\a ) and vp(\beta ) are non-negative integers, one of them must be 0, 
making that factor a unit by Lemma 8.4.2. A similar argument shows p is also prime. 
This also gives unique factorization: if \a \in\Zp, then since \a = pvp (\a )u for some 
unit u, \a can be written as a product of irreducibles in Zp, and uniquely so since the 
valuation vp(\a ) is well-defined. Finally, 
Qp = 
{ \a 
\beta : \a, \beta \in\Zp, \beta  = 0 
} 
by mutual inclusion (Exercise 8.36).