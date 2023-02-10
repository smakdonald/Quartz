### Problem 4 – EDs are PIDs
Let $R$ be a [[Commutative Ring|commutative]] [[Integral Domain|domain]].
(a) State the definition for $R$ to be a [[Euclidean Domain|Euclidean domain]].
(b) Prove that in a Euclidean domain every [[Ideal|ideal]] is [[Principal Ideal|principal]].

##### *Proof.*
Let $R$ be a commutative domain.

###### Part (a)
A Euclidean domain is a domain $R$ together with a function $N: R \to \Z_{\geq 0}$ such that $N(0) = 0$ and the following property holds: for any two elements $a, b \in R$ with  $b \ne 0$, there are elements $q$ and $r$ of $R$ such that
$$
a = qb + r \text{ and either } r = 0 \text{ or }N(r) < N(b).
$$
***
###### Part (b)
Let $I$ be an ideal in $R$, and let $S$ denote the set of norms for a nonzero generating set of $I$. If none exist then $I=(0)$ then in it is principally generated, so we can assume there is some nonzero $x\in I$, meaning our set $S$ is nonempty. 

As $S$ is a set of natural numbers bounded below, by the Least Upper Bound Axiom there exists a smallest element. Let $b$ denote the nonzero element in $S$ with smallest norm.

Suppose $a$ and $b$ are nonzero elements of the generating set for $I$. As $R$ is an ED there exist $q,r\in R$ such that $a=qb+r$ with either $r=0$ or $N(r)<N(b)$. 

Notice that $r=a-qb$, where $a\in I$ and $-qb\in I$ by absorption. Thus $r\in I$, meaning that $N(r)\geq N(b)$. Thus $r=0$. Then $a=qb$, meaning that $a\in (b)$. Thus every element in the generating set for $I$ is contained in $(b)$, and thus $I=(b)$, making $I$ principally generated. 
***
#qual