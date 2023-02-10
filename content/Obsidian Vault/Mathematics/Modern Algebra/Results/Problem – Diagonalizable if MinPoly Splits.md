### Problem 7 – Diagonalizable if MinPoly Splits
Let $V$ be a [[Dim (Vector Space)|finite dimensional]] [[Vector Space|vector space]] over a [[Field|field]] $F$ and let $\t : V \to V$ be an $F$-[[Linear Operator|linear operator]] on $V$. Prove $\t$ is [[Diagonalizable|diagonalizable]] over $F$ if and only if its [[Minimum Polynomial|minimum polynomial]] $p(x)$ factors into distinct linear terms in $F[x]$[^1]. 

##### *Proof*.
$(\Rightarrow)$ Suppose that $g$ is diagonalizable. Thus there exists a change of basis matrix $A$ such that $A$ is diagonal. As it is diagonal, its diagonal entries are the eigenvalues of $g$, and thus the roots of the minimal polynomial of $g$. Using row and column operations we can rearrange $A$ so that all repeated linear factors are next to each other in the diagonal, for convenience. 

We know that $\mp_A(x)$ is the smallest monic polynomial that sends $A$ to 0. Take all the distinct eigenvalues $\lambda_i$ and consider $q(x)=\prod(x-\lambda_i)$. 

We examine $q(A)$. It will be a product of matrices, one for each $\lambda_i$. First, take the first matrix in this product, $(A-\lambda_1I)$, and note that it sends all $\lambda_1$ in $A$ to 0. Thus all of the rows and columns that contained a $\lambda_1$ are now 0, and thus all these rows and columns will be 0 in the final product $q(A)$. As this is we set $q(x)=\prod(x-\lambda_i)$ for all $l\lambda_i\in A$, we see that for each row and column in $A$ there will exist a matrix $A-\lambda_iI$ in the product $q(A)$ such that the row and column will be 0. Thus the entire matrix will be 0, and $q(A)=0$.

Note that if any $\lambda_i$ were excluded from $q(x)$ there would exist a non-zero row and column for every matrix in the product, and thus $q$ would not send $A$ to 0. Thus $q(x)$ is indeed the minimal polynomial of $A$. As $q(x)=\prod(x-\lambda_i)$, we see it does indeed factor into distinct linear terms. 

$(\Leftarrow)$ Suppose the minimum polynomial of $g$ factors completely into distinct linear factors, each of which has the form $x-\lambda_i$ for some $\lambda_i\in F$. As each $\lambda_i$ is distinct, each elementary divisor is of the form $(x-\lambda_i)^1$.

We construct the Jordan Canonical Form of $g$. As the elementary divisors are linear the Jordan blocks are $1\times1$ matrices, making the $JCF$ a diagonal matrix. As the JCF is itself a change of basis matrix, we see that $g$ is diagonalizable.
***
#qual

[^1]: Notation: [[Polynomial Ring]]