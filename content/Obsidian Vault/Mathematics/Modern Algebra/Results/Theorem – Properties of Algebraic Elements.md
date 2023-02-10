#### $\thm$ – Properties of Algebraic Elements
Suppose $F \subseteq L$ is a [[Field|field]] [[Field Extension|extension]] and $\a \in L$. Define $$I := \{f(x) \in F[x] \mid f(\a) = 0\},$$ a subset of $F[x]$[^1].

1. The subset $I$ is an [[Ideal|ideal]] of $F[x]$.
2. $I = 0$ if and only if $\a$ is [[Algebraic Element|transcendental]] over $F$; so $I\neq 0$ if and only if $\a$ is [[Algebraic Element|algebraic]] over $F$.
3. Assume $\a$ is algebraic over $F$.
	- The unique monic [[Generator|generator]] of $I$, which we will write as $m_{\a, F}(x)$[^2], is [[Irreducible|irreducible]] (and hence $I$ is a [[Mathematics/Modern Algebra/Definitions/Prime|prime]] ideal).
	- There is a unique [[Isomorphism|isomorphism]] of fields[^3] $$F[x]/(m_{\a, F}(x)) \cong F(\a)$$sending $F$ identically to $F$ and sending $x$ to $\a$.
	- $F[\a] = F(\a)$ and in particular $F[\a]$ is a field.
4. $\a$ is algebraic over $F$ if and only if $[F(\a): F] < \infty$[^4]. In this case,[^5] $$[F(\a): F] = \deg(m_{\a, F}(x)).$$
5. $\a$ is transcendental over $F$ if and only if $[F(\a): F] = \infty$. In this case, there is a unique isomorphism of fields $$F(x) \cong F(\a)$$ sending $F$ identically to $F$ and sending $x$ to $\a$. (Here, $F(x)=\left\{\frac{g(x)}{f(x)}\mid g\neq 0\right\}$ is the [[Field of Fractions|field of fractions]] of $F[x]$.)

##### *Proof.*
All parts use the following construction:
  
Let $\phi: F[x] \to L$ be the evaluation homomorphism, given by sending $f(x)$ to $f(\a)$. Note that $\phi$  satisfies $\phi|_F = \id_F$ and $\phi(x) = \alpha$. We have $\im(\phi) = F[\a]$ by definition of the latter. 
The First Isomorphism Theorem for rings thus  gives that $\phi$ induces a ring isomorphism
$$\ov{\phi}: \frac{F[x]}{I}  \xra{\cong} F[\a]$$
given by $\ov{\phi}(f(x)+(p(x)))={\phi}(f(x))=f(\a)$.  In particular, since $F[\a]$ is a subring of $L$, it is an integral domain, and hence $I$ must be a prime ideal (possibly the $0$ ideal). 

Let us now prove the various parts:

(1) holds because $I$ is the kernel of the ring map $\phi$. 

(2) is by definition.

For (3) assume $\a$ is algebraic. Then $I \ne 0$ and hence it has a unique monic generator, which we write $m_{\a, F}(x)$. Since $I$ is prime, $m_{\a, F}(x)$ is irreducible; this proves (3a). Also, this shows that $\frac{F[x]}{(m_{\a,F}(x))}$ is a field and hence so is $F[\a]$. Since $F[\a] \subseteq F(\a)$, $F[\a]$ contains $F$ and $\a$, and $F[\a]$ is a field, we must have $F[\a] = F(\a)$. This proves (3b) and (3c).

For (4), if $\a$ is algebraic over $F$, then  $[F(\a):F] = \deg(m_{\a, F}(x)) < \infty$ by  (3b) and Proposition \ref{prop:degreeF(a)}. For the converse, if $[F(\a): F] < \infty$, then the infinite list $1, \a, \a^2, \dots$ of elements of $F(\a)$ cannot be $F$-linearly independent. So, $a_0 + a_1 \a + \cdots a_n \a^n = 0$ for some $n$ and some $a_0, \dots, a_n \in F$ not all of which are $0$. This shows $\a$ is the root of a non-zero polynomial.

For (5), if $\a$ is transcendental, then $I = 0$ and so $\phi: F[x] \into L$ is injective. Since $L$ is a field, $F[x]$ is a domain, and $\phi$ is injective, it can be extended to the field of fractions $F(x)$ of $F[x]$, i.e. there is a ring homomorphism $$\tilde{\phi}: F(x) \to L$$given by $\tilde{\phi} \left(\frac{f(x)}{g(x)}\right) = \frac{f(\a)}{g(\a)}$ for all $f(x), g(x) \in F[x]$ with $g(x) \ne 0$. The image of $\tilde{\phi}$ is precisely $F(\a)$. The map $\tilde{\phi}$ is injective since it is a ring homomorphism whose source is a field. 
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Minimum Polynomial]]
[^3]: See: [[Quotient Ring]], [[Field Extension]]
[^4]: See: [[Degree of Field Extension]]
[^5]: See: [[Polynomial Degree]]