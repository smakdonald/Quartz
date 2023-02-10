### Problem 2 – Proper Subgroup and Union of Conjugates
Let $G$ be a [[Order|finite]] [[Group|group]] and let $H$ be a proper [[Subgroup|subgroup]] of $G$ with $[G:H]=h$[^1].

(a) Prove that $H$ has at most $h$ distinct [[Conjugacy Class|conjugate]] sets $gHg^{-1}$ for $g\in G$.
(b) Prove that $G\neq \bigcup_{g\in G} gHg^{-1}$.

##### *Proof.*
##### Part (a)

Let $f:G/H\to gHg\inv$ be defined by $f(gH)=gHg\inv$. Suppose $xH=yH$. Notice that $f(xH)=xHx\inv$ and $f(H)=yHy\inv$, but as $x=y$ we have equality, and thus $f$ is well defined. Let $gHg\inv$ be a conjugate set, and let $gH\in G/H$. Then $f(gH)=gHg\inv$, and so we have surjectivity. As $|G/H|=|[G:H]|=h$, there can be at most $h$ distinct conjugate sets for $g\in G$. 
***
###### Part (b)
Let $G$ act on $H$ by conjugation. We know that the orbits of this action partition $H$. However, under this action the orbits are exactly the conjugacy classes of $H$. There are at most $h$ conjugacy classes. Each conjugacy class has at most $|H|$ elements in it, and each one has the identity. As there are at most $h$ of them then when we add all of their orders we get at most $h(|H|-1)$, which is less than the order of $G$.
***
#qual

[^1]: Notation: [[Index]]