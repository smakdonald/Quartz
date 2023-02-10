#### $\prop$ – Bijection of Matrices and Hom Functor
Suppose $R$ is a [[Ring|ring]] and $F$ and $E$ are [[Basis and Free Module|free]] $R$-[[Module|modules]] with ordered [[Basis and Free Module|bases]]
$X = \{x_1, \dots, x_m\}$ and $Y = \{y_1, \dots, y_n\}$, respectively.
There is a bijective correspondence
$$\Mat_{n \times m}(R) \to \Hom_R(F, E)$$
that sends a matrix $A = (a_{i,j})_{1 \leq i \leq n, 1 \leq j \leq m}$ to the unique $R$-module [[Homomorphism|homomorphism]] $T_A: F \to E$  satisfying  $T_A(x_j)=\sum_{i= 1}^n a_{i,j} y_i$ for each $1 \leq j \leq m$. 

###### *Proof.* 
Assume $R$ is a ring, let $F$ and $E$ be free $R$-modules and let $X \subseteq F$ and $Y \subseteq E$ be chosen bases for each. Let's also assume each basis  is a finite set and choose orderings of their elements: So say
$$
X = \{x_1, \dots, x_m\} 
\textand
Y = \{y_1, \dots, y_n\} 
$$
ordered as $x_1 < \cdots < x_m$ and $y_1 < \cdots < y_n$.
As shown in Example \ref{ex23}, there are isomorphisms of $R$-modules
$$
\phi^F_X: R^m \xra{\cong} F \textand \phi_Y^E: R^n \xra{\cong} E
$$
given by 
$$\begin{equation}
\phi^F_X \left(\begin{bmatrix} r_1 \\ \vdots \\ r_m \end{bmatrix}\right) = \sum_i r_i x_i
\end{equation}$$
and
$$\begin{equation}
\phi^E_Y \left(\begin{bmatrix} s_1 \\ \vdots \\ s_n \end{bmatrix}\right) = \sum_i s_i y_i.
\end{equation}$$
For any $R$-module homomorphism $f: F \to E$, for each $j$ with $1 \leq j \leq m$ we have $f(x_j) = \sum_{i= 1}^n r_{i,j} y_i$ for a unique list of elements $r_{1,j}, \dots, r_{n,j}$ in $R$.  Such an equation exists and is unique since $Y$ is a basis.

Conversely, given and $n \times m$ array of  elements $r_{i,j}$ for $1 \leq i \leq n$ and $1 \leq j \leq m$, let us first define a function $X \to E$ by sending $x_j$ to $\sum_i r_{i,j} y_i \in E$ and then apply by the UMP for free modules to obtain that there is a unique $R$-module homomorphism $f: F \to E$ such that 
$f(x_j) = \sum_{i= 1}^n r_{i,j} y_i$.

Since these two construction are mutually inverse, this proves
***