#### $\lem$ – Square Roots in 2-Adic Integers
Let $\beta \in\Z^{\times}_{2}$. Then $\beta$ has a square root in $\Z_{2}$ iff $\beta \equiv 1 \mod 8$

##### *Proof.*
First, suppose \a 2 = \beta in Z2. Then since \beta \in\Z\times 
2, we know \beta \mod 2 = 1, 
and so \a \mod 2 = 1 as well. This forces \a \mod 8 \in {1, 3, 5, 7}, and for any of these 
choices we get \beta \equiv \a 2 \equiv 1 \mod 8. 
Conversely, suppose \beta \equiv 1 \mod 8. We proceed as in the proof of Hensel’s Lemma, 
inductively computing more and more coefficients of the 2-adic expansion of a square 
root. We will show that we can construct the sequence of coefficients a n \in {0, 1} 
so that \a n = a0 + \cdots + a n-1 p n-1 satisfies \a 2 
n \equiv \beta \mod 2n+1 for5 all n \geq 1. The 
base case of n = 1 is handled by \a 1 = 1, since then both \a 2 and \beta are congruent 
to 1 \mod 2 1+1. Suppose for the sake of induction that we have found \a n so that 
\a 2 
n \equiv \beta \mod 2n+1 and so \a 2 
n - \beta = cn 2n+1 for some cn \in\Z2. We wish to choose 
a n so that \a n+1 = \a n + a n 2n gives the next correct coefficient of \beta when squared:
\a 2 
n+1 \equiv \beta \mod 2n+2. We compute 
\a 2 
n+1 - \beta = \a 2 
n + 2\a n a n 2n + a^{2} 
n 2 2n - \beta 
\equiv \a 2 
n - \beta + a n \a n 2n+1 
\equiv 2n+1 (c n + a n \a n ) (\mod 2n+2) 
For this to be zero, it suffices for the parenthetical to be even, which is equivalent to 
simply choosing a n = c n \mod 2 since \a n \equiv \a 1 \equiv 1 \mod 2.