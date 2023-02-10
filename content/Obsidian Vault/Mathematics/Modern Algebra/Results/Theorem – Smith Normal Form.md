#### $\thm$ – Smith Normal Form
Let $R$ be a [[Euclidean Domain|Euclidean domain]] and let $A \in \Mat_{m \times n}(R)$. Then there is a sequence of elementary [[Elementary Row & Column Operations|row]] and column operations that transform $A$ into a matrix $S = [s_{i,j}]$ such that all non-diagonal entries of $S$ are $0$ and the diagonal entries of $S$ satisfy $$
s_{1,1} \mid s_{2,2} \mid s_{3,3} \mid \cdots.$$ 
###### *Proof.* 
The main point of the proof is to establish: 

  {\bf Claim}: 
There is a sequence of row and column operations that transforms $A$ to 
$$
A' = \begin{bmatrix}
g & 0 \\
0 & B \\
\end{bmatrix}
$$
for some $(n-1) \times (m-1)$ matrix $B$ and  where $g =  \gcd(A)$.
(We adopt the convention that if $A$ is the matrix of all $0$'s, then $g = 0$.)
Note that, by Lemma \ref{lem33}, we have $\gcd(A) = \gcd(A')$ and thus $g \mid \gcd(B)$.


Granting this claim, by applying it again to $B$ we arrive at a matrix of the form
$$
A'' = \begin{bmatrix}
g & 0 & 0\\
0 & g' & 0 \\
0 & 0 & C
\end{bmatrix}
$$
where $g' = \gcd(B)$ and $g \mid g'$ and $g' \mid \gcd(C)$.  (Observe that the row and column operations on $B$ will not affect the first row and column of $A'$.)
Continuing in this fashion, we arrive at the matrix $S$ in the statement.


To prove the claim, let $a$ be the upper-left entry of $A$.

Suppose $a$ happens to be $g = \gcd(A)$. Then, in particular,  it divides  every entry of the first row and column of $A$, and so by doing row
and column operations of type I, we may $0$ out these entries to arrive at a matrix of the desired form directly.
 


In general, let $l$ to be the number of prime factors in a prime factorization of of $a/\gcd(A)$, and 
proceed by induction on  $l$.

If $l = 0$, then $a = \gcd(A)$ (up to associates), and we already did this case.

Assume  $l > 0$. Then there is at least one entry $b = a_{i,j}$ such that $a \nmid b$.

Case I: There is such a $b$ belonging to the first row of $A$. In this case we we may implement the
Euclidean algorithm in the form of suitable column operations to replace $a$ by $\gcd(a,b)$ and $b$ by $0$, as in the example above.  Since  $a \nmid b$,
$\gcd(a,b)$ is a proper divisor of $a$, and it follows that the number of factors in a 
prime factorization of $\gcd(a,b)/g$ is smaller than $l$, and we are done by induction.

Case II: There is such a $b$ in the first column. Just as in the previous case, we are done by induction upon implementing the Euclidean algorithm using suitable row operations.   


Case III: $a$ divides every entry of the first row and first column.  In
this case, suitable row and column operations transform $A$ to 
$$
D = 
\begin{bmatrix}
a & 0 \\
0 & E \\
\end{bmatrix}.
$$
By Lemma \ref{lem33} we have  $\gcd(D) = \gcd(A)$, and thus there is some element 
$e$ of $E$ such that $a \nmid e$ (since we are assuming $a$ is not the gcd of $A$).  A suitable row operation
puts $e$ into row one without affecting $a$, and we are back to the previously solved Case I.
***