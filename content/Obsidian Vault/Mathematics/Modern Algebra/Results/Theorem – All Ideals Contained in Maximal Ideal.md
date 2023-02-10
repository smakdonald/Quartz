#### $\thm$ – All Ideals Contained in Maximal Ideal
If $R$ is a [[Ring|ring]] with $1\neq 0$ and $I$ is a proper [[Ideal|ideal]] of $R$, then there is a [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] ideal of $R$ containing $I$. In particular every ring $R$ contains a maximal ideal.

###### *Proof.* 
Let $\cC$ be the set of proper ideals of $R$ that contain $I$ and view $\cC$ as a poset under containment. We will apply Zorn's Lemma. Suppose $\cT$ is a totally ordered subset of $\cC$. We need to show $\cT$ has an upper bound in $\cC$. If $\cT$ is empty, $I$ is such a bound. Otherwise, let $U = \bigcup_{L \in \cT} L$. 

Since $\cT$ is non-empty, we have $I \subseteq U$ and so  $U\neq \emptyset$. 

Given $x,y \in U$, then $x \in L, y \in L'$ for some $L, L' \in \cT$. Since $\cT$ is totally ordered, either $L \subseteq L'$ or $L' \subseteq L$, and hence $x + y \in L$ or $x +y \in L'$.  Either way, $x + y \in U$.

For $x \in U$ and $r \in R$, we have $x \in L$ for some $L \in \cT$ and hence $rx \in L \subseteq M$. 

This proves $U$ is an ideal that contains $I$. Since every $L\in\cT$ is a proper ideal, $L\cap R^\times =\emptyset$, so $U\cap R^\times  = \bigcup_{L \in \cT} L\cap R^\times=\emptyset$ and hence $U$ is a proper ideal, so $U\in\cC$. By Zorn's Lemma, we conclude $\cC$ has at least one  maximal element $M$. This is a maximal ideal in the sense of definition \ref{def:primemax} since if $J$ is an ideal of $R$ and $M\subseteq J$ then either $J=R$ or, if $J$ is proper, then $J\in \cC$, which yields $J=M$ by using that $M$ is a maximal element of $\cC$.

The existence of a maximal ideal follows by applying the first part of the theorem for $I=(0)$.
***