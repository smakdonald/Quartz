### Problem 6 – Similarity of 3 x 3 Matrices
Let $F$ be any [[Field|field]].

(a) Let $A$ and $B$ be two $3\times 3$ matrices with entries in $F$. Prove $A$ and $B$ are [[Similar Matrices|similar]] if and only if they have the same [[Characteristic Polynomial|characteristic polynomial]] and the same [[Minimum Polynomial|minimum polynomial]].
(b) Show, by way of an example with justification, that the previous part would become false if  “$3\times 3$” were replaced by “$4\times 4$”.
(c) Give an example of a field $F$ and two $3\times 3$ matrices with entries in $F$ having the same minimum polynomial that are not similar.

##### *Proof*.
Let $F$ be any field.

###### Part (a)
Let $A$ and $B$ be two $3\times 3$ matrices with entries in $F$. 
First, suppose that $A\sim B$ . Matrices are similar if and only if they share the same invariant factors. As minimum polynomial is an invariant factor and the characteristic polynomial is a product of the invariant factors, we see that $A$ and $B$ must share the same invariant factors.

Next suppose that $A$ and $B$ share the same characteristic polynomial and the same minimal polynomial. As $A$ and $B$ are $3\times 3$ matrices, the characteristic polynomial of both $A$ and $B$ must be a degree $3$ polynomial. We proceed via cases based on the degree of $\mp_{A,B}(x)$. 
- First, suppose $\deg\mp_{A,B}(x)=3$. Then $\mp_{A,B}(x)=\cp_{A,B}(x)$, making $\cp_{A,B}(x)$ the only invariant factor of both $A$ and $B$. Thus $A$ and $B$ have the same invariant factors and are therefore similar. 
- Next, suppose $\deg\mp_{A,B}(x)=2$. As $\mp|\cp$ and the degrees of all invariant factors must sum to the $\deg\cp$, we know that $\cp=\mp\cdot k(x)$, where $k(x)$ is a degree $1$ polynomial, which we denote $f(x)$ for $A$ and $g(x)$ for $B$.. Since $A$ and $B$ share the same minimum and characteristic polynomials, we see $\mp\cdot f=\cp$ and $\mp\cdot g=\cp$, and thus that $f=g$. Hence $A$ and $B$ share the same invariant factors, making $A\sim B$. 
- Finally, suppose $\deg\mp=1$. The minimum polynomial is the largest invariant factor, and thus the invariant factors of $A$ and $B$ must be $\{\mp,\mp\mp\}$, making them similar. 
***
###### Part (b) 
If we replaced $3\times 3$ with $4\times 4$ then this would allow for $\cp_{A,B}(x)=x^4$ and $\mp_{A,B}(x)=x^2$, allowing two sets of invariant factors: $\{x^2,x^2\}$  $\{x,x,x^2\}$, 
Notice that $C(x)=\begin{bmatrix}0\end{bmatrix}$ and $C(x^2)=\begin{bmatrix}0&0\\1&0\end{bmatrix}$. Set $A=C(x^2)\oplus C(x^2)$ and $B=C(x)\oplus C(x)\oplus C(x^2)$, so 
$$A=\begin{bmatrix}0 & 0 & 0 & 0 \\1 & 0 & 0 & 0 \\0 & 0 & 0 & 0\\ 0 & 0 & 1 & 0\end{bmatrix} \text{ and } B=\begin{bmatrix}0 & 0 & 0 & 0 \\0 & 0 & 0 & 0 \\0 & 0 & 0 & 0\\ 0 & 0 & 1 & 0\end{bmatrix}.$$ These matrices have the same $\cp$ and $\mp$ but are not similar.
***
###### Part (c) 
Let $F=\Q$. We define $A=C(x-1)\oplus C(x^2-1)$ and $B=C(x+1)\oplus C(x^2-1)$. Notice that these matrices are in [[Theorem – Rational Canonical Form|rational canonical form]]. However, the invariant factors of $A$ are $\{(x+1), (x^2-1)\}$ and the invariant factors of $B$ are $\{(x-1)(x^2-1)\}$. Thus $A$ is not similar to $B$, but the minimal polynomial of both is $x^2-1$. 
***
#qual