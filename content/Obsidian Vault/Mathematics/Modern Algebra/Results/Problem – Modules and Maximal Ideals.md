### Problem 5 – Modules and Maximal Ideals
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] (with $1$)[^1] and let $M$ be an $R$-[[Module|module]]. Show that if $M\neq 0$ and the only [[Submodule|submodules]] of $M$ are $0$ and $M$, then there is a [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] [[Ideal|ideal]] I of $R$ such that $M$ is [[Isomorphism|isomorphic]] to $R/I$[^2].

##### *Proof*.
Let $R$ be a commutative ring (with $1$) and let $M$ be an $R$-module such that $M\neq 0$ and the only submodules of $M$ are $0$ and $M$. 

As $M\neq 0$, there exists a non-zero element $m\in M$. Let $f:R\to M$ be defined by $f(r)=rm$. Since $1\in R$ and $1m=m\in Rm$, we have $Rm=M$. By the [[Theorem – Module Isomorphism Theorems|First Isomorphism Theorem]] we see that $R/\Ker(f)\cong M$, making $\Ker(f)$ an ideal in $R$, which we shall conspicuously denote as $I$ henceforth. By the Lattice Isomorphism Theorem the only two ideals of $R/I$ are $0$ and $R/I$, making $R/I$ a field, and $I$ a maximal ideal in $R$.
***
#qual

[^1]: Notation: [[Unital Ring]]
[^2]: Notation: [[Quotient Ring]]