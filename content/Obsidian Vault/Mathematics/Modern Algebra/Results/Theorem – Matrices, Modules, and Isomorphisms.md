#### $\thm$ – Matrices, Modules, and Isomorphisms
Let $R$ be a non-zero [[Commutative Ring|commutative]] [[Ring|ring]] and let $A \in \Mat_{m \times n}(R)$ and $B \in Mat_{m' \times n'}(R)$ for some $m,n,m',n' \geq 1$. Then $A$ and $B$ present [[Isomorphism|isomorphic]] $R$-[[Module|modules]] if $B$ can be obtained from $A$ by any finite sequence of operations of the following form: 
1. an elementary [[Elementary Row & Column Operations|row]] operation, 
2. an elementary column operation,
3. deletion of the $j$-th column and $i$-th row of a matrix whose $j$-th column is the vector $e_i$,
4. the reverse of (3),
5. deletion of a column of all $0$'s, 
6. the reverse of (5).

###### *Proof.* 
Note: This proof was not covered in class.
Assume $B$ is obtained from $A$ by a single one of the steps listed above. We need to prove that there is an isomorphism $R^m/\im(T_A) \cong R^{m'}/\im(T_B)$ of $R$-modules.
1. In this case,  $B = E A$ for some elementary matrix $E$. More generally, let $E$ be any invertible matrix such that $B = EA$.  Then $T_E: R^m \to R^m$ is an isomorphism and it maps $\im(T_A)$ bijectively onto $\im(T_B)$. It follows that the kernel of the composition $R^m \xra{T_E} R^m \onto R^m/\im(T_B)$ is $\im(T_A)$ and hence by the first isomorphism theorem it induces an isomorphism $$R^m/\im(T_A) \xra{\cong} R^m/\im(T_B).$$
2. In this case, $B=AE$ for some elementary matrix $E$.  More generally, assume $E$ is any  invertible matrix such that $B = AE$. Since $T_E$ is an isomorphism, we have $$\im(T_B) = \im(T_{AE})=\im(T_A\circ T_E)=\im(T_A)$$and so $R^m/\im(T_A) = R^{m}/\im(T_B)$. (For this one we get equality, not merely an isomorphism.)
3. For notational simplicity, let us assume $i = j =1$; that is, the first column of $A$ is $e_1$ and $B$ is obtained by deleting the first row and column of $A$, giving a $(m-1) \times (n-1)$ matrix. So $$A = \begin{bmatrix} 1 & r \\ 0 & B \\\end{bmatrix}$$where $r$ denotes some row vector and $0$ denotes a column of all $0$'s. Let $p: R^{m} \onto R^{m-1}$   and  $q: R^{n} \onto R^{n-1}$  be projection onto the last $m-1$ and $n-1$ components, respectively. Because of the nature of $A$ and $B$, the diagram (page 40 in notes) commutes. Moreover, the kernel of $q$ is $Re_1$ and the kernel of $p$ is $Re_1$, and since the first column of $A$ is $e_1$, $T_A$ maps the kernel of $q$ bijectively onto the kernel of $p$. A "diagram chase'' shows that $\coker(T_A) \cong \coker(T_B)$. In detail: Since the diagram commutes, $p(\im(T_A)) \subseteq \im(T_B)$ and hence $p$ induces an $R$-module  homomorphism $$\ov{p}: R^m/\im(T_A)   \to R^{m-1}/\im(T_B).$$(by the $0$-th isomorphism theorem). Since $p$ is onto, so is $\ov{p}$. Suppose $v + \im(T_A)  \in \ker(\ov{p})$. So, $p(v) \in \im(T_B)$. Say $p(v) = B w$. Since $q$ is onto, $w = q(u)$ for some $u$. Then $$
p(v - Au) = p(v) - pA(u) = p(v) - Bq(u) = p(v) - Bw = p(v) - p(v) = 0, $$ and thus $v - Au \in \ker(p)$. As noted above, $T_A$ maps $\ker(q)$ onto $\ker(p)$ and hence $$v - Au = Ay$$for some vector $y$. This proves $v = A(u+y) \in \im(T_A)$ and hence that $v +\im(T_A) =  0$ in $R^m/\im(T_A)$. This proves $\ov{p}$ is one-to-one.
4. It is clear that the columns of $B$ generate the same submodule of $R^m$ as do the columns of $A$, and thus $\im(T_A) = \im(T_B)$ and $R^m/\im(T_A)  =R^m/\im(T_B)$.
5. Since the isomorphism relation is reflexive, the statements of parts 3. \& 5. show that parts 4.\& 6. are true as well.
***