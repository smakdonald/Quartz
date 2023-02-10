#### $\lem$ – Linear Independence and Span
Suppose $I$ is a [[Linearly Independent|linearly independent]] subset of an $F$-[[Vector Space|vector space]] $V$ and $v \in V \setminus \Span(I)$[^1], then $I \cup \{v\}$ is also linearly independent.

###### *Proof.* 
We need to prove that every finite subset of $I \cup \{v\}$ is linearly independent. Let $w_1, \dots, w_n$ be a list of distinct elements  of $I \cup \{v\}$ and suppose $\sum_i c_i w_i = 0$ for some $c_i \in F$. If $v \ne w_i$ for all $i$, then $c_i = 0$ for all $i$ since $I$ is linearly independent. Without loss, say $w_1 = v$. If $c_1 \ne 0$, then $v = \sum_{i \geq 2} c_1^{-1} c_i w_i \in \Span(I)$, contrary to the assumption. So we must have $c_1 =0$. But then $c_i = 0$ for all $i \geq 2$ by the same reasoning as in the first case.
***

[^1]: See: [[|Span]] #fix 