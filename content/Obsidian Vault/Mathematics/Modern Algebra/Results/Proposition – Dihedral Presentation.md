#### $\prop$ – $D_{2n}$ Presentation
Let $r:\R^2\to\R^2$ denote counterclockwise rotation around the origin by $\frac{2\pi}{n}$ radians and let $s:\R^2\to\R^2$ denote reflection about the $x$-axis respectively.  Then 
$$D_{2n} = \langle r,s \mid r^n = 1, s^2 = 1, srs^{-1} = r^{-1} \rangle.$$

###### *Proof.* 
Set $X_{2n}=\langle r,s \mid r^n = 1, s^2 = 1, srs^{-1} = r^{-1} \rangle$[^2]. This [[Proposition – Writing Elements of Dihedral Groups|proposition]] gives that $\{r,s\}$ is a set of [[Generator|generators]] for $D_{2n}$[^1] and we also know that  the [[Mathematics/Modern Algebra/Definitions/Relation|relations]] listed above $r^n = 1, s^2 = 1, srs^{-1} = r^{-1}$  are true. The concern is that we may not have discovered all the relations of $D_{2n}$ (or rather, enough relations so that any other valid relation follows as a consequence of the ones listed). 

Assume that $D_{2n}$ has more relations than $X_{2n}$ does. Then $D_{2n}$ would be a group of cardinality strictly smaller than that of  $X_{2n}$, i.e. $|D_{2n}|<|X_{2n}|$. (This will become more clear once we properly define presentations). We show below that in fact $|X_{2n}|\leq 2n=|D_{2n}|$, thus obtaining a contradiction. Now we show that $X_{2n}$ has at most $2n$ elements using just the information contained in the presentation: Every element $x\in X_{2n}$  can be written as 
$$x = r^{m_1} s^{n_1} r^{m_2} s^{n_2} \cdots r^{m_j} s^{n_j}$$for some $j$ and integers (possibly negative) $m_1, \dots, m_j, n_1, \dots, m_j$. (Note that, e.g., $m_1$ could be $0$ so that expressions beginning with a power of $s$ are included in this list.) As a consequence of the last relation, we have
$$
sr = r^{-1}s,
$$
and its not hard to see that this implies
$$
sr^m = r^{-m} s
$$
for all $m$. 
Thus, we can "slide an $s$ past a power of  $r$'', at the cost of changing the sign of the power. Doing this repeatedly gives that we can rewrite $x$ as 
$$
x = r^M s^N
$$
By the first relation, $r^n = 1$, from which it follows that $r^a = r^b$ if $a$ and $b$ are congruent modulo $n$. Thus we may assume $0 \leq M \leq n-1$. Likewise, we may assume $0 \leq N \leq 1$. This gives a total of at most $2n$ elements.
***

[^1]: See: [[Dihedral Group]]
[^2]: See: [[Presentation]]