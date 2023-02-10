#### $\lem$ – Primitive Roots and Quadratic Residues
Let $g$ be a primitive root$\mod p$. Then the non-zero quadratic residues$\mod p$ are 
precisely the even powers of $g$.

##### *Proof.*
We begin by observing that g itself is a non-square modulo p. Indeed, if g = 
h2, then by Fermat’s Little Theorem, 1 \equiv h p-1 \equiv g( p-1)/2 \mod p, contradicting 
the fact that g has order p - 1. Now, every a \in\Z/( p)\times can be written in the form 
g k for some 1 \leq k \leq p - 1. We show that a is a square if and only if k is even. First, 
if k = 2 is even, then a = g k = g2 = (g )2 is a square. Second, if k = 2 + 1 is 
odd and a = b^{2} were a square, then b^{2} \equiv (g )2 \cdot g, so g \equiv (bg- )2 is a square, a 
contradiction.