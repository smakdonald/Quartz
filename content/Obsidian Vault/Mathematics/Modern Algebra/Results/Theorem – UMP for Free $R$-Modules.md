#### $\thm$ – UMP for Free $R$-Modules
Let $R$ be a [[Ring|ring]], let $M$ be a [[Basis and Free Module|free]] $R$-[[Module|module]] with [[Basis and Free Module|basis]] $B$, let $N$ be an $R$-module, and let $j: B \to N$ be any function. Then there is a unique $R$-module [[Homomorphism|homomorphism]] $h: M \to N$ such that $h(b) = j(b)$ for all $b \in B$.

In other words, there is a bijection of sets
$$\Hom_R(M,N) \leftrightarrow\Fun(B, N)$$
given by sending a homomorphisms $f: M \to N$ to its restriction $f|_B:B \to N$ to $B$. (Here, $\Hom_R(M,N)$ is the set of all $R$-module homomorphisms from $M$ to $N$ and $\Fun(B, N)$ is the set of all functions from $B$ to $N$.)

###### *Proof.* 
{\em Existence:}
Given a function $j: B \to N$, define $f: M\to N$ as follows:
Given $m \in M$,   by Lemma \ref{lem:uniquelincomb}  $m$ can be
written uniquely as a finite sum $m = \sum_{b \in B} r_b b$. We set 
$$
f(m) = \sum_{b \in B} r_b j(b).
$$
Note that $f$ is a well-defined function by the uniqueness of the equation $m = \sum_{b \in B} r_b b$.

We need to prove $f$ is an $R$-module homomorphism.
I'll just show it preserves scaling --- the proof for addition is similar.
Given $x \in R$ and $m \in M$, we have $m = \sum_{b \in B} r_b b$ for some $r_b \in R$, and hence
$xm = \sum_b (xr_b) b$. By definition of $f$, 
$$
f(xm) = \sum_b (xr_b) j(b) = x \sum_b r_b j(b) = x f(m).
$$

Finally, for any $y \in B$ we have $y = \sum_{b \in B} r_b b$ where $r_b = 1$ if $b = y$ and $r_b = 0$ if $b \ne y$.
So $f(y) = j(y)$ by construction. This proves existence. 


{\em Uniqueness:} Let $g:M\to N$ be another  $R$-module homomorphism such that $g(b)=g(b)$ for each $b \in B$.
Given $m \in M$ we have $m = \sum_{b \in B} r_b b$ 
and hence
$$
g(m) = \sum_b g(r_b (b)  = \sum_b r_b g(b)  = 
\sum_b r_b j(b) = f(m).
$$
and hence $g = f$. 
***