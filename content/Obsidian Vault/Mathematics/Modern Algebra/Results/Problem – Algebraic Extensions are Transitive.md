### Problem 4 – Algebraic Extensions are Transitive 
Let $F \subseteq K \subseteq L$ be [[Field Extension|extensions]] of [[Field|fields]], not necessarily [[Degree of Field Extension|finite]].

(a) Prove that $K/F$ and $L/K$ are [[Algebraic Extension|algebraic]] if and only if $L/F$ is algebraic.
(b) Give an example where $K/F$ and $L/K$ are [[Galois Extension|Galois]] but $L/F$ is not Galois.

##### *Proof.*
Let $F \subseteq K \subseteq L$ be extensions of fields, not necessarily finite.

###### Part (a) 
Suppose that $K/F$ and $L/K$ are algebraic extensions. Let $\a\in L$. Then $\a$ is the root of the polynomial $$f(x)=a_nx^n+\dots+a_0,$$with $a_{i}\in K$. Notice that $f$ is a polynomial in $F(a_n,\dots,a_0)[x]$, making $\a$ is algebraic over this as well. Consider the [[Chain|chain]] of field extensions
$$F \subseteq F(a_0) \subseteq F(a_0,a_1) \subseteq \cdots \subseteq F(a_0, a_1, \dots, a_{n-1} )\subseteq F(a_0, \dots, a_{n}, \a)$$
Since $a_i$ is algebraic over $F$ for all $i$ and $\a$ is algebraic over $F(a_0, a_1, \dots, a_{n})$, by [[Theorem – Properties of Algebraic Elements|Theorem]] each step in this chain has finite degree. By the [[Proposition – The Degree Formula|Degree Formula]], $[F(a_0, \dots, a_{n}, \a): F]$ is finite and thus so is $[F(\a):F]$. By the Theorem again, $\a$ is algebraic over $F$.

Next suppose that $L/F$ is algebraic. Let $\a\in K$. Then $\a\in L$, and so it is algebraic over $F$. Now let $\b\in L$. Then $\b$ is the root of a polynomial in $F$, which is also in $K$, so $L/K$ is algebraic as well. 
***
###### Part (b) 
$K=\Q(\sqrt{2})$ is Galois over $F=\Q$, and $L=\Q(\sqrt{2},\sqrt[4]{2})$ is Galois over $K$, but $L$ is not Galois over $F$, as the [[Splitting Field|splitting field]] of $x^4-2$ has degree $8$. 
***
#qual