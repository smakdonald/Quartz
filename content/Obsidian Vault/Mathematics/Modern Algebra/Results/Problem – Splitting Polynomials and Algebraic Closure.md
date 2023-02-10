### Problem 9 – Splitting Polynomials and Algebraic Closure
Assume $F\subseteq L$ is an [[Algebraic Extension|algebraic]] [[Field|field]] [[Field Extension|extension]] such that every non-constant polynomial in $F[x]$ splits completely into linear factors in $L[x]$. Prove $L$ is an [[Algebraic Closure|algebraic closure]] of $F$.

###### *Proof*.
Let $F\subseteq L$ be an algebraic field extension such that every non-constant polynomial in  $F[x]$ splits completely into linear factors in $L[x]$.

Let $f$ be a polynomial in $L[x]$, so $f=a_nx^n+\dots+a_1x+a_0$, with $a_i\in L$, and let $\a$ be a root of $f$. There [[Theorem – Existence and Uniqueness of Algebraic Closures|exists]] some field extension $L\subseteq K$ such that $K$ is [[Algebraically Closed|algebraically closed]], meaning $\a\in K$. Notice that $\a$ is [[Algebraic Element|algebraic]] over $L(\a)$.

Consider the chain of field extensions $$F\subseteq L\subseteq L(\a),$$making $\a$ algebraic over $F$ as well. As every non-constant polynomial in  $F[x]$ splits completely into linear factors in $L[x]$, this yields $\a\in L$. 
***
#qual