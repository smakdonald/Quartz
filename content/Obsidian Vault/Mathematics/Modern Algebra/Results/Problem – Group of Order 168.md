### Problem 3 – Group of Order 168
Suppose $G$ is a [[Simple Group|simple]] [[Group|group]] of [[Order|order]] $168 = 2^3 · 3 · 7.$ (Yes, there is such a group.)
(a) How many elements of order $7$ does $G$ have?
(b) Show that $G$ has at least $14$ elements of order $3$

##### *Proof.*
###### Part (a)
By [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]], $|\Syl_7(G)|\equiv 1\mod{7}$ and divides $2^3\cdot 3=24$. Thus the only options are $1$ and $8$. However, as $G$ is simple there cannot be only one Sylow $7$-Subgroup, as it would be [[Normal Subgroup|normal]]. Thus there are $8$, each having $7$ unique elements and the identity. Thus there are $49$ elements of order $7$. 
***
###### Part (b)
By Sylow's Theorem, $|\Syl_3(G)|\equiv 1\mod{3}$ and divides $2^3\cdot 7=56$. As $G$ is simple there cannot be one, so there must be at least $7$, each with $2$ non-identity elements. Thus there must be at least $14$ elements of order $3$. 
***
#qual