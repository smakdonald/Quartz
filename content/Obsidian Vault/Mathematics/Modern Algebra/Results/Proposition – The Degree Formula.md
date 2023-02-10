#### $\prop$ – The Degree Formula
Suppose $F \subseteq L \subseteq K$ are [[Field|field]] [[Field Extension|extensions]]. Then[^1]
$$
[K:F] = [K:L] [L:F].
$$
In particular, the composition of two [[Degree of Field Extension|finite]] extensions of fields is again a finite extension.

###### *Proof.*
Let $A \subseteq K$ be a [[Basis and Free Module|basis]] for $K$ as an $L$-[[Vector Space|vector space]] and let $B \subseteq L$ be a basis for $L$ as an $F$-vector space. Let $AB$ denote the subset $\{ab \mid a \in A, b \in B\}$ of $K$. The Proposition follows from the following two facts:
- $AB$ is a basis of $K$ as an $F$-vector space and
- the function $A \times B \to AB, (a,b) \mapsto ab$ is bijective (so that the cardinality of $AB$ is $|A| \cdot |B|$).
Concerning (a), for $\a \in K$, we have $\a = \sum_i l_i a_i$ for some $a_1, \dots, a_m \in A$ and $l_1, \dots, l_m \in L$. For each $i$, $l_i$ is an $F$-[[Linear Combination|linear combination]] of a finite set of elements of $B$. Combining these gives that $\a$ is in the $F$-span of $AB$. 

To prove [[Linearly Independent|linear independence]], it suffices to prove that if $a_1, \dots, a_m$ and $b_1, \dots, b_n$ be distinct elements of $A$ and $B$ respectively, then the set $\{a_ib_j\}$ is linearly independent.
Suppose $\sum_{i,j} f_{i,j} a_i b_j = 0$ for some $f_{i,j} \in F$. Since the $b_j$'s are $L$-linearly independent and $$\sum_{i,j} f_{i,j} a_i b_j = \sum_j (\sum_i f_{i,j} a_i) b_j$$and $f_{i,j} a_i \in L$, we get that, for each $j$, $\sum_i f_{i,j} a_i = 0$. Using now that the $a_i$'s are $F$-linearly independent, we have that for all $j$ and all $i$, $f_{i,j} = 0$. This proves $\{a_i b_j \mid i = 1, \dots, m, j = 1, \dots, n\}$ is linearly independent over $F$, and hence $AB$ is linearly independent over $F$.

Concerning (b), if $ab = a'b'$ for some $a,a' \in A, b, b' \in B$, then $ab - a'b' = 0$, and since the $b$'s are $L$-linearly independent, we must have $b = b'$ and hence $a = a'$.
***

[^1]: See: [[Degree of Field Extension]]