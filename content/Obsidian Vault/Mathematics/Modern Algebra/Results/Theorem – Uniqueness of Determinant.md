#### $\thm$ – Uniqueness of Determinant
For each fix positive integer $n$ and non-zero [[Commutative Ring|commutative]] [[Ring|ring]] $R$, the [[Determinant Function|determinant function]] is the unique function of the form $$\phi: \overbrace{R^n \times \cdots \times R^n}^n \to R$$such that
1. $\phi$ is $R$-[[Multilinear and Alternating|multi-linear]],
2. $\phi$ is [[Multilinear and Alternating|alternating]], and
3. $\phi(I_n) =1$ (i.e., $\phi(e_1, \dots, e_n) = 1$ where $e_i$ is the $i$-th standard column vector).

###### *Proof.* 
We start by proving that $\det$ has these properties.\footnote{I might skip this in class.}

Let $v_1, \dots, v_n$ form the columns of a matrix $A$. (I.e, the $s$-th entry of $v_t$ is $a_{s,t}$.)
  We have
$$
\begin{aligned}
\det(v_1, \dots, v_{i-1}, r v_i + v'_i, v_{i+1}, \dots, v_n) 
& =  \sum_{\s} \sgn(\s) \prod_{j\ne i} a_{\s(j), j} \cdot (r a_{\s(i), i} + a'_{\s(i), i})\\
& =  r \sum_{\s} \sgn(\s) \prod_{j\ne i} a_{\s(j), j} \cdot (a_{\s(i), i})  \\
& + \sum_{\s} \sgn(\s) \prod_{j\ne i} a_{\s(j), j} \cdot (a'_{\s(i), i})  \\
& = r \det(v_1, \dots, v_{i-1}, v_i , v_{i+1}, \dots, v_n) +
\det(v_1, \dots, v_{i-1},  v_i', v_{i+1}, \dots, v_n) \\
\end{aligned}
$$
and this proves $R$-multi-linearity. 

For the alternating property, for notational simplicity, let us assume that $v_1 = v_2$  (i.e., the first two columns of the matrix  are equal). (The proof of the general
case is essentially the same.)
Note that$$
\det(A) = \sum_{(i,j, g)} \sgn(i,j,g) a_{i,1} a_{j,2} a_{g(3), 3} a_{g(4), 4} \cdots a_{g(n), n}
$$where the sum ranges over triples $(i,j,g)$ where $i \ne j$ and $g$ is an injective function from $\{3, \dots, n\}$ to $\{1, \dots, n\} \setminus \{i,j\}$ and by $\sgn(i,j,g)$ we mean the sign of the permutation sending $1$ to $i$, $2$ to $j$ and $s$ to $g(s)$ for all other $s$. For each $(i,j,g)$, we have $\sgn(i,j,g) = -\sgn(j,i,g)$, since the corresponding permutations differ by a transposition. Since $a_{i,1} = a_{i,2}$ and $a_{j,1} = a_{j,2}$, it follows that the terms in the formula for $\det(A)$ cancel in pairs to give $0$.

The property $\det(I_n) = 1$ follows from the formula. (See Example \ref{ex215}.)

Let us now prove the uniqueness part of the Theorem:

Let $\phi$ be any function with the three properties stated in the Theorem. Let $A = (a_{i,j})$ be any square matrix with columns $v_1, \dots, v_n$. Note that $v_j = \sum_i a_{i,j} e_i$ where $e_i$ is the $i$-th standard basis (column) vector. Using the $R$-multi-linearity property repeatedly we have
$$
\begin{aligned}
\phi(A) & = \phi(\sum_{i_1} a_{i_1,1} e_{i_1},  \sum_{i_2} a_{i_2,2} e_{i_2}, \cdots, \sum_{i_n} a_{i_n,n} e_{i_n}) \\
& = \sum_{i_1} a_{i_1,1} \phi(e_{i_1},  \sum_{i_2} a_{i_2,2} e_{i_2}, \cdots, \sum_{i_n} a_{i_n,n} e_{i_n}) \\
& = \sum_{i_1}a_{i_1,1} \sum_{i_2} a_{i_2,2} \phi(e_{i_1},   e_{i_2}, \cdots, \sum_{i_n} a_{i_n,n} e_{i_n}) \\
& = \vdots \\
& = \sum_{ i_1, \dots, i_n } a_{i_1, 1} \cdots a_{i_n,n} \phi(e_{i_1}, \dots, e_{i_n}) \\
\end{aligned}
$$
where each of $i_1, \dots, i_n$ ranges from $1$ to $n$. By the alternating property $\phi(e_{i_1}, \dots, e_{i_n}) = 0$ unless all the $i_1, \dots, i_n$ are distinct. If they are distinct, then by Lemma \ref{lem221} we have
$$
\phi(e_{i_1}, \dots, e_{i_n}) = \sgn(\s) \phi(e_1, \dots, e_n)
$$
where $\s$ is the permutation defined as $\s(t) = i_t$. Finally, recall  $\phi(e_1, \dots, e_n) = 1$ by assumption. Putting all of this together gives$$
\phi(A) = \sum_{\text{ distinct  $i_1, \dots, i_n$}} \sgn(\text{the permutation $t \mapsto i_t$}) a_{i_1, 1} \cdots a_{i_n,n}.
$$This is just a re-writing of the formula for $\det$; so $\phi = \det$.
***