#### $\lem$ – Diagonal Presentation
Suppose $R$ is a [[Commutative Ring|commutative]] [[Ring|ring]] and $A = (a_{i,j})$ is a $m \times n$ matrix such that $a_{i,j} = 0$ for all $i \ne j$ and set $d_i = a_{i,i}$ for all $1 \leq i \leq \min\{m,n\}$. If $n \geq m$ then 
$$\coker(T_A) \cong R/R \cdot d_1 \oplus R/R\cdot d_2 \oplus \cdots \oplus R/R \cdot d_m $$
  and if $n \leq m$ then$$\coker(T_A) \cong R/R \cdot d_1 \oplus R/R\cdot d_2 \oplus \cdots \oplus R/R \cdot d_n \oplus R^{m-n}.$$

###### *Proof.* 
Assume $n \leq m$ and define $g: R^m \to R/R \cdot d_1 \oplus R/R \cdot d_2 \oplus \cdots \oplus R/ R \cdot d_n \oplus R^{m-n}$ to be the map sending $(r_1, \dots, r_m)^\tau$ to $(\ov{r}_1, \dots, \ov{r}_n, r_{n+1}, \dots, r_m)$ where $\ov{r}_i = r_i + R \cdot d_i$ for $1 \leq i \leq n$.  (I.e., $g$ is the unique $R$-map sending the $i$-th standard basis vector $e_i$ to $(0, \dots, 0, \ov{1}, 0, \dots, 0)$ with $\ov{1}$ in the $i$-th position, for $1 \leq i \leq n$, and to $e_i$ itself for $i > n$.) Then $g$ is clearly onto and the kernel $\ker(g)$ of $g$ is the set of those tuples $(r_1, \dots, r_m)^\tau$ such that $r_i =  x_i d_i$ for some $x_i$ for all $1 \leq i \leq n$ and $r_j = 0$ for $j > n$.  
Given such a tuple, $$ (r_1, \dots, r_m)^\tau = x_1 (d_1, 0, \dots, 0)^\tau + x_2 (0,d_2, 0, \dots, 0)^\tau + \cdots + x_n (0, \dots, 0, d_n, 0, \dots, 0)^\tau. $$
This proves $\ker(g)$ is contained $$
R \cdots (d_1, 0, \dots, 0)^\tau + R \cdot (0,d_2, 0, \dots, 0)^\tau 
  + \cdots + R \cdot (0, \dots, 0, d_n, 0 \dots, 0)^\tau = \im(T_A).
  $$Arguing backwards we see that the opposite containment also holds, so that in fact $\ker(g) = \im(T_A)$. 
  
By the First Isomorphism Theorem, $$ \coker(T_A) = R/\im(T_A) = R/\ker(g) \cong R/R \cdot d_1 \oplus \cdots \oplus R/R \cdot d_n \oplus R^{m-n}.$$If $n \leq m$ then, by deleting columns of all $0$'s, we may reduce to the case when $n = m$, which is included in the first case. 
***