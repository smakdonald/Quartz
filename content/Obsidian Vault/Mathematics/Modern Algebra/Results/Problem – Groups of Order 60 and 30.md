### Problem 3 – Groups of Order 60 and 30
(a) Let G be a [[Simple Group|simple]] [[Group|group]] of [[Order|order]] 60. Determine the number of elements of G of order 5.
(b) Show that there is no simple group of order 30.

##### *Proof.*
###### Part (a)
Let $G$ be a simple group of order $60=2^2\cdot3\cdot 5.$ 
By Sylow's Theorem we know that $n_5|12$ and that $n_5\equiv 1\mod{5}$. Thus the options for $n_5$ are $1$ and $6$. Since $G$ is simple we see that $n_5=6$. As each Sylow $5$-subgroup of $G$ has $4$ unique elements of order $5$ and the identity we see that the number of elements or order $5$ in $G$ is $(5-1)\cdot 6=24$. 
***
###### Part (b)
Suppose by way of contradiction that $G$ is a simple group of order $30$. Similarly to above, $n_5=6$, yielding $24$ elements of order $5$. Now, $n_3|10$ and $n_3\equiv 1\mod{3}$, so $n_3=10$, yielding far too many elements to fit in $G$. 

#qual