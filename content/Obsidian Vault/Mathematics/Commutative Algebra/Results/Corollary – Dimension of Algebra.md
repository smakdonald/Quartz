#### $\cor$ – Dimension of Algebra
If $R$ is a $k$-[[Algebra|algebra]], the dimension of $R$ is less than or equal to the minimal size of an algebra generating set for $R$ over $k$. If $R = k[f_1, \ldots, f_d]$ and $\dim(R) = d$, then $R$ is isomorphic to a polynomial ring over $k$, and the generators $f_i$ are algebraically independent.

##### *Proof.*
The first statement is trivial unless $R$ is finitely generated, in which case we can write $R=k[f_1,\dots,f_s] \cong k[x_1,\dots,x_s]/I$ for some ideal $I$, so $$\dim(R) \leqslant \dim(k[x_1,\dots,x_s]) = d.$$ Suppose we chose $s$ to be minimal. If $I\neq 0$, then $\dim(R)< s$, since the zero ideal is not contained in $I$.