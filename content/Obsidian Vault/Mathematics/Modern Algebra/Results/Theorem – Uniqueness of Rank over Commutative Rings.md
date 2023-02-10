 #### $\thm$ – Uniqueness of Rank over Commutative Rings
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] such that $1 \ne 0$ and let $M$ be a [[Basis and Free Module|free]] $R$-[[Module|module]] with [[Basis and Free Module|bases]] $A$ and $B$.
Then $A$ and $B$ have the same [[Dim (Vector Space)|rank]], i.e. there exists a (non unique) bijection of sets joining them.

###### *Proof.* 
Let $R$ be a non-zero commutative ring and let $M$ be a free $R$-module with two {\em finite} bases, $A$ and $B$. 
We need to show $A$ and $B$ have the same cardinality. Since $A$ and $B$ are finite, by Example \ref{ex23}
the assertion is equivalent to the following statement:
\begin{quote} For a non-zero commutative ring $R$,
if there is an isomorphism $R^n \cong R^m$ of $R$-modules for some integers $n$ and $m$, then $n = m$.
\end{quote}

I will prove this statement by taking it as already known that it holds in the special case when $R$ is a field. (We will prove it for fields later.)

Since $R$ is not the zero ring, it contains at least one maximal ideal $I$. (This is proven using Zorn's Lemma.) Recall that $R/I$ is a field.

Given an isomorphism $f: R^n \xra{\cong} R^m$ of $R$-modules, by Lemma \ref{lem727} we have an induced 
homomorphism of $R/I$-module $\ov{f}:  R^n/IR^n \to R^m /IR^m$. Likewise, the inverse map $f^{-1}: R^m \xra{\cong} R^n$ 
induces a map $\ov{f^{-1}}:  R^m/IR^m \to R^n /IR^n$. Also by that Lemma we have
$\ov{f} \circ \ov{f^{-1}} = \ov{f \circ f^{-1}} = \ov{\id} = \id$ and similarly
$\ov{f^{-1}} \circ \ov{f}$ is the identity. That is, we have an isomorphism $R^n/IR^n \cong R^m /IR^m$ of $R/I$-modules.


Next, I claim that there is an isomorphism
$$
R^n/IR^n \cong (R/I)^n
$$
of $R/I$-modules. Define $R^n \to (R/I)^n$ in the evident way (modding out by $I$ entry-wise). 
It is a surjective map of $R$-modules with kernel $I R^n$ and thus, by the First Isomorphism Theorem, it
induces an isomorphism 
$$
g: R^n/I R^n \xra{\cong} (R/I)^n
$$
given by $g((r_1, \dots, r_n)^\tau + IR^n) = (r_1 + I, \dots, r_n + I)^\tau$ (where $\tau$ denotes taking the transpose).  
Now, what we have said so far only shows that $g$ is isomorphism of $R$-modules, but it is easy to see that $g$ is in fact
$R/I$-linear (I'll leave that to you) and thus it is an isomorphism of $R/I$-modules.

Putting the results proven so far together, we conclude that $(R/I)^n$ and $(R/I)^m$ are isomorphic as $R/I$-modules. 
Since $R/I$ is a field and since we are assuming the result holds for fields,  we deduce that $n = m$.
***