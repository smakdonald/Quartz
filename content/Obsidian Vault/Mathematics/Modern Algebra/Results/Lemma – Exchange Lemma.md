#### $\lem$ – Exchange Lemma
Let $F$ be a [[Field|field]], let $B$ be a [[Basis and Free Module|basis]] of an $F$-[[Vector Space|vector space]] $V$, and let $C$ be any finite set of $m$ [[Linearly Independent|linearly independent]] vectors in $V$. Then there are distinct vectors $v_1, \dots, v_m$ in $B$, such that $(B \setminus \{v_1, \dots, v_m\}) \cup C$ is also a basis $V$.

###### *Proof.* 

Let $C = \{w_1, \dots, w_m\}$. 
As noted, the  sublemma establishes  the case $w = 1$ of the Exchange Lemma. The general case proceeds recursively:

Suppose that for some $0 \leq k < m$, we have found $v_1, \dots, v_k \in B$ such that $B'' := (B \setminus \{v_1, \dots, v_k\}) \cup \{w_1, \dots, w_k\}$
is a basis for some $k < m$. We need to show we can ``swap out one more''; that is, we need to prove there is a $v_{k+1} \in
(B \setminus \{v_1, \dots, v_k\}) $ such that 
$(B'' \setminus \{v_{k+1}\}) \cup \{w_{k+1}\}$ is also a basis. 

Since $B''$ is a basis, there is a (unique) equation of the form
$$
w_{k+1} = \sum_{i=1}^n a_i u_i
$$
with $u_i \in B''$ and $a_i \ne 0$.  Now, there must be at least one $u_i$ that is not in $\{w_1, \dots, w_k\}$, for
otherwise we would have $w_{k+1} \in \Span( w_1, \dots, w_k)$, contrary to $C$ being linearly independent. 
Let $v_{k+1} = u_i$ for such an $i$. Then by the sublemma
$$
(B'' \setminus \{v_{k+1}\}) \cup \{w_{k+1}\}
$$
is a basis of $V$. 
***