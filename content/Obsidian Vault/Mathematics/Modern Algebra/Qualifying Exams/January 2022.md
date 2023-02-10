## Section I: Group theory
Solve two of the following three problems.  
### Problem 1 – Prime Index and HK
[[Problem – Prime Index and HK]]
### Problem 2 – Group of Order 2835
[[Problem – Group of Order 2835]]
### Problem 3 #unfinished

(a) Let $K$ be a [[Subgroup|subgroup]] of a [[Group|group]] $G$. Prove that $K\nsg G$ (See: [[Normal Subgroup|Normal]]) if and only if there is a group $H$ and a [[Homomorphism|homomorphism]] $\varphi : G\to H$ such that $K = \ker(\varphi)$ (See: [[Kernel]]). 
(b) Let $G$ be the group of all $2\times 2$ matrices with entries from $\Z$ having determinant $1$. Let $p$ be prime number, and take $K$ to be the subset of $G$ consisting of all $\begin{bmatrix}a & b\\ c & d \end{bmatrix}$ with $a\equiv d\equiv 1 \mod{p}$ and $b\equiv c\equiv 0\mod{p}$. Prove that K is a normal subgroup of G.

##### *Proof*.
###### Part (a)
First, suppose $K\nsg G$. Let $H=G/K$ (which is a group since $K$ is normal in $G$) and define $\varphi: G\to G/K$ such that $\varphi(g)=gK$. Let $k\in K$, and observe that $\varphi(k)=kK=K$, and so $k\in\ker(\varphi)$. Let $g\in\ker(\varphi)$, meaning that $\varphi(g)=K$, placing $g\in K$. As [[Lemma – Quotient Map is Surjective Homomorphism|quotient maps are homomorphisms]], this direction is complete.

Next, suppose there exists a group $H$ and and a homomorphism $\varphi : G\to H$ such that $K = \ker(\varphi)$. Let $g\in G$ and consider $gKg\inv$. Observe $$\varphi(gKg\inv)=\varphi(g)\varphi(K)\varphi(g\inv)=0,$$given that $\ker(\varphi)=K$. Thus $gKg\inv\subseteq K$ for all $g\in G$, making $K$ a normal subgroup of $G$. 
***
###### Part (b)
So ad-bc=1, b and c are multiples of p 
Let $f$ mod out each of the entries of a matrix by p. 
Thus any matrix in $G$ sent to $I$ must have $a,d$ congruent to 1 mod p and $b,c$ congruent to 0. So $K$ is the kernel of this map. 

f(AB)=AB mod p 
f(A)f(B)=Amodp Bmodp
***
## Section II: Rings, Modules and Linear Algebra  
Solve two of the following three problems.  
### Problem 4 – Prime Ideal with Finite Index
[[Problem – Prime Ideal with Finite Index]]
### Problem 5 #unfinished
Let F be a field, $V$ and $W$ finite dimensional $F$-vector spaces, and $g : V\to W$ an  
$F$-linear transformation.

(a) Prove that there exists bases of $V$ and $W$ such that the matrix representing $g$ with respect to these bases has the form
$$\begin{bmatrix} I_{r\times r} & 0 \\ 0 & 0 \end{bmatrix},$$
where $I_{r\times r}$ is the $r\times r$ identity matrix and all the $0$’s denote zero matrices of the appropriate size.
(b) Prove that the number $r$ appearing in part (a) is independent of choice of bases; that is, if, for another pair of bases of $V$ and $W$, the matrix representing $g$ has the form $$\begin{bmatrix} I_{r'\times r'} & 0 \\ 0 & 0 \end{bmatrix}$$then $r'=r$.

##### *Proof*.
Let F be a field, $V$ and $W$ finite dimensional $F$-vector spaces, and $g : V\to W$ an  
$F$-linear transformation.

###### Part (a) 
We form $B$ and $C$ in steps.

Start by picking an ordered basis   $C' = \{w_1, \dots, w_r\}$ of the image of $g$. For each $i$ pick $v_i \in V$ such that $g(v_i) = w_i$ and set $B' = \{v_1, \dots, v_r\}$. Then pick a basis $B''$ of the kernel of $g$. Let us list the   elements of $B''$ as $\{v_{r+1}, \dots, v_n\}$. 

I claim that $B := B'  \cup B'' = \{v_1, \dots, v_n\}$ is a basis of $V$.  (Note that $B' \cap B'' = \emptyset$ since $g(v_i) = w_i \ne 0$ for all $i$ with $1 \leq i \leq r$ and $g(v_i) = 0$ for all $i > r$.) Pick $v \in V$. Then, since $C'$ spans the image of $g$, we have  $g(v) = \sum_{i=1}^r a_i w_i$ for some scalars $a_i \in F$.
It follows that $v - \sum_{i=1}^r a_i v_i \in \ker(g)$ and hence, since the kernel is spanned by $B''$, 
we have$$v - \sum_{i=1}^r a_i v_i = \sum_{i=r+1}^n a_i v_i,$$for some $a_{r+1}, \dots, a_n \in F$. We rearranging this equation, we conclude $v \in \Span(B)$ and thus $B$ spans $V$.

Now say $\sum_{i=1}^n c_i v_i = 0$ for some $c_i$'s in $F$. Since $g(v_i) = 0$ for all $i > r$ and $g(v_i) = w_i$ for all $i \leq r$, this gives that $0 = g(0) = g(\sum_{i=1}^n c_i v_i) = \sum_{i=1}^n c_i g(v_i) =\sum_{i=1}^r c_i w_i = 0$. Since $C'$ is linearly independent, we have $c_i = 0$ for $1 \leq i \leq r$. Going back to the original equation

$\sum_{i=1}^n c_i v_i = 0$, we see that $\sum_{i=1}^r c_i v_i = 0$ and hence $c_i=0$ for all $i$, since $B''$ is linearly independent.

Finally we extend $C'$ to an ordered  basis $C = \{w_1, \dots, w_r, w_{r+1}, \dots, w_m\}$ of $W$ arbitrarily.

By our construction, for any $v_i \in B$ we have $$
g(v_i) = \begin{cases}
w_i & \text{for $1 \leq i \leq r$ and} \\
0 & \text{for $r+1 \leq i \leq n$} \\
\end{cases}$$and hence
$$
[g]_B^C = 
\begin{bmatrix}
I_r & 0 \\
0 & 0 \\
\end{bmatrix}.
$$

***
###### Part (b) 

***
### Problem 6 – Similarity of 3 x 3 Matrices
[[Problem – Similarity of 3 x 3 Matrices]]
## Section III: Fields and Galois Theory
Solve two of the following three problems.
### Problem 7 – Splitting Field of Positive Quartic
[[Problem – Splitting Field of Positive Quartic]]
### Problem 8 – Cubic Polynomial with Two Complex Roots
[[Problem – Cubic Polynomial with Two Complex Roots]]
### Problem 9 – Construct Field of Size 16
[[Problem – Construct Field of Size 16]]