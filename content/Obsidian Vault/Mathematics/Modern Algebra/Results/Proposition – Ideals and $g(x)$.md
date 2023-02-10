#### $\prop$ – Ideals and $g(x)$
Given a $n \times n$ matrix $A$ with entries in a [[Field|field]] $F$, the set $I := \{g(x) \mid g(A) = 0 \}$ forms a non-zero [[Ideal|ideal]] of $F[x]$[^1].

###### *Proof.* 
$I$ is an ideal since the result of evaluating the sum of two polynomials $g(x) + f(x)$ at $x = A$ is $g(A) f(A)$. the result of evaluating the product $g(x) f(x)$ at $x = A$ is $g(A) f(A)$. 

To show it is non-zero, consider the matrices $I_n, A, A^2, \dots, A^{n^2}$. This is a collection of $n^2 + 1$ matrices in the $n^2$ dimensional $F$-vector space $\Mat_{n \times n}(F)$, and hence the must be linearly dependent: there are $a_0, \dots, a_{n^2+1} \in F$, not all of which are $0$, such that $\sum_i a_i A^i = 0$. This proves $\sum_i a_i x^i \in I$.
***

[^1]: See: [[Polynomial Ring]]