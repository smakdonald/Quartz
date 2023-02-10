#### Exercise
Let $a, b$ and $c$ be integers. Suppose that $c \not= 0$. Prove that $a|b$ if and 
only if $ac|bc$.
#### Exercise
Let $a$ and $b$ be integers. The numbers $a$ and $b$ are *relatively prime* if the following condition holds: if $n$ is an integer such that $n|a$ and $n|b$, then $n = \pm1$. Prove that the following are equivalent
(a) $a$ and $b$ are relatively prime.
(b) $a$ and $-b$ are relatively prime.
(c) $a + b$ and $b$ are relatively prime.
(d) $a - b$ and $b$ are relatively prime.
#### Exercise
Let $A$ and $B$ be sets. Prove that it is not possible that $A \subsetneq B$ and $B \sse A$ are both true.
#### Exercise
Let $A$ and $B$ be sets. Prove that $(A\cup B)-A = B - (A \cap  B)$
#### Exercise
Let $A$, $B$ and $C$ be sets. Suppose that $C \subset  A \cup B$, and that $C \cap  A = \es$. Prove that $C \sse B$.
#### Exercise
For real numbers $a, b$ and $c$, we know that $a - (b - c) = (a - b) + c$. Let $A, B$ and $C$ be sets.
(a) Suppose that $C \sse A$. Prove that $A - (B -C) = (A - B) \cup C$.
(b) Does $A - (B - C) = (A - B) \cup C$ hold for all sets $A, B$ and $C$? Prove or give a counterexample for this formula. If the formula is false, find and prove a modification of this formula that holds for all sets.
#### Exercise
Let $X$ be a non-empty set, 
and let $S \sse X$ be a subset. The *characteristic map* for $S$ in $X$, denoted $\chi S$, is the function $\chi S : X \to \{0, 1\}$ defined by
\chi S(y) = 
{ 
1, if y \in S 
0, if y \in X - S.

Let $A, B \sse X$ be subsets. Prove that $\chi A = \chi B$ if and only if $A = B$. (Observe that “$\chi A = \chi B$” is a statement of equality of functions, whereas “$A = B$” is a statement of equality of sets.)
#### Exercise
Let $A$ and $B$ be sets, let $P, Q \sse A$ be subsets and let $f : A \to B$ be a function.
(1) Prove that $f (P) - f (Q) \sse f (P - Q)$.
(2) Is it necessarily the case that $f (P - Q) \sse f (P) - f (Q)$? Give a proof or a counterexample.
#### Exercise
Let $A$ be a non-empty set, and let $g : P (A) \to P (A)$ be a function. The function $g$ is *monotone* if $X \sse Y$ implies $g(X) \sse g(Y )$ for all $X,Y \in P (A)$. Suppose that $g$ is monotone.
(a) Let $D$ be a family of subsets of $A$. Prove that g (⋂ 
X\in D X) \sse ⋂ 
X\in D g(X). 
It is not sufficient simply to cite Theorem 4.2.4 (7), because it is not necessarily the case that $g = f_{∗}$ for some function $f : A \to A$.
(b) Prove that there is some $T \in P (A)$ such that $g(T ) = T$. Such an element $T$ is called a fixed point of $g$. Use Part (1) of this exercise.
#### Exercise
Let $A$ and $B$ be sets, let $U \sse A$ and $V \sse C$ be subsets, and let $f : A \to B$ and $g : B \to C$ be functions. Prove that $(g \circ f )(U) = g( f (U))$ and $(g \circ f )-1(V ) = f -1(g-1(V ))$.
#### Exercise
Let $A, B$ and $C$ be sets. Prove that there is a bijective function $g : (A \times B) \times C \to A \times (B \times C)$.
#### Exercise
Let $A$ and $B$ be sets, let $P, Q \sse A$ be subsets and let $f : A \to B$ be a function. Suppose that $f$ is injective. Prove that $f (P - Q) = f (P) - f (Q)$.
#### Exercise
Let $A$ and $B$ be sets, and let $f : A \to B$ and $g : B \to A$ be functions.
(a) Suppose that $f$ is injective, and that $g$ is a left inverse of $f$. Prove that $g$ is surjective.
(b) Suppose that $f$ is surjective, and that $g$ is a right inverse of $f$. Prove that $g$ is injective.
(c) Suppose that $f$ is bijective, and that $g$ is the inverse of $f$. Prove that $g$ is 
bijective.
#### Exercise
Let $A$, $B$ and $C$ be sets, and let $f : A \to B$ and $g : B \to C$ be functions.
(a) Prove that if $g \circ f$ is injective, then $f$ is injective.
(b) Prove that if $g \circ f$ is surjective, then $g$ is surjective.
(c) Prove that if $g \circ f$ is bijective, then $f$ is injective, and $g$ is surjective.
(d) Find an example of functions $f : A \to B$ and $g : B \to C$ such that $g \circ f$ is bijective, but $f$ is not surjective, and $g$ is not injective. Hence Parts (1)–(3) of this exercise are the best possible results
#### Exercise
Let $f : \N \to \N$ be a function. Suppose that $f (n) < f (n + 1)$ for all $n \in\N$. Prove that $f (n)  \geq  n$ for all $n \in \N$. Be explicit about which properties of $\N$, as stated in Section 6.2, you are using.
#### Exercise
Let $f : \N \to \N \cup \{0\}$ be a function. Suppose that $f (1) = 0$, and that if $n < m$ then $f (n) < f (m)$, for all $n, m \in \N$. Prove that for each $x \in \N$, there are unique $n, p \in \N$ such that $f (n) < x  \leq  f (n + 1)$ and $x = f (n) + p$. (If, for example, we let $b \in \N$, and we use the function $f$ defined by $f (n) = (n -1)b$ for all $n \in \N$, then we obtain a variant of the Division Algorithm (Theorem A.5).)
#### Exercise
Let $p \in \N$, and let $G \sse \N$. Suppose that
(a) $1 \in G$;
(b) if $n \in \{1, \dots  , p - 1\}$ and $\{1, \dots  , n\} \sse G$, then $n + 1 \in G$.
Prove that $\{1, \dots  , p\} \sse G$.
#### Exercise
Let $k, m \in \N$, and let $f : \{1, \dots  , m\} \to \{1, \dots  , k\}$ be a function. 
Prove that if $m > k$, then $f$ is not injective. A combinatorial interpretation of this fact is known as the Pigeonhole Principle, which says that if m objects are placed in $k$ boxes, where $m > k$, then there will be a box with more than one object in it. Though this principle may seem innocuous, it is very important in combinatorics. 
#### Exercise
Let $A$ and $B$ be sets, let $X \sse A$ be a subset and let $f : A \to B$ be a function. Suppose that $f$ is injective. Prove that $X  \sim  f (X)$.
#### Exercise
Let $A$ and $B$ be sets. Suppose that $A  \sim  B$. Prove that if $A$ is finite, infinite, countably infinite, countable or uncountable, then so is $B$.
#### Exercise
(a) Give an example of sets $A, B$ and $C$ such that $A  \sim  B$ and $A \cup C \not \sim  B\cup C$.
(b) Let $A, B$ and $C$ be sets. Suppose that $A  \sim  B$ and that $A \cap  C = \es$ and $B \cap  C = \es$. Prove that $A \cup C  \sim  B \cup C$.
(c) Let $A, B$ and $C$ be sets. Suppose that $A \cup C  \sim  B \cup C$ and that $A \cap  C = \es$ and $B \cap  C = \es$. Is it necessarily the case that $A  \sim  B$? Give a proof or a counterexample.
#### Exercise
Let $A$ and $F$ be sets. Suppose that $F$ is finite, and that $A$ is respectively finite, infinite, countably infinite, countable or uncountable.
(a) Prove that $A - F$ is respectively finite, infinite, countably infinite, countable or uncountable.
(b) Prove that $A \cup F$ is respectively finite, infinite, countably infinite, countable or uncountable.
#### Exercise
Let $A, B$ and $C$ be sets.
(a) Prove that $\es 4 A$.
(b) Prove that $A 4 A$.
(c) Prove that if $A 4 B$ and $B 4 C$, then $A 4 C$.
#### Exercise
Let $A$ and $B$ be sets. Suppose that $A$ and $B$ are finite. Prove that $A \cup B$ is finite.
#### Exercise
Let $A \sse \N$ be a subset. Suppose that there is some $M \in \N$ such that $a  \leq  M$ for all $a \in A$. Prove that $A$ is finite.
#### Exercise
Let $A$ be a set. Prove that $A$ is finite if and only if there is an injective function $f : A \to \{1, \dots  , n\}$ for some $n \in \N$ if and only if there is a surjective function $f : \{1, \dots  , n\} \to A$ for some $n \in \N$.
#### Exercise
Let $A$ and $B$ be sets, and let $f : A \to B$ be a function. Suppose that $A$ and $B$ are finite sets, and that $|A| = |B|$. Prove that $f$ is bijective if and only if $f$ is injective if and only if $f$ is surjective.
#### Exercise
Let $F \sse \N$ be a set. Suppose that $F$ is finite and non-empty. Use Theorem 6.3.11 (1) to prove that there is some $k \in F$ such that $p  \leq  k$ for all $p \in F$.
#### Exercise
Let $X$ be a set. Suppose that $X$ is countably infinite. Prove that there is a function $f : X \to X$ that is injective but not surjective.
#### Exercise
Let $A$ be a set. Prove that $A$ is uncountable if and only if it contains an uncountable subset.
#### Exercise
Let $A$ and $B$ be sets. Suppose that $A$ and $B$ are countable. Prove that $A \times B$ is countable.
#### Exercise
(a) Let $n \in \N$. Let $An$ be the set of all roots of polynomials of degree $n$ with rational coefficients. Prove that $A n$ is countable. You may assume the fact that a polynomial of degree $n$ has at most $n$ roots.
(b) Prove that the set of algebraic numbers is countably infinite.
#### Exercise
(a) Prove that $(0, 1) \times (0, 1)  \sim  (0, 1)$. Use the fact that every real number can be expressed uniquely as an infinite decimal, if decimal expansions that eventually become the number $9$ repeating are not allowed.
(b) Let $A$ and $B$ be sets. Suppose that $A  \sim  \R$ and $B  \sim  \R$. Prove that $A \times B  \sim  \R$.
#### Exercise
This exercise is for the reader who is familiar with the complex numbers. Prove that the set of complex numbers $\C$ has the same cardinality as $\R$.