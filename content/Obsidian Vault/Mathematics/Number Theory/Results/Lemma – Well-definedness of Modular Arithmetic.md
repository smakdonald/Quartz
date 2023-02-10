#### $\lem$ – Well-definedness of Modular Arithmetic
Let $a, b, c, d$ be [[Integers|integers]]. If $a \equiv c (\mod n)$[^1] and $b \equiv d (\mod n)$, then $a +b \equiv c+  d (\mod n)$, and $ab \equiv cd (\mod n)$. Equivalently, in the language of [[Equivalence Class|equivalence classes]], if $[a] = [c]$ and $[b] = [d]$ in $\Z/(n)$, then $[a] + [b] = [c] + [d]$ and $[a] \cdot  [b] = [c] \cdot  [d]$.

##### *Proof.*
If a \equiv c (\mod n) and b \equiv d (\mod n), then n | (c - a) and n | (d - b), so  
n | (c - a) + (d - b) = (c + d) - (a + b),  
showing that a + b \equiv c + d (\mod n). Multiplication is similar (Exercise 4.30).

[^1]: Notation: [[Mod]]