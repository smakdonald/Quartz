#### $\defn$ – Matrix of Free Module Homomorphism
Let $R$ be a non-zero [[Commutative Ring|commutative]] [[Ring|ring]] and  let $V,W$, be $R$-[[Module|modules]] of finite rank $n$ and $m$, respectively. (For instance, $R$ could be a [[Field|field]] and $V$ and $W$ could be arbitrary [[Dim (Vector Space)|finite dimensional]] [[Vector Space|vector spaces]].) Let $B=\{b_1, \dots, b_n\}$ and $C=\{c_1, \dots, c_m\}$ be *ordered* [[Basis and Free Module|bases]] of $V$ and $W$. 
1. For each $v \in V$, let $[v]^B$ denote the unique column vector $\begin{bmatrix} r_1 \\ \vdots \\ r_n \end{bmatrix}$ such that $v = \sum_i r_i b_i$. Define $[w]^C$ for $w \in W$ similarly.
2. If $f: V \to W$ is an $R$-module [[Homomorphism|homomorphism]] then we define elements $a_{ij}\in R$ for $1\leq i\leq m$ and $1\leq j\leq n$ by the formulas $\begin{equation} f(b_i) = \sum_{j=1}^m a_{j,i} c_j. \end{equation}$
Define $[f]_B^C$ to be the matrix
$$[f]_B^C= 
\begin{bmatrix}
a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m,1} & a_{m,2} & \cdots & a_{m,n} \\
\end{bmatrix}.$$
***