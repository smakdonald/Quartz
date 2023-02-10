#### $\thm$ – Finding Intermediate Bases
Let $V$ be an $F$-[[Vector Space|vector space]] and assume $I \subseteq S \subseteq V$ are subsets such that $I$ is [[Linearly Independent|linearly independent]] and $S$ spans $V$. Then there is a subset $B$ such that  $I \subseteq B \subseteq S$ and $B$ is a [[Basis and Free Module|basis]] of $V.$  

###### *Proof.* 
Let $\cP$ denote the collection of all subsets $X$ of $V$ such that $I\subseteq X \subseteq S$ and $X$ is linearly independent. We make $\cP$ into a poset by the order relation $\subseteq$, set
containment.

We note that $I \in \cP$. 

Let $\cT$ be any totally ordered subset of $\cP$.  If $\cT$ is empty,
then $\cT$ is (vacuously) bounded above by $I$.

Assume $\cT$ is non-empty. Let $Z = \bigcup_{Y \in \cT} Y$. I claim $Z \in \cP$. Given  $z_1, \dots, z_m \in Z$, for each $i$ we have $z_i \in Y_i$ for some $Y_{i} \in \cT$. Since $\cT$ is totally ordered, one of $Y_1, \dots, Y_m$ contains all the others and hence it contains all the $z_i$'s. Since each $Y_i$ is linearly independent, this shows $z_1, \dots, z_m$ are linearly independent. We have shown that every finite subset of $Z$ is linearly independent, and hence $Z$ is linearly independent. Since $\cT$ is non-empty, $Z \supseteq I$. Since each member of $\cT$ is contained in $S$, $Z \subseteq S$. Thus, $Z \in \cP$, and it is clearly an upper bound for $\cT$. 

We may thus apply Zorn's Lemma to conclude that  $\cP$ has at least one  maximal element,  $B$.  I claim $B$ is a basis of $V$. Note that $B$ is linearly independent and  $I \subseteq B \subseteq S$ by construction. We need to show that it spans $V$. Suppose not. Since $S$ spans $V$, if $S \subseteq \Span(B)$, then $\Span(B)$ would have to be all of $V$. (For note that if $\Span(S) = V$ and  $S \subseteq \Span(B)$, then for any $v \in V$ we may write $v = \sum_i c_i s_i$ for $s_i \in S$ and $s_i = \sum_j a_{i,j} b_{i,j}$ with $b_{i,j} \in B$ and hence $v= \sum_{i,j} c_i a_{i,j} b_{i,j}$, which implies $\Span(B) = V$.)  Since we are assuming $\Span(B) \ne V$, there must be  at least one $v \in S$ such that $v \notin \Span(B)$. Set $X := B \cup \{v\}$. Clearly, $I \subset X \subseteq S$ and, by Lemma \ref{lem1116}, $X$ is linearly independent. This shows that $X$ is an element of $\cP$ that is strictly bigger than $B$, contrary to the maximality of $B$. So, $B$ must span $V$ and hence it is a basis. 
***