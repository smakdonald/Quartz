### Problem 8 – Galois Group and Transitivity
Suppose that $F \sse L$ is a [[Degree of Field Extension|finite]] [[Galois Extension|Galois extension]] with [[Galois Extension|Galois group]] $G$, and that $\a \in L$. Prove that $L = F (\a)$ if and only if the images of $\a$ under elements of $G$ are distinct.

###### *Proof*.
First, suppose that $L=F(\a)$. As $L$ is a Galois extension the [[Minimum Polynomial|minimum polynomial]] of $\a$ in $F$ splits completely into linear factors (See: [[Theorem – Galois Extension Equivalencies|Theorem]]). Thus $G$ acts [[Faithful Action|faithfully]] on the roots of $\mp_\a(x)$, which includes $\a$ (See: [[Corollary – Automorphisms and Group Actions (Fields)|Corollary]]). Thus the images of $\a$ under elements of $G$ are distinct.

Now suppose that the images of $\a$ under elements of $G$ are distinct, and suppose by way of contradiction that there exists some $\b\in L$ that is not in $F(\a)$. Consider the intermediate field $F(\a,\b)$. By the FTGT there exists a nontrivial subgroup of $G$ whose elements fix elements of $F(\a,\b)$, including $\a$, a contradiction. 
***