#### $\thm$ – Lagrange’s Lemma
For every prime $p \equiv 1 \mod 4$, there exists an $m \in\Z$ such that $p | m^{2} + 1$.

##### *Proof.*
We write p = 4k+1 and then apply Wilson’s Theorem 
to get 
-1 \equiv 1 \cdot 2 \cdots 4k (\mod p) 
\equiv (1 \cdot 2 \cdots 2k) \cdot ((-2k) \cdots (-2) \cdot (-1)) (\mod p) 
= (1 \cdot 2 \cdots 2k)2 \cdot (-1)2k (\mod p) 
\equiv ((2k)!)2 (\mod p). 
Setting m = (2k)!, we have m2 \equiv -1 (\mod p) and so p | m2 + 1.