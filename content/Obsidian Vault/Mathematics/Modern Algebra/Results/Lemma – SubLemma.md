#### $\lem$ – SubLemma
Let $F$ be a [[Field|field]]. Given a [[Basis and Free Module|basis]] $B$ of an $F$-[[Vector Space|vector space]] $V$ and vector $w \in V$, let $$w = a_1 v_1 + \cdots + a_n v_n,$$for $n \geq 0$, $0 \ne a_i \in F$ and $v_i \in B$ for all $i$, be the unique way of writing $w$ as a [[Linear Combination|linear combination]] of some of the members of $B$ using non-zero coefficients. Then for any $1 \leq i \leq n$, we have that
$$B' := (B \setminus \{v_i\}) \cup \{w\}$$ is also a basis of $V$.

###### *Proof.* 
If $w = 0$ the sublemma is vacously true since $n = 0$ in that case. 

For $w \ne 0$, we may as well assume (to simplify the notation) that $i =1$. 
We need to show $B' = (B \setminus \{v_1\}) \cup \{w\}$ is linearly independent and spans. 

By solving for $v_1$ (as we may since $a_1 \ne 0$) we obtain
$$
v_1 = b_1 w + \sum_{j \geq 2} b_j v_j 
$$
for some $b_j \in F$ and hence $v_1 \in \Span(B')$. 
Given any $u \in V$, since $B$ spans, we have $u = \sum_i c_i u_i$ for some $c_i \in F, u_i \in B$. 
If one of  $u_i$'s is equal to $v_1$, then we may use the previous equation to replace the term $c_i u_i$ with a linear combination
of members of $B'$. This proves that $u \in \Span(B')$. So $B'$ spans $V$. 

To show $B'$ is linearly indepedent, suppose 
$$
cw + \sum_{i=1}^p c_i u_i= 0
$$
for some $c, c_i \in F$ and some $u_i \in (B \setminus \{v_1\})$. If $c \ne 0$, then we have
$$
w = \sum_i d_i u_i
$$
for some $d_i$. But this contradicts the uniqueness of 
$w = a_1 v_1 + \cdots + a_n v_n$ (for note that  $u_i \ne v_1$ for all $i$). So we must have $c = 0$. 
But then we must also have $c_i = 0$ for all $i$ since $B$ is linearly independent.
This proves $B'$ is linearly independent.  This completes the proof of the sublemma. 
***