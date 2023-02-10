#### $\thm$ – Finding Equivalent Matrices
Let $F$ be a [[Field|field]]. Given an $F$-[[Linear Transformation|linear transformation]] $g: V \to U$ between [[Dim (Vector Space)|finite dimensional]] $F$-[[Vector Space|vector spaces]] $V$ and $U$, there are [[Basis and Free Module|bases]] $B$ and $C$ of $V$ and $U$, respectively, such that[^1] $$[g]_B^C = 
\begin{bmatrix}
I_r & 0 \\
0 & 0 \\
\end{bmatrix}$$
where $r = \rank(g)$[^2] and the $0$'s denote appropriately sized matrices with all $0$ entries. 

###### *Proof.* 

We form $B$ and $C$ in steps.

Start by picking an ordered basis   $C' = \{w_1, \dots, w_r\}$ of the image of $g$. For each $i$ pick $v_i \in V$ such that $g(v_i) = w_i$ and set $B' = \{v_1, \dots, v_r\}$. Then pick a basis $B''$ of the kernel of $g$. Let us list the   elements of $B''$ as $\{v_{r+1}, \dots, v_n\}$. 

I claim that $B := B'  \cup B'' = \{v_1, \dots, v_n\}$ is a basis of $V$.  (Note that $B' \cap B'' = \emptyset$ since $g(v_i) = w_i \ne 0$ for all $i$ with $1 \leq i \leq r$ and $g(v_i) = 0$ for all $i > r$.) Pick $v \in V$. Then, since $C'$ spans the image of $g$, we have  $g(v) = \sum_{i=1}^r a_i w_i$ for some scalars $a_i \in F$.
It follows that $v - \sum_{i=1}^r a_i v_i \in \ker(g)$ and hence, since the [[Kernel|kernel]] is spanned by $B''$, 
we have$$v - \sum_{i=1}^r a_i v_i = \sum_{i=r+1}^n a_i v_i,$$for some $a_{r+1}, \dots, a_n \in F$. We rearranging this equation, we conclude $v \in \Span(B)$ and thus $B$ spans $V$.

Now say $\sum_{i=1}^n c_i v_i = 0$ for some $c_i$'s in $F$. Since $g(v_i) = 0$ for all $i > r$ and $g(v_i) = w_i$ for all $i \leq r$, this gives that $0 = g(0) = g(\sum_{i=1}^n c_i v_i) = \sum_{i=1}^n c_i g(v_i) =\sum_{i=1}^r c_i w_i = 0$. Since $C'$ is [[Linearly Independent|linearly independent]], we have $c_i = 0$ for $1 \leq i \leq r$. Going back to the original equation

$\sum_{i=1}^n c_i v_i = 0$, we see that $\sum_{i=1}^r c_i v_i = 0$ and hence $c_i=0$ for all $i$, since $B''$ is linearly independent.

Finally we extend $C'$ to an ordered basis $C = \{w_1, \dots, w_r, w_{r+1}, \dots, w_m\}$ of $W$ arbitrarily.

By our construction, for any $v_i \in B$ we have
  $$
  g(v_i) = \begin{cases}
    w_i & \text{for $1 \leq i \leq r$ and} \\
    0 & \text{for $r+1 \leq i \leq n$} \\
  \end{cases}
  $$
and hence
$$
[g]_B^C = 
\begin{bmatrix}
I_r & 0 \\
0 & 0 \\
\end{bmatrix}.
$$
Note that, in our construction, $r = \dim_F(\im(g)) = \rank(g)$.[^3]
***

[^1]: See: [[Homomorphism Matrix]]
[^2]: See: [[Dim (Vector Space)|Rank]]
[^3]: See: [[Dim (Vector Space)|Dimension]]