#### $\defn$ – Jordan Block
Given a [[Field|field]] $F$, and integer $n \geq 1$, and an element $r\in F$,  the *Jordan block* $J_n(r)$ is the $n \times n$ with entries in $F$ such that its diagonal entries are all $r$, each entry just below the diagonal is a $1$, and all other entries are $0$:
$$
J_n(r) = 
\begin{bmatrix}
  r & 0 & 0 & \cdots & 0 \\
  1 & r & 0 & \cdots & 0 \\
  0 & \ddots & \ddots && \vdots \\
  \vdots && \ddots & \ddots & 0\\
  0 & \cdots & 0 & 1 & r \\
  \end{bmatrix}.
$$
(More precisely, $a_{i,i} = r$ for all $1 \leq i \leq n$, $a_{i,i-1} = 1$ for all $2 \leq i \leq n$, and $a_{i,j} = 0$ for all other $i,j$.) 
***