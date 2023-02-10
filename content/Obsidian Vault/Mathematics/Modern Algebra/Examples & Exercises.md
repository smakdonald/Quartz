#### Example – Non-Abelian Groups
1. For any set $S$, the [[Permutation Group|permutations]] on $S$ $$\rm{Perm}(S)=\{f:S\to S \ | \ f \text{ is a bijection}\}$$form a non-[[Abelian Group|abelian]] [[Group|group]] under composition.
2. For any [[Field|field]] $F$ and positive integer $n$, let $$\GL_n(F)=\{ \text{invertible }  n \times n \text{ matrices with entries in } F\}.$$By invertible I mean those matrices that have two-sided inverses, but in turns out that if an $n \times n$ matrix has a left inverse then it it is automatically a right inverse too, and vice versa. Then $\GL_n(F)$ is a non-[[Abelian Group|abelian]] [[Group|group]] under matrix multiplication. 
#### Example – Abelian Groups
1. the *trivial* [[Group|group]] is the group with a single element $\{e\}$.
2. $(\Z, +)$, $(\Q, +)$, $(\R, +)$ and $(\C,+)$. 
3. For any $n$, let $\Z/n$ denote the integers modulo $n$. Then $(\Z/n, +)$ is an [[Abelian Group|abelian]] group where $+$ denotes addition modulo $n$.
4. For any [[Field|field]] $F$ (e.g., $\Q, \R, \C$ or $\Z/p$ for a prime $p$), the set $F^{\times} := F \setminus\{0\}$ is an abelian group under the usual multiplication.
#### Exercise – $|\GL_n(\Z/p)|$
These example are infinite if $F$ is infinite, but if we take $F = \Z/p$ for a prime $p$, then $\GL_n(\Z/p)$ is a finite group. Can you find its cardinality?

###### Solution
***
#### Exercise – Left Inverse Without Right Inverse
Give an example of a pair $(G,\cdot)$ that satisfies axioms 1 and 2 of the [[Group|group definition]] and an element of $G$ that has a *left* inverse but not a *right* inverse.

###### Solution
***
#### Exercise – $sr$ is a Reflection
Prove that $sr$ is a reflection and hence that $srsr=1_{\R^2}$.

###### Solution
***
#### Exercise – Disjoint Cycles Commute
Disjoint [[Cycle|cycles]] commute, that is, if $i_1 , i_2 \, \dots i_m, j_1 , j_2 \, \dots j_k\in [n]$,
$$\sigma_1=(i_1 \, i_2 \, \dots i_m), \quad \sigma_2=(j_1 \, j_2 \, \dots j_k)$$
and
$$\{i_1 , i_2 , \dots i_m\}\cap \{j_1 , j_2 , \dots j_k\}=\emptyset,$$
then $\sigma_1 \circ \sigma_2=\sigma_2\circ \sigma_1$.

###### Solution
***
#### Example – Isomorphisms
The identity map is a group isomorphism for any group $G$.
The exponential map $\exp: (\R, +) \to (\R \setminus \{0\}, \cdot)$ is a homomorphism. So is $\ln: (\R_{>0}, \cdot) \to (\R, +)$. In fact, these maps are inverse to each other so we obtain an isomorphism . $(\R, +)\cong (\R_{>0}, \cdot)$.
***
#### Example – Homomorphism
For any positive integer $n$ and field $F$, the map determinant map $\det: \GL_n(F) \to (F \setminus \{0\}, \cdot)$ is a group homomorphism.
***
#### Example – $S_n, \Z/n, D_{2n}$
- $S_n\cong S_m$ if and only if $n=m$ by comparing the orders of the groups.
- $\Z/6\ncong S_3$ because $\Z/6$ is abelian and $S_3$ is not abelian.
- $D_{24}\ncong S_4$ because $|Z(D_{24})|=2$ by  HW~1 and  $|Z(S_n)|=1$ (i.e., $Z(S_n)=\{\id_{[n]}\}$). Arguing with orders of elements works as well.
***
#### Example – Trivial Action
For any [[Group|group]] $G$ and any set $S$, $g \cdot s := s$ defines an [[Group Action|action]], the *trivial action*. The associated group [[Homomorphism|homomorphism]] is $G \to \Perm(S)$ by $g\mapsto \id_S$.
***
#### Example – $D_{2n}$ Acting on $P_n$
The [[Group|group]] $D_{2n}$ [[Group Action|acts]] on the vertices of $P_n$, which I will number as $V_1, \dots, V_{n}$ in a counterclockwise fashion, with $V_1$ on the positive $x$-axis. That is, $D_{2n}$ acts on $S=\{V_1, \dots, V_n \}$. In detail, for $g \in D_{2n}$ and a number $1 \leq j \leq n$, set $g \cdot V_j = g(V_j)$. Note that by the distance-preserving property where we consider distance from the origin $g$ takes vertices of $P_n$ to vertices of $P_n$ and so $g(V_i)$ is really an element of $S$. This satisfies the two axioms of a group action.
***
#### Example – Conjugation Action
Let $G$ be any [[Group|group]] and fix an element $g \in G$. Define *the conjugation action* of $G$ on itself by setting $$g\cdot x=gxg^{-1} \text{ for any } g,x\in G.$$The [[Group Action|action]] of $G$ on itself by conjugation is not necessarily [[Faithful Action|faithful]]. In fact the [[Kernel|kernel]] of the [[Proposition – Permutation Representation|permutation representation]] for the conjugation action is the [[Center|center]] $Z(G)$. In detail, if $\rho:G\to \Perm(G)$ is the permutation representation for $G$ acting on $G$ by conjugation, then $$g\in \ker\rho\iff g\cdot x=x, \forall x\in G \iff gxg^{-1}=x, \forall x\in G$$
$$ \iff gx=xg, \forall x\in G \iff g\in Z(G). $$
***
#### Example – $\Z,\Q,\C$
$\Z < \Q < \R < \C$ and $\Z^\times < \Q^\times < \R^\times < \C^\times$.
***
#### Example – $\SL_n(F)$
For any [[Field|field]] $F$, the *special linear group*
$$\SL_n(F)=\{A \mid A = n\times n \text{ matrix with entries in } F, \det(A)=1_F\}$$
is a [[Subgroup|subgroup]] of the general linear group $\GL_n(F)$ because $\SL_n(F)$ is the [[Kernel|kernel]] of the group [[Homomorphism|homomorphism]] $\det:\GL_n(F)\to F^\times$.
***
#### Example – $\langle x\rangle$
The Lemma implies that for an element $x$ of a [[Group|group]] $G$, $\langle x\rangle=\{x^j \mid j\in \Z\}$.
***
#### Example – Generating $D_{2n}$
$D_{2n}=\langle r,s \rangle$, meaning that $D_{2n}$ is the [[Subgroup|subgroup]] of $D_{2n}$ [[Generator|generated]] by $\{r,s\}$. Do not mistake this for a [[Presentation|presentation]] with no [[Mathematics/Modern Algebra/Definitions/Relation|relations]].
***
#### Example – Generating $S_n$
For any $n$, $S_n$ is generated by the collection of "adjacent transpositions''.
***
#### Example – Cyclic Groups
The main examples of [[Cyclic|cyclic]] [[Group|groups]] (in additive notation) are
- $(\Z,+)$, with [[Generator|generator]] 1 or -1, and 
- $(\Z/n,+)$ with generator $[a]_n$ for any integer $a$ such that $\gcd(a,n)=1$.
***
#### Example – Poset
The set of all positive integers is a poset with respect to divisibility ($a\leq b$ iff $a|b$). The supremum of $a$ and $b$ is $\lcm(a,b)$ and the infimum of $a$ and $b$ is $\gcd(a,b)$.
***
#### Example – Subsets of Set is Poset
The set of all subsets of a set is a poset with respect to containment ($A\leq B$ iff $A\subseteq B$). The supremum of $A$ and $B$ is $A\cup B$ and the infimum of $A$ and $B$ is $A\cap B$.
***
#### Example – Quotient of $\Z$
Let $G=\Z$ and let $\sim$ be $\equiv \pmod n$ for some $n\in \Z$, $n\geq 1$. Then $$(\Z,+)/\equiv \pmod n=(\Z/n,+).$$
***
#### Example – Left Cosets and Modular Arithmetic
Let $G=\Z$ and $H=\langle n\rangle=n\Z=\{nk \mid k\in \Z\}$. Then $x\sim_{ n\Z} y \iff x=y+nk$ for some $k\in \Z$ $\iff x\equiv y \pmod n$. Therefore the equivalence relation $\sim_{ n\Z}$ is the same as congruence modulo $n$ and the right and left [[Coset|cosets]] of $n\Z$ in $\Z$ are the congruence classes of integers modulo $n$.
***
#### Exercise – Number of Cosets in Infinite Groups
Even if $G$ is not [[Order|finite]] the number of left and right [[Coset|cosets]] of a [[Subgroup|subgroup]] $H\leq G$ is still the same. *(Hint*: consider the map $gH\mapsto Hg^{-1}$ and show it's a bijection. Why is the inverse needed?)

###### Solution
***
#### Example – Normal Subgroups
- The trivial [[Subgroup|subgroups]] $\{e\}$, $G$ of a [[Group|group]] $G$ are [[Normal Subgroup|normal]].
- Any subgroup of an [[Abelian Group|abelian]] group is normal.
- Any subgroup of [[Index|index]] two is normal (see HW~4).
- For any group $G$, $Z(G)\norm G$.
- $A_n\norm S_n$ (see HW~3).
- [[Kernel|Kernels]] of group [[Homomorphism|homomorphisms]] are normal (see HW~4). We will see later that, conversely, all normal subgroups are kernels of group homomorphisms.
- Preimages of normal subgroups are normal, that is, if $f:G\to H$ is a group homomorphism and $K\norm H$ then $f^{-1}(K)\norm G$ (see HW~4).
***
#### Exercise – Coset Equivalence
If $A,B$ are subsets of a [[Group|group]] $G$ and $g\in G$ then $$A=B\iff Ag=Bg\iff gA=gB.$$

###### Solution
***
#### Example – Infinite Dihedral Group
The *infinite dihedral group* $D_\infty$ is the set $D_\infty = \{r^i,r^is \mid i \in \Z\}$ with multiplication defined by $(r^i)(r^j) = r^{i+j}, (r^i)(r^js) = r^{i+j}s, (r^is)(r^j) = r^{i-j}s$, and $(r^is)(r^js) = r^{i-j}$. 
In other words,  $D_\infty$ is the [[Group|group]] having [[Presentation|presentation]]
$$D_\infty=\langle r,s \mid s^2=e, srs=r^{-1}\rangle.$$
Then $\langle r^n \rangle \norm D_\infty$ and $D_\infty/ \langle r^n \rangle \cong D_{2n}$ via $r\langle r^n \rangle\mapsto r$ and $s\langle r^n \rangle\mapsto s$.
***
#### Example – Commutator Subgroup
Let $G$ be any [[Group|group]]. For $x,y \in G$, set $[x,y] = xyx^{-1}y^{-1}$. Let $G'$ denote the *commutator subgroup* of $G$ [[Generator|generated]] by all elements of the form $[x,y]$ for $x,y \in G$. (Some people write $G'$ as $[G,G]$.) Then  $G'$ is in fact [[Normal Subgroup|normal]]: $G' \norm G$.  

Now let $f: G \to A$ be any group [[Homomorphism|homomorphism]] from $G$ to an [[Abelian Group|abelian]] group $A$. Since $f([x,y]) = [f(x),f(y)] = e$ for all $x, y \in G$ (since $A$ is abelian), we have that $\ker(f)$ must contain $G'$. By the [[Theorem – UMP of a Quotient Group|UMP]] for quotients, we get that $f$ factors as
$$f:G \xra{\pi} G/G' \xra{\overline{f}} A$$
for a unique group homomorphism $\ov{f}$.  The group $G/G'$ is called the *abelianization* of $G$ and the motto is: A homomorphism from a group to an abelian group factors uniquely through the abelianization.
***
#### Example – FIT and Matrices
For a [[Field|field]] $F$ and integer $n \geq 1$, set $G = \GL_n(F)$. Let $H = \SL_n(F)$, those square matrices with determinant $1$. This is a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] for say $A \in \GL_n(F)$ and $B \in \SL_n(F)$. Then $$\det(ABA^{-1}) = \det(A) \det(B) \det(A)^{-1} = \det(A) \det(A)^{-1} = 1,$$so that $ABA^{-1} \in H$. This proves $A \SL_n(F) A^{-1} \subseteq \SL_n(F)$. 
Let's prove that $\GL_n(F)/\SL_n(F) \cong (F \setminus \{0\}, \cdot)$. The map $$\det: \GL_n(F) \to (F \setminus \{0\}, \cdot)$$is a surjective group [[Homomorphism|homomorphism]] whose [[Kernel|kernel]] is by definition $\SL_n(F)$. Now apply the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]].
***
#### Exercise – Properties of $HK$
1. If $H\leq G$ and $K\leq G$ then $HK\leq G$ if and only if $HK=KH$.
2. If $H\leq G$ and $K\leq G$ and either one of $H$ or $K$ is a normal subgroup then $HK\leq G$ and $HK=KH=\langle H\cup K\rangle$.
***
#### Example – $HK$ and $D_{2n}$
In $D_{2n}$, let $H=\langle s\rangle$ and $K=\langle r\rangle$. Then $HK=KH=D_{2n}$ but of course $r$ and $s$ do not commute. The fact that $HK=KH$ can also be justified by observing that $K\norm D_{2n}$.
***
#### Example – SIT and Matrices
For a field $F$ and integer $n \geq 1$, let $G = \GL_n(F)$, $N = SL_n(F)$ and $H$ the set of diagonal invertible matrices. As we known $N \norm G$ and it's pretty easy to see $H \leq G$. Moreover, $H N = G$ since every invertible matrix $A$ can be written as a product of a diagonal matrix and a matrix of determinant $1$. 
It follows that
$$H/(N \cap H) \cong G/N$$ and since we previously showed that $G/N \cong (F \setminus \{0\}, \cdot)$ we get
$$H/(N \cap H) \cong (F \setminus \{0\}, \cdot).$$

Indeed, it's not hard to see this directly (without using the 2nd Isomorphism Theorem). Note that 
$$H \cong (F \setminus \{0\}, \cdot)^{\times n}$$
where the right-hand side denotes a cartesian product of groups. $N \cap H$ consists of those diagonal matrices of determinant $1$ and, under this isomorphism, it corresponds to the subgroup of 
$M$ of $(F \setminus \{0\}, \cdot)^{\times n}$ consisting of  those $n$-tuples $(x_1, \dots, x_n)$ with $\prod_i x_i = 1$. 
We have
$$(F \setminus \{0\}, \cdot)^{\times n}/M \cong (F \setminus \{0\}, \cdot)$$
via the map induced by the map that  sends $(x_1, \dots, x_n)$ to $x_1 \cdots x_n$ (using there First Isomorphism Theorem). 
***
#### Example – TIT and Matrices
Let $G = \GL_n(\R)$, $N = \{A \in \GL_n(\R) \mid \det(A) > 0\}$ and $M = \SL_n(\R)$. It's not hard to see $N \norm G$, it is clear $M \leq N$ and we already know $M \norm G$. By the Third Isomorphism Theorem we get
$$\GL_n(\R)/N \cong (\GL_n(\R)/\SL_n(\R))/(N/SL_n(\R)).$$
Let us analyze the right hand side a bit. Recall $\GL_n(\R)/\SL_n(\R) \cong (\R \setminus \{0\}, \cdot)$ via the determinant map. Under this isomorphism, $N/SL_n(\R)$ corresponds to $(\R_{>0}, \cdot)$. So the right hand is isomorphic to $(\R \setminus \{0\}, \cdot)/(\R_{>0}, \cdot)$. The latter is isomorphic to the two element group $(\pm 1, \cdot)$ via the sign map $x \mapsto x/|x|$. 
So, $\GL_n(\R)/N \cong (\pm 1, \cdot)$. We could have proven this directly by defining a function $\psi: \GL_n(\R) \to (\pm 1, \cdot)$ by $\psi(A)=\det(A)/|\det(A)|$ and checking that it is a surjective homomorphism with kernel $N$. 
***
#### Exercise – Homomorphisms Preserve Normality
If $f:G\to H$ is a group homomorphism and $K\norm G$ then $f(K)\norm f(G)$. In particular, if $f$ is surjective then $f(K)\norm H$ (but  this need not be true in the absence of surjectivity, see HW~4).

###### Solution
***
#### Example – Lattices
The picture on the left below shows the lattice of subgroups of $C_{12}\cong \Z/12$ and that on the right the lattice of subgroups of its quotient $C_{12}/C_2\cong \Z/12/\langle[6]\rangle$
IMAGE NEEDED
***
#### Example – Free Groups
The free group on a singleton set $A={x}$ is the infinite cyclic group $C_\infty$. It is easy to visualize this since $C_\infty\cong \Z$.
It is already somewhat challenging to visualize the free group on two generators, $F({x,y})$. The best one can do to represent it  is an infinite graph called the *Cayley graph* of this group. It is obtained by starting at the origin (the center of the picture below), then branching out in four directions by a length of 1, then branching out similarly by a length of 1/2, then by 1/4, then by 1/8, etc ( I stopped there, to avoid cluttering the picture too much but to get the complete Cayley graph one continues infinitely obtaining a fractal kind of picture). Then every element of $F ({x, y})$ corresponds in a rather natural way to exactly one dot in this diagram. Indeed, we can place the empty word at the center; and we can agree that every $x$ in a word takes us one step to the right, every $x^{-1}$ to the left, every $y$ up, and every $y^{-1}$ down. For example, the word $yx^{-1}yx$ takes us here:
***
#### Example – Presentation for $C_n$
For $A=\{x\}$, $R=\{x^n\}$ we obtain the cyclic group of order $n$:
$$C_n=\langle x \mid x^n=e\rangle = \frac{F(\{x\})}{\langle x^n\rangle ^N}=C_\infty/\langle x^n \rangle.$$
***
#### Example – Verifying $D_{2n}$ Presentation
For $A=\{r,s\}$, $R=\{s^2,r^n,srsr\}$ we obtain the usual presentation for $D_{2n}$:
$$D_{2n}=\langle r,s \mid s^2=e,r^n=e,srsr=e \rangle =\frac{F\left( \{r,s\}\right)}{\{s^2,r^n,srsr\}^N}.$$
***
#### Example – Presentation UMP and Matrices
To find a groups homomorphism $D_{2n}\to \GL_2(\R)$ it suffices to find a map $g:\{r,s\}\to \GL_2(\R)$, say $r\mapsto R, s\mapsto S$ and to verify that $S^2=I_2,R^n=I_2, SRSR=I_2$. As you have shown on homework, this does hold for the matrices
$$R=\begin{bmatrix} \cos\left(\frac{2\pi}{n}\right) & -\sin\left(\frac{2\pi}{n}\right) \\ \sin\left(\frac{2\pi}{n}\right)& \cos\left(\frac{2\pi}{n}\right)\end{bmatrix}, S=\begin{bmatrix}  0 & 1 \\ 1& 0\end{bmatrix}.$$
By the UMP of the presentation there is a group homomorphism $f:D_{2n}\to \GL_2(\R)$ that extends $g$; that is $f(r^is)=R^iS$ for all $0\leq i<n$.
***
#### Example – Symmetries of the Cube
Let $G$ be the group of orientation-preserving symmetries of the cube (equivalently isometries of the cube which are compositions of rotations). 
Let $G$ act on the collection $S$ of $6$ faces of the cube. This action  is transitive and so the one and only orbit has length $6$. Moreover, thinking of $F$ as a square, the orientation preserving isometries of $F$ are just the orientation-preserving elements of $D_8$ which there are 4 of. Indeed, these correspond to the 4 rotations of the cube  by $0$, $90$, $180$ or $270$ degrees about the axis of symmetry passing through the mid-point of $F$ and the mid-point of the opposite face. Applying the orbit-stabilizer theorem gives
$$|G|=|\Orb_G(F)|\cdot |\Stab_G(F)]=6\cdot 4=24.$$
***
#### Example – Conjugacy Classes of $S_4$
The conjugacy classes for $S_4$ are
1. $\{e\}$, 
2. all two cycles of which there are ${4 \choose 2} = 6$, 
3. all three cycles of which there are $4 \cdot 2 = 8$, 
4. all four cycles of which there are $3! = 6$, and 
5. all product of two disjoint two cycles of which there are $3$.
This totals $24$, as we need, since the conjugacy classes partition $S_4$. 
***
#### Example – Normal Subgroups in $S_4$
One thing we get from the previous example and lemma is a very short list of all possible sizes of normal subgroups of $S_4$. Here's why:
An important, general observation is that, any group $G$ and $N \nsg G$, since $gNg^{-1} = N$ for all
$g$, it follows that $N$ is necessarily a union of conjugacy classes. In other words, the action of $G$ on itself by conjugation restricts to an action on $N$
since $N$ is normal, and thus $N$ is a union of orbits of this action. Moreover, if $G$ is finite then,
by Lagrange, $|N| \mid |G|$. Finally, $N$ certainly contains $e$. Putting these facts together we get than $|N|$ must both divide $|G|$ and be a sum of
cardinalities of conjugacy classes, including the class $\{e\}$.
For example, if  $N \nsg S_4$, then $|N| \mid 24$ and $|N|$ must equal $1$ plus the sum of some sub-list of 
$6, 8, 6, 3$. The only possibilities are
$$1, 1 + 3, 1 + 3 + 8, \text{ and }1 + 6 + 8 + 6 + 3$$
Having determined the sizes, also determines what the corresponding set $N$ is. Let me stress that just because the size of $N$ satisfies the restrictions given by Lagrange's theorem and Corollary \ref{lem:normconj} it does not automatically follow that $N$ really is a subgroup or that it is normal.  (In other words these are just necessary conditions.) So we still need to check whether the candidate sets we found do indeed give normal subgroups.
The first and last case represent the boring normal subgroups: $\{e\}$ and $G$. The case $1 + 3$ also represents a normal subgroup, which consists of all the products of all product of two disjoint two cycles and the identity:
$$V=\{e, (1 2)(3 4), (1 3)(2 4), (1 4)(2 3)\}.$$ The last case also corresponds to a normal subgroup which is $A_4$.
***
#### Example – Conjugacy Classes of $A_5$
Let us analyze the conjugacy classes of $A_5$. 
Since $A_5 \leq S_5$, we know that *if* two elements of $A_5$ are conjugate, *then* they have the same cycle type. But there is no reason for the converse to hold for observe that given $\a, \beta \in A_5$ of the same cycle type, the elements $\s \in S_5$ that give $\s \a \s^{-1} = \beta$ might all belong to $S_5 \setminus A_5$. Indeed, this does happen in some cases.
The possible cycle types of elements of $A_5$ are
1. five cycles, of which there are $4! = 24$, 
2. three cycles, of which there are ${5 \choose 3} 2 =   20$,
3. products of two disjoint transpositions, of which there are $5 \cdot 3 = 15$, and
4. $\{e\}$.
Let's start with five cycles. Let $\s = (1 \, 2 \, 3 \, 4 \, 5)$.  
We have by Theorem \ref{thm:conjclass} (a) that
$$C_{S_5}(\s) = \frac{S_5}{\left|\text{ conjugacy class of }\s \text{ in }S_5\right|}=\frac{5!}{4!}=5.$$
This yields  that the centralizer of $\s$ {\em in $S_5$} is
$$C_{S_5}(\s) = \{e, \s, \s^2, \s^3, \s^4\},$$
since the five listed permutations do commute with $\s$ and there can be no more elements in $C_{S_5}(\s)$ because of cardinality reasons. Moreover, it is obvious from the definitions that
$$C_{A_5}(\s) = C_{S_5}(\s) \cap A_5$$
and so we conclude that 
$$C_{A_5}(\s) = \{e, \s, \s^2, \s^3, \s^4\}$$
too. Thus, by LOIS, 
$$\text{ the size of the conjugacy class of \s in A_5} = [A_5: C_{A_5}(\s)] = 60/5 = 12.$$
That is, $\s$ is only conjugate in $A_5$  to half of the five cycles. 
If we pick a five cycle $\s'$ that is not conjugate in $A_5$ to $\s$, the same reasoning shows that $\s'$ is conjugate to exactly $12$ elements, which must be exactly the other $12$ five cycles. It is not hard to see that in fact $(1 \, 2 \, 3 \, 4 \, 5)$ and $(2 \, 1 \, 3 \, 4 \, 5)$ are not conjugate. In a bit more detail, they *are* conjugate in $S_5$ via the element $(1 \,2)$. From this one sees that the only elements $\a$ in $S_5$ such that
$$\a (1 \, 2 \, 3 \, 4 \, 5) \a^{-1} = (2 \, 1 \, 3 \, 4 \, 5)$$ holds are members of the coset $C_{S_5}(\s) \cdot (1 \, 2)$, which contains no elements of $A_5$.)
Given two three cycles $(a \, b \, c)$ and $(d \, e \, f)$, there is a $\s \in S_5$ such that
$$\s (a \, b \, c) \s^{-1}  = (d \, e \, f).$$
If $\s$ is not in $A_5$, then let $x,y$ be the two elements of $\{1, \dots, 5\} \setminus \{a,b,c\}$. Then we have
$$(\s \cdot (x \, y)) (a \, b \, c) (\s \cdot (x \, y))^{-1}  = (d \, e \, f).$$
and $\s \cdot (x \, y) \in A_5$. 
To figure out what's going on the in last case, set $\a = (1 \, 2)(3 \, 4)$. Because the cardinality of the conjugacy class of $\a$ in $S_5$ is 15 (it consists of all the products of two disjoint two-cycles) we get
$$15=|[\a]_{c\text{ in } S_5}|=[S_5: C_{S_5}(\a)]=\frac{120}{\left|C_{S_5}(\a)\right|}\Rightarrow \left|C_{S_5}(\a)\right| = 8.$$
Since
$$C_{A_5}(\a) = C_{S_5}(\a) \cap A_5,$$
it follows that $\# C_{A_5}(\a)$ must divide both $8$ and $60$, and so must be one of $1, 2$ or $4$.  Since $\a$ commutes with $e$, $\a$, $(1 \, 3)(2 \, 4)$ and $(1 \, 4)(2 \, 3)$ and each of these belongs to $A_5$, we must have 
$\# C_{A_5}(\a) = 4$. It follows that $\a$ is conjugate to $60/4 = 15$ elements -- i.e., $\a$ must be conjugate in $A_5$ to all elements of its cycle type. 
We conclude that  the conjugacy classes of $A_5$ are given by the following list:
1. the conjugacy class of $(1 \, 2 \, 3 \, 4 \, 5)$ has $12$ elements,
2. the conjugacy class of $(2 \, 1 \, 3 \, 4 \, 5)$ has $12$ elements, and this class is distinct from the previous one, 
3. the collection of all three cycles, of which there are $20$, forms a conjugacy class, 
4. the collection of all products of two disjoint transpositions, of which there are $15$, forms one conjugacy class, and
5. $\{e\}$ is a conjugacy class.
***
#### Example – Sylow and $D_{2p}$
In $D_{2p}$ for a prime $p$, $\langle r \rangle$ is a Sylow $p$-subgroup. If $p > 2$, there is only one Sylow $p$-subgroup of $D_{2p},$ so $n_p=1$. 
In $D_{2n}$ for $n$ odd, each of the subgroups $\langle sr^j \rangle$, for $j = 0, \dots, n-1$ is a Sylow $2$-subgroup, so $n_2=p$.
***
#### Example – Sylow and $S_5$
In $S_5$, the Sylow $5$-subgroups are the cyclic groups $\langle \sigma \rangle$ for any  five cycle $\sigma$, so $n_5=6$ because there are 24 five cycles, but there are four of these in every Sylow 5-subgroup. The Sylow $3$-subgroups are the cyclic groups $\langle \sigma \rangle$ for any three cycle $\sigma$, so $n_3=10$ because there are 20 three cycles, but there are two of these in every Sylow 3-subgroup. 
A Sylow $2$-subgroup of $S_5$ is any subgroup of order $8$. For example $\langle (1 \, 4)(2 \, 3) , (1 \, 2 \, 3 \, 4) \rangle$ is a Sylow $2$-subgroup. There are many others.
***
#### Example – Simple Groups and Element Counting
Let us prove that no group or order $12$ is simple.  Let $G$ be any group of order $12$. We will prove that $G$ must have either a normal subgroup of order $3$ or a normal subgroups of oder $4$.
Sylow theory gives that $n_2=|\Syl_2(G)|$ is either $1$ or $3$ and $n_3= |\Syl_3(G)|$ is either $1$ or $4$. If either of these numbers is $1$, we have a unique subgroup of order $4$ or of order $3$, and such a subgroup must be normal. Suppose these numbers are $3$ and $4$, respectively. We deduce a contradiction by "counting elements''. 
In detail, say $P_1, \dots, P_4$ are the $4$ Sylow $3$-subgroups. By Lagrange $P_i \cap P_j = \{e\}$ for all $i \ne j$. Thus the *set* $T := \bigcup_{i=1}^4 P_i$ has $9$ elements, one of which is $e$ and the other $8$ of which must have order $3$. That is, there are $8$ elements of order $3$ in $G$. But now consider the three Sylow $2$-subgroups $Q_1, Q_2, Q_3$. Each has order $4$ and $Q_i \cap T = \{e\}$ for all $i$. It follows that  $Q_i = \{e\} \cup (G \setminus T)$ for all $i$, and thus $Q_1 = Q_2 = Q_3$, a contradiction.
***
#### Example – Simple Groups and Conjugation
No group of order $80=5 \cdot 16$ is simple.
By way of contradiction suppose $G$ is
simple and $|G| = 80$. Sylow theory gives $|\Syl_2(G)| = 5$ and $|\Syl_5(G)| = 16$ (since they cannot be $1$ by the assumption that $G$ is simple). The "counting elements trick'' would work, but let's proceed in a different way: Consider the action of $G$ on $\Syl_2(G)$ by conjugation and let
$$\rho: G \to S_5$$
be the associated permutation representation (obtained by choosing a numbering $1, \dots, 5$ of the members of $\Syl_2(G)$). The map $\rho$ is non-trivial since the action is transitive by part (2) of the Sylow Theorem. But $80$ does not divide $120$ and so $\rho$ cannot be injective. It follows that $\ker(\rho)$ is a non-trivial, proper normal subgroup of $G,$ a contradiction.
***
#### Example – Direct Product and Isomorphism
If $\gcd(m,n)=1$ then $\Z/m\times \Z/n\cong \Z/mn$. Indeed consider the elements $x=(1,0)$ and $y=(0,1)$ in $\Z/m\times \Z/n$. Then $|x|=m, |y|=n$ and $x+y=y+x=(1,1)$. Therefore $|xy|=\lcm(|x|,|y|)=mn$. Since $\langle x+y \rangle \subseteq \Z/m\times \Z/n$ and both of these sets have cardinality $mn$ it must be the case that $\Z/m\times \Z/n=\langle x+y \rangle=\langle (1,1) \rangle$. Since $\langle x+y \rangle$ and $\Z/mn$ are both cyclic groups of order $mn$ they are isomorphic. Thus $$\Z/m\times \Z/n\cong \Z/mn.$$
***
#### Example – Trivial Homomorphism and Direct Product
Given $H$ and $K$ we could always take $\rho$ to be the trivial homomorphism, so that $\rho(y)(x) = x$ for all $y \in K$ and $x \in H$. Then $K \sdp_\rho H$ is just the usual direct product:
$$(y_1, x_1) (y_2, x_2) = (y_1 y_2, x_1 x_2).$$
***
#### Example – Normal Subgroups and Automorphisms
Fix a group $G$, a normal subgroup $H \nsg G$ and a subgroup $K \leq G$. Then the function
$$\rho: K \to \Aut(H)$$
given by $\rho(x)(y) = xyx^{-1}$ for $x \in K, y \in H$ is a homomorphism. Thus $K$ acts on $H$ via automorphisms.
***
#### Example – $D_{2n}$ and External Semidirect Products
Let $K = \langle x \rangle$ be cyclic of order $2$ and $H = \langle y \rangle$ be cyclic of order $n$ for any $n \geq 1$. There is an automorphism of $K$ that sends $y$ to $y^{-1}$. This automorphism is clearly its own inverse; i.e., it has order $2$. Therefore, by the UMP for cyclic groups, there is a group homomorphism
$$\rho: K \to \Aut(H)$$
with $\rho(x)(y) = y^{-1}$. We may thus form the group
$$G := H \sdp_\rho K.$$
The elements of $G$ are $(y^i, x^j)$ for $0 \leq i \leq n-1$ and $0 \leq j \leq 1$, in particular $|G|=2n$. Set
$$\tilde y = (y,e) \in G \text{ and } \tilde x = (e,x) \in G$$
Then
$$\tilde y^n = (y,e_K)^n = (y^n,e_K) = (e_H, e_K)= e_G$$
$$\tilde x^2 = (e_H,x)^2 = (e_H, x^2) = (e_H, e_K)= e_G$$
and
$$\tilde x \tilde y \tilde x \tilde y = (e_H,x)(y,e_K)(e_H, x)(y,e_K) = (\rho(x)(y),x)(\rho(x)(y),x) = (y^{-1},x)(y^{-1},x) = (y^{-1}y, e) = e_G.$$
Looks familiar!
Indeed, by the universal mapping property for $D_{2n}$ we have a homomorphism
$$\theta: D_{2n} \to G$$
such that $\theta(r) = (y,e_K)$ and $\theta(s) = (x,e_H)$. Moreover, $\theta$ is onto since 
$$\theta(r^is^j)=(y^i, x^j) \text{ for all } 0 \leq i \leq n-1, 0 \leq j \leq 1$$
and since $|D_{2n}|=|G|=2n$ it follows that $\theta$ is a bijection. So the dihedral group is a semidirect product, in which the two component groups are cyclic of orders $n$ and $2$ respectively:
$$D_{2n} \cong \langle y \rangle \sdp_\rho \langle x \rangle$$
and $\rho$ is the inversion homomorphism as described above. 
***
#### Exercise – Actions and Conjugations
If we identify $K$ with $K'$ and $H$ with $H'$ via the isomorphisms $i$ and $j$,  prove the action of $H'$ on $K'$ via conjugation in $K \sdp_\rho H$ coincides with the original action $\rho$.

###### Solution
***
#### Example – $D_{2n}$ and Internal Semidirect Products
Returning to $D_{2n}$, let $H = \langle s \rangle$ and $K = \langle r \rangle$. Then $H \leq G$, $K \nsg G$, $HK = G$ and $H \cap K =\{e\}$. So, $G$ is isomorphic to a semi-direct product, as we already showed.
***
#### Example – $S_n$ and Internal Semidirect Products (1)
Let $G = S_n$, $K = A_n$ and $H = \langle (1 \, 2) \rangle$. Then $K \nsg G$, $H \leq G$, $KH = G$ and $K \cap H  = \{e\}$. It follows that
$$S_n \cong A_n \sdp_\rho C_2$$
where $C_2 = \langle x \rangle$ is cyclic of order $2$ and the action $\rho: C_2 \to \Aut(A_n)$ sends $x$ to conjugation by $(1 \, 2)$. 
***
#### Example – $S_n$ and Internal Semidirect Products (2)
Let $G = S_n$ and $K = A_n$ again, but this time take $H' = \langle (1 \, 3) \rangle = (1 \,2 \, 3) \langle (1 \, 2) \rangle (1 \,2 \, 3)^{-1}$ (assuming $n \geq 3$). Then we get
$$S_n \cong A_n \sdp_{\rho'} C_2$$
where $C_2 = \langle x \rangle$ is cyclic of order $2$ and the action $\rho': C_2 \to \Aut(A_n)$ sends $x$ to conjugation by $(1 \,3)$.
The actions $\rho$ and $\rho'$ are not identical. For example, assuming $n\geq 4$ we have
$$\rho(x)(1 \, 2) (1 \, 2) (3 \, 4) = (1 \, 2) (3 \, 4) \text { maps } 1\mapsto 2$$
and
$$\rho'(x)(1 \, 2) (3 \, 4) = (1 \, 3) (1 \, 2) (3 \, 4) (1 \, 3) \text { maps } 1\mapsto 4.$$
Yet 
$$A_n \sdp_{\rho} H \cong
A_n \sdp_{\rho'} H'$$
since each is isomorphic to $S_n$.
On HW~8 you will give a more conceptual reason for why these two semidirect products turned out to be isomorphic: it is because  $H$ and $H'$ are conjugate in $S_n$. More generally, below is a criterion for a two semidirect products to be isomorphic.
***
#### Example – Groups of Order $6$
Any group of order $6$ is isomorphic either to $C_6$ or to $D_6$.
***
#### Example – Finitely Generated Infinite Groups
The following are finitely generated, but not finite groups:
- $\Z\cong F(\{x\})$
- $F(\{x_1,\ldots, x_n\})$ the free group on $n$ letters
- $\underbrace{\Z\times \dots \times \Z}_{r \text{ terms }}=\Z^r=\langle a_1,\ldots, a_r \mid a_ia_j=a_ja_i\rangle$ the free abelian group of rank $r$.
***
#### Example – Elementary Divisor Form
For $G\cong\Z/3\times Z/5\times Z/5$ we have $Q_1=\Z/3$, $Q_2=\Z/5\times Z/5$.
***
#### Example – Converting Elementary Divisors to Invariant Factors
Say I tell you
$$G \cong \Z^{3} \times \Z/4 \times \Z/8 \times \Z/9 \times \Z/27 \times \Z/25$$
The Chinese Remainder Theorem \ref{thm:CRT} gives 
$$\Z/8 \times \Z/27 \times \Z/25 \cong \Z/(8 \cdot 27 \cdot 25)$$
and
$$\Z/4\times \Z/9  \cong \Z/(4 \cdot 9)$$
so that
$$G \cong \Z^{3} \times \Z/(4 \cdot 9) \times \Z/(8 \cdot 27 \cdot 25).$$
Since $n_2:=(4 \cdot 9) \mid n_1:=(8 \cdot 27 \cdot 25)$, this is in invariant factor form, and hence the rank of $A$ is $3$ and the invariant factors of $A$ are $4 \cdot 9$ and $8 \cdot 27 \cdot 25$.
***
#### Example – Converting Invariant Factors to Elementary Divisors
Suppose now I tell you $$G \cong \Z^{4} \times \Z/6 \times \Z/36 \times \Z/180.$$ Then by the Chinese Remainder Theorem \ref{thm:CRT} $$G \cong \Z^{4} \times \Z/2 \times \Z/3 \times \Z/4 \times \Z/9 \times \Z/4 \times \Z/5 \times \Z/9,$$ given the elementary divisor form.
***
#### Example – Classifying Abelian Groups of Order $75$
Classify the abelian groups of order 75 up to isomorphism.
Let $G$ be an abelian group of order 75. Since $G$ is finite the rank of $G$ is $r=0$. Let's determine the possible elementary divisors $p_i^{a_{i,j}}$ so that 
$$G\cong \prod_{k=1}^s   \prod_{j=1}^{i_k} \Z/p_i^{a_{k,j}}.$$
The above equation gives $75=|G|= \prod_{k=1}^s\prod_{j=1}^{i_k}p_i^{a_{k,j}}$ and the possibilities for factoring $75$ as a product of prime powers are $75=3\cdot 5 \cdot 5$ or $75=3\cdot 25$ which gives 
$$G\cong \Z/25 \times \Z/3 \text{ or } G\cong \Z/5 \times \Z/5 \times \Z/3.$$
Note that the two groups above are not isomorphic. To see this, note that there is an element of order 25 in $\Z/25 \times \Z/3$, namely $([1]_{25},[0]_3)$ whereas every element $(a,b,c)\in \Z/5 \times \Z/5 \times \Z/3$ has order 
$$|(a,b,c)=\lcm(|a|, |b|, |c|)\leq 15$$
since $|a|, |b|\in\{1,5\}$ and $|c|\in\{1,3\}$.
Alternatively we could argue that the uniqueness of the FTFGAG tells us that $G$ uniquely determines the elementary divisors, so two groups with distinct elementary divisors cannot be isomorphic.
***
#### Exercise – Commutativity of Addition
Commutativity of addition is a consequence of the other ring axioms in rings with $1$.
#### Example – Ring Examples
1. $R=\{0\}$ is called the {\em trivial ring}. Notice that in the trivial ring $0=1$. Conversely, if $1 = 0$ in a ring, then $R = \{0\}$, since in this case for all $a$, we have $a \cdot 0 = 0$  and hence $a = a \cdot 1 = a \cdot 0 = 0$. 
2. $\Z$ is a commutative ring.
3. $\Z/n$ is a commutative ring under addition and multiplication modulo $n$. Note that $\Z/n$ is a field if any only if $n$ is prime.
4. The familiar sets of "numbers" $\Q, \R, \C$ are fields.
5. If $R$ is any ring (not necessarily commutative), so is $\M_{n}(R)$ for any natural number $n$, using the usual rules for addition and multiplication of square matrices.
6. Let $i,j,k$ be formal symbols and set $\bH$ to be the four dimensional $\bR$-vector space consisting of all expressions of the form $a + bi + cj + dk$ with $a,b,c,d \in \R$. Addition is vector space addition: $$(a + bi + cj + dk) +(a' + b'i + c'j + d'k) = (a + a') + (b + b') i + (c + c')j + (d + d')k.$$Multiplication is uniquely determined by the axioms of a ring together with the rules $$i^2 = j^2 = k^2 = -1, -ji = ij = k, -kj = jk = i, -ik = ki = j.$$and the fact that the real coefficients commute with each other and $i,j,k$. It's not obvious that the multiplication defined in this way satisfies associativity, but in fact it does (this amounts conditions very similar to the associativity of the group $Q_8$). $\bH$ is a division ring, since one can check that $$ (a + bi + cj + dk)^{-1} = \frac{a -  bi -  cj - dk}{\|a + bi + cj + dk\|}$$where $$\|a + bi + cj + dk \| := a^2 + b^2 + c^2 + d^2.$$In the equation above  $\|a + bi + cj + dk \|$ is non-zero real number if $a + bi + cj + dk$ is not the zero element. The quantity $\|a + bi + cj + dk \|$ is called the *norm* of the quaternion $a + bi + cj + dk$.
7. The cartesian product $R\times R'$ of two rings $R$ and $R'$ has a natural ring structure with addition and multiplication defined componentwise: $$(a,b)+(c,d)=(a+c,b+d)$$ $$(a,b)\cdot(c,d)=(a\cdot c,b\cdot d)$$
8. If $X$ is a set and $R$ is a ring, let $\Fun(X, R)$ be the collection of set theoretic functions from $X$ to $R$, and define $(f + g)(x) = f(x) + g(x)$ and $(f \cdot g)(x) := f(x) \cdot g(x)$. Then $\Fun(X,R)$ is a ring.  If $X$ is a finite set and $|X|=n$, then $\Fun(X,R)$ may be identified with $R^n=\underbrace{R \times \cdots \times R}_n$, the direct product of $n$ copies of $R$.
9. If $A = (A, +)$ is any abelian group, set $\End_{Ab}(A)$ to be the collection of endomorphisms of $A$ – that is, the set of group homomorphisms $f: A \to A$ from $A$ to itself. Then $\End_{Ab}(A)$ is a ring with addition $(f + g)(a) := f(a) + g(a)$ and multiplication $f \cdot g := f \circ g$. This is almost  always a non-commutative ring.
***
#### Example – Matrices and Units
$\Mat_{n}(F)^\times = \GL_n(F)$.
***
#### Example – Integral Domains
1. Every field is an integral domain (follows from the previous lemma).
2. $\Z/n$ is an integral domain if and only if $n$ is prime (in which case it happens to be a field too) or $n = 0$ (in which case $\Z/0\cong \Z$). 
***
#### Example – Subring Examples
- $\Z$ is a subring of $\Q$, which is a subring of $\R$, which is a subring of $\C$.
- $2\Z$ is a subring without $1$ of the ring $Z$ with $1$.
- The set of continuous functions  mapping $[0,1]\to \R$ is a subring of $\Fun([0,1],\R)$, denoted $\cC([0,1])$.
- The set $\Z[i]=\left\{a+bi\mid a,b \in \Z\right\}$ is a subring of $\C$ called the ring of Gaussian integers.
***
#### Exercise – Finding Subring Counterexamples
If $R$ is a ring and $S$ is a subring of $R$, it can happen that
1. $R$ is unital but $S$ is not (e.g. $S=2\Z\subset R= \Z$)
2. $S$ is unital but $R$ is not
3. both $R$ and $S$ are unital but $1_R\neq 1_S$
Find examples for each of these situations!

###### Solution
***
#### Exercise – Subring Preservations
Any subring of a commutative ring is a commutative ring. Any unital subring of an integral domain is an integral domain.

###### Solution
***
#### Example – Group Rings and $S_3$
Take $G = S_3$ and $R = \R$. Then $\R[S_3]$ is a six dimensional real vector space with basis $\{e, (1 \, 2), (1 \, 3), (2 \, 3), (1 \, 2 \, 3),  (1 \, 3 \, 2) \}$. An element is any expression of the form
$$r_1e + r_2  (1 \, 2) + r_3 (1 \, 3) + r_4 (2 \, 3) + r_5  (1 \, 2 \, 3) + r_6 (1 \, 3 \, 2)$$
where $r_1, \dots, r_6$ are real numbers. 
This ring has some zero divisors – for example
$$(e - (1 \, 2))(e + (1 \, 2)) = e - (1 \, 2) + (1 \, 2) - (1 \, 2)^2 = e - e = 0.$$
Here we are abusing notation a bit – for example, $- (1 \, 2)$ is really $(-1_R) (1 \, 2)$. In general, $1_R g$ is just written as $g$ in $R[G]$ and $(-r)g$ is just written as $- rg$, since $(-r)g$ is the additive inverse of $rg$.
***
#### Exercise –  $R[G]$ Commutative iff $G$ abelian
Let $R$ be any commutative ring and $G$ a group. Show $R[G]$ is commutative if and only if $G$ is abelian.

###### Solution
***
#### Example – Quaternions and Group Rings
Let $Q_8 = \{\pm 1, \pm i, \pm j, \pm k\}$ denote the group of quaternions and $\R$ the field of real numbers, and let us consider the group ring $\R[Q_8]$. Actually, the notation here is not so good since $(-1) k$ is easily confused with $1 (-k)$, and, even worse, things like $1 \cdot 1$, $1 \cdot (-1)$ are highly confusing. So, let us rename the elements of $Q$, so that $$Q_8 = \{e, e', i, i', j, j', k, k'\}$$so that $e$ is what we were writing as $1$, $e'$ is what we were writing as $-1$, $i'$ is what we were writing as $-i$, etc. So, for example, we now have $i^2 = e'$ in this group.
$\R[Q_8]$ is a non-commutative  ring, and you might guess that it is the same as the quaternions $\bH$ defined above, but it can't be: 
$\R[Q_8]$ is $8$-dimensional as a $\R$-vector space whereas $\bH$ is $4$ dimensional. In fact $\R[Q_8]$ is not a division ring, since it has zero divisors: $(e - i)(e + i + i^2 + i^3) =0$ and so neither of the two factors can be units.
The problem is that $(-1) e \in R[Q_8]$ is {\em not} the same thing as $1 e'\in R[Q]$, but we want them to be the same in $\bH$. 
Once we learn about quotient rings, we will be able to show that $\bH$ is the quotient of $R[Q_8]$ by the ideal generated by $e' + e$. Roughly this means we mod out by the relation $e' \sim -e$ and all consequences of this relation. For example, once one imposes this equivalence relation, the element
$$e + i + i^2 + i^3 = e + i + e' + e' i = (e + e') + i(e + e')$$ becomes the zero element. 
***
#### Example – Free Abelian Group and Group Rings
Group rings give lots of cool examples of rings, but we will now just focus on the boring case when $G$ is a free abelian group (written with multiplicative
notation) generated by $x_1, x_2, \dots, x_n$. In this case an element of $G$ may be written uniquely as $x_1^{e_1}, \dots, x_n^{e_n}$ for $e_1, \dots, e_n \in\Z$. For any commutative ring $R$ a typical element of $R[G]$ is thus $$\sum_{e_1, \dots, e_n \in \Z} r_{e_1, \dots, e_n} x_1^{e_1} x_2^{e_2} \cdots x_n^{e_n}$$
This is a *Laurent polynomial* in the variables $x_1, \dots, x_n$ with $R$-coefficients. 
Say $n = 1$ and let $x = x_1$, so that $G = \langle x \rangle$. Then $a x^{-3} + b x^{1} + c + dx^5$ with $a,b,c,d \in R$ is a representative example of an element of $R[G]$. Addition is by combining like powers of $x$. Multiplication is uniquely determined by the fact that it must satisfy the distributive law and $x^i x^j = x^{i +j}$ for $i, j \in \Z$.
***
#### Example – Basic Polynomial Ring
If $n = 1$, letting $x = x_1$, then $R[x]$ consists of all expressions of the form $\sum_{i=0}^\infty r_i x^i$ with $r_i = 0$ for all but a finite number of $i$.
***
#### Example – Ideal Examples
- In any ring $R$, $\{0\}$ and $R$ itself are ideals. 
- The ideals of $\Z$ are $n\Z$.
- The sets $R_i=\left\{\begin{bmatrix} 0 & 0 & \cdots & 0\\ \cdots & \cdots & \cdots & \cdots \\ a_{i1} & a_{i2} & \cdots &a_{in} \\  \cdots & \cdots & \cdots & \cdots \\  0 & 0 & \cdots &0\end{bmatrix}\right\}$ and $L_j=\left\{\begin{bmatrix} 0 & \cdots & a_{j1} &\cdots & 0\\ \cdots & \cdots & \cdots & \cdots \\0 & \cdots & a_{ji} &\cdots & 0\\ \cdots & \cdots & \cdots & \cdots \\ 0 & \cdots & a_{jn} &\cdots & 0\\\end{bmatrix}\right\}$ are a right ideal and a left ideal of $\M_n(R)$ respectively. Neither are two-sided ideals.
***
#### Exercise – Proper Ideals
An ideal $I$ is *proper* if $I\neq R$.  An ideal $I$ of a unital ring $R$ is proper if and only if $I$ contains no units.
Moreover, if $F$ is a field it has only two ideals $\{0\}$ and $F$.

###### Solution
***
#### Example – Generated Ideals and $\Z$
- In the commutative ring $\Z$, we have $(2,3)=(1)=\Z$. Indeed any element $n\in \Z$ can be written as $n=(-n)\cdot 2+n\cdot 3=n\cdot 1$. Note that $1=\gcd(2,3)$.
- In the commutative ring $\Z$, we have $(2,4)=(2)=2\Z$, the set of all even integers. Notice this shows that different sets can generate the same ideal. Also note that $2=\gcd(2,4)$.
- In $\Z[x]$, we have $(2,x)=\{a+xp(x) \mid a \text{ is even}, p(x)\in\Z[x]\}$ and this ideal cannot be generated by a single element.
***
#### Example – Principal Ideals
- every ideal of $\Z$ is principal with $I=(n)$ for some $n\in \Z$ ($\Z$ is a PID)
- for any field $F$, every ideal of $F[x]$ is principal ($F[x]$ is a PID)
- for any field $F$, every ideal in $F[x_1,\ldots,x_n]$ is finitely generated, but not necessarily principal. This is a consequence of a deep theorem called the Hilbert Basis Theorem, which you will see in Math 905.
***
#### Example – Quotient of $\Z$
If $I=(n)$ is an ideal in the ring $\Z$, then the quotient ring $\Z/(n)$ is the familiar ring $\Z/n$.
***
#### Exercise – Evaluation Homomorphism
If $R\subseteq S$ are commutative rings with $1\neq 0$ and $a\in S$, then the evaluation at $a$ function $\phi:R[x]\to S$ given by $\phi(f(x))=f(a)$ is a ring homomorphism.

###### Solution
***
#### Example – $\R[x]/(x^2+1)$
Here is a nice application of the First Isomorphism Theorem. Consider the ring $\R[x]$ and let $I = (x^2 + 1)$ be the principal ideals generated by $x^2+1$. Since $\R[x]$ is commutative, we have  $$(x^2 + 1) = \{ g(x)(x^2 + 1) \mid g(x)\in \R[x] \},$$ so $(x^2 + 1)$ is simply the collection of polynomials having $x^2 + 1$ as a factor. I claim that $\R[x]/(x^2 + 1)$ is isomorphic as a ring to $\C$. To prove this we define a map
$$\phi: \R[x] \to \C$$
sending $f(x)$ to $f(i)$, the evaluation of $f$ at $i$. It is easy to check $\phi$ is a ring homomorphism and it is onto since elements of the form $a + bx$ in the source map to all possible complex numbers under $\phi$.

We claim the kernel of $\phi$ is $(x^2 +1)$.  It is clear that $x^2 + 1 \in \ker(\phi)$ and it follows that $(x^2 + 1) \subseteq \ker(\phi),$ since $\ker(\phi)$ is a two-sided ideal.

Suppose $\phi(f(x)) = 0$ and write $f(x) = (x^2 + 1)q(x) + r(x)$ with degree of $r(x)$ at most one, using the division algorithm in the polynomial ring $\R[x]$. So $r(x) = a + bx$ for real numbers $a,b$. If $r(x) \ne 0$, then $r(i) \ne 0$, which would contradict $f(i) = 0$. So we must have $r(x) = 0$ and hence $f(x) \in (x^2 +1)$.
Applying the First Isomorphism Theorem for Rings, we get $$\R[x]/(x^2+1) \cong \C$$via the map sending $f(x) + (x^2 + 1)$ to $f(i)$.
Intuitively, we have adjoined a formal symbol $x$ to the real numbers, and by modding out $x^2 + 1$ we have forced $x$ to be a square root of $-1$. That is, we have adjoined $i$ to the real numbers, obtaining $\C$.
***
#### Example – Ideal of $\Z[x]$ and Isomorphism
Consider the ideal $J = (2, x^2 + x + 1)$  of $\Z[x]$. Explicitly, by Lemma \ref{lem:idealgen} we have $$J =\{ p(x)\cdot 2 + q(x)(x^2 + x+ 1) \mid p(x),q(x)\in\Z[x]\}.$$ Suppose we want to understand $\Z[x]/J$. Then the Third Isomorphism Theorem is our friend. Set $I=(2)$ and note that $I \subseteq J$, and so by the Third Isomorphism Theorem
$$\Z[x]/J \cong \frac{\Z[x]/I}{J/I}.$$
Next we express both the numerator and the denominator in better terms. I claim
$$\Z[x]/I =\Z[x]/(2) \cong (\Z/2)[x].$$
To see this consider the reduction homomorphism $\rho: \Z[x] \to (\Z/2)[x]$ sending a polynomial $p(x)$ to its reduction modulo $2$. The kernel of this surjective ring map is $I$, establishing our claim by the First Isomorphism Theorem.

Recall that $J/I$ denotes the image of $J$ under the quotient map $\pi:\Z[x]\to \Z[x]/I$.
Therefore we have
$$\begin{eqnarray*}
J/I &=\pi(J)=\{\pi( p(x) \cdot 2 + q(x)(x^2 + x+ 1)) \mid  p(x),q(x)\in\Z[x]\}\\
&=\{\pi( p(x)) \cdot \pi(2) + \pi(q(x))\pi(x^2 + x+ 1)) \mid  p(x),q(x)\in\Z[x]\}\\
&=\{\pi( p(x)) \cdot 0 + \pi(q(x))\pi(x^2 + x+ 1)) \mid  p(x),q(x)\in\Z[x]\}\\
&=\{ f(x)\pi(x^2 + x+ 1)) \mid f(x)\in\Z[x]/I\}=\left((x^2+x+1)+I\right).
\end{eqnarray*}$$
In other words, J/I is the ideal generated by the coset of x^2+x+1 in Z[x]/(2).
Moreover, under the isomorphism $\bar\rho:\Z[x]/I \to (\Z/2)[x]$ discussed above, we have that $f(x)+I\mapsto \ov{f}(x)$, where $\ov{f}(x)$ denotes the reduction of the coefficients of $f$ modulo 2. Therefore $\bar \rho(J/I)=([1]x^2+[1]x+[1]),$ where $[1]$ denotes the congruence class of $1$ modulo 2.
Now we put everything together: consider the ring homomorphism $\varphi=\pi'\circ \bar \rho$ where
$$\Z[x]/I\stackrel{\bar \rho}{\rightarrow}(\Z/2)[x] \stackrel{\pi'}\rightarrow \frac{(\Z/2)[x]}{([1]x^2+[1]x+[1])}.$$
Notice that since $\bar\rho$ and $\pi'$ are surjective, so is $\varphi$, thus $\im(\varphi)=\frac{(\Z/2)[x]}{([1]x^2+[1]x+[1])}$ and 
$$\ker(\varphi)=\ker(\pi'\circ \bar \rho)=\ker(\pi')=([1]x^2+[1]x+[1])$$
since $\bar\rho$ is an isomorphism and $\pi'$ is a quotient map. Applying the First Isomorphism Theorem to $\varphi$ gives
$$\frac{\Z[x]/I}{J/I}\cong \frac{(\Z/2)[x]}{([1]x^2+[1]x+[1])}$$
and combining this with the Third Isomorphism Theorem further yields
$$\Z[x]/J \cong \frac{(\Z/2)[x]}{([1]x^2+[1]x+[1])}.$$
***
#### Example – Ideal and LIT
It turns out that the ring $F=\frac{(\Z/2)[x]}{([1]x^2+[1]x+[1])}$ we discussed in the previous example is a field and by a problem from HW 11, any field $F$ has only two ideals $(0)$ and $F$ itself. This implies via the Lattice Isomorphism Theorem that there are only two ideals in  $(\Z/2)[x]$ which contain $([1]x^2+[1]x+[1])$, namely $([1]x^2+[1]x+[1])=\pi^{-1}(0)$ and $(\Z/2)[x]=\pi^{-1}(F)$.
***
#### Exercise – Prime iff Complement Closed
An ideal $P$ is prime if and only if $R \setminus P$ is closed under multiplication.

###### Solution
***
#### Example – Prime Ideals
- In $\Z$, the prime ideals are $(0)$ and the ideals generated by prime integers $P=(p)$, where $p$ is a prime integer. The maximal ideals are the ideals generated by prime integers. In particular $(0)$ is prime but not maximal.
- In $\Z[i]$ the ideal $(13)$ is not prime, because $13=(3+2i)(3-2i)\in(13)$, but $3+2i\not \in (13)$ and  $3-2i\not \in (13)$ (because if $3\pm2i=13\a$ then $N(3\pm2i)=N(13)N(\a)$ so $13=13^2N(\a)$, a contradiction).
- In $\Z[x]$ the ideal $(2,x)$ is maximal and prime (proof in the example given later), the ideals $(2)$ and $(x)$ are prime but not maximal.
***
#### Exercise – In Domain, Kernel of Homomorphism Prime
If $R$ is a domain, $S$ is a ring and $f:R\to S$ is a ring homomorphism, then $\ker(f)$ is a prime ideal.

###### Solution
***
#### Example – $\Z[x]$ and $(2,x)$
We show that in $\Z[x]$ the ideal $(2,x)$ is maximal. For this we consider the quotient ring $\Z[x]/(2,x)$. By the Third Isomorphism Theorem, and because $\Z[x]/(x)\cong\Z$ and under this isomorphism $(2,x)/(x)$ is mapped to $(2)$, we have (omitting some details) $$\frac{\Z[x]}{(2,x)}\cong\frac{\Z[x]/(x)}{(2,x)/(x)}\cong\Z/2, \text{ a field}.$$ Since the quotient ring is field, we conclude that $(2,x)$ is maximal.
***
#### Example – The Trivial Norm
A "degenerate'' example is a field $F$ equipped with the trivial norm $N(r) = 0$ for all $r$. Given $a,b \in F$ with $b \ne 0$, we have $a =(ab^{-1})b + 0$.
Note that in this example there is no need to include "$r=0$'' in the description of the division algorithm, since $b \ne 0$ implies $|0| < |b|$. This is not the case in other examples. Also observe that as we've defined remainders they are {\em not} unique. For example, in dividing $13$ by $5$, both $$13 = 2 \cdot 5 + 3 \text{ and } 13 = 3 \cdot 5 + (- 2)$$ are considered valid.
This calculation shows, more generally, that if $b$ is a unit, then for all $a$ there exists an equation $a = bq + r$  with $r = 0$, not matter what norm $N$ is used.
One could make remainders (and hence quotients) unique for $\Z$ by insisting that remainders always be non-negative, but this is not part of the abstract theory since it doesn't generalize to all cases well.
***
#### Example – The Gaussian Integers are an ED
The ring $R = \Z[i]$ of Gaussian integers is a Euclidean domain with $N$ being the usual complex (Euclidean) square norm $N(a+bi)=a^2+b^2$.
Let $\alpha$, $\beta$  $\in \Z[i]$ and let $\frac{\alpha}{\beta}=p+qi \in \Q(i)$ (here we use that the fraction field of $\Z[i]$ is $\Q(i)$). Now pick $s,t\in\Z$ so that $|p-s|\leq 1/2$ and $|q-t|\leq 1/2$. We have
$$\a=\beta(s+ti)+\beta(p+qi)-\beta(s+ti).$$
Set $q=s+ti$ and set $r=\beta(p+qi)-\beta(s+ti)=\beta(s+ti-(p+qi))$ and notice that $q\in \Z[i]$ because $s,t\in\Z$ and $r\in \Z[i]$ by closure. If $r=0$ we're good, and if $r\neq 0$ then, using that the complex squared norm is multiplicative as well as the Pythagorean Theorem and the choice for $s,t$, we have
$$N(r)=N(\beta(s+ti-(p+qi)))=N(\beta)N(s+ti-(p+qi))\leq N(\beta)\cdot(1/4+1/4)<N(\beta).$$
Thus the norm function $N$ makes $\Z[i]$ into a Euclidean domain.
***
#### Example – Degree and Norm
The next classical example is $R = F[x]$ with $F$ a field and where we define the norm to be degree: $N(f(x)) = \deg(f(x))$ if $f\neq 0$ and $N(0)=0$. This ring is a ED because of the familiar long division  for polynomials.
***
#### Example – PID not ED
The ring $\Z\left[ \frac{1 + \sqrt{-19}}{2}\right]=\left\{a+ b\frac{1 + \sqrt{-19}}{2} \mid a,b\in \Z\right\}$ is a PID, but not a Euclidean domain. It is the simplest example of such a ring, but the proofs of these claims are not easy. I will not cover a proof of this fact.
***
#### Example – Prime and Irreducible Elements
- the prime elements of $\Z$ are the prime integers and their negatives; they are also irreducible
- any element $\a\in Z[i]$ with $N(\a)$ a prime integer is irreducible e.g. $\a=1+2i$ is irreducible
- the element $13=(2+3i)(2-3i)$ is not irreducible in $\Z[i]$
- the polynomial $x^2+x+[1]\in (\Z/2)[x]$ is irreducible; indeed if it factors nontrivially, it must factor as a product of two linear polynomials: $x^2+x+[1]=(x+[a])(x+[b])$. Then $-[b]$ is a root for $x^2+x+[1]$. But neither $[0]$ nor $[1]$ are roots for this polynomial, a contradiction.
***
#### Example – In $\Z[\sqrt{-5}]$, $2$ Irreducible but not Prime
In the domain $\Z[\sqrt{-5}]$ the element $2$ is irreducible but not prime. Note that $2\cdot 3=(1+\sqrt{-5})(1-\sqrt{-5})$ and thus $(1+\sqrt{-5})(1-\sqrt{-5})\in (2)$. However we claim that neither $1+\sqrt{-5}$ nor $1-\sqrt{-5}$ are in $(2)$. If $\a=1\pm\sqrt{-5}\in (2)$ then $\a=2\beta$ for some $\beta\in  \Z[\sqrt{-5}]$ and so  $6=N(\a)=N(2)N(\beta)=4N(\beta)$, a contradiction. Thus $2$ is not prime.
***
#### Example – $\C[x,y]/(x^2-y^3)$, $y$ Irreducible but not Prime
In the ring $\C[x,y]/(x^2-y^3)$ the element $y$ is irreducible but not prime.
Since  $\C[x,y]/(x^2-y^3)\cong \C[t^3, t^2]\subseteq \C[t]$ this ring is a domain. The element $y$ is irreducible for degree reasons. The ideal $(y)$ contains $x^2$ but doesn't contain $x$ so $y$ is not prime.
***
#### Example – UFD Examples
- $\Z$ is a UFD by the Fundamental Theorem of Arithmetic.
- $F[x]$ where $F$ is a field is a UFD. This is the case because $F[x]$ is a Euclidean domain and Euclidean domains are UFD's (we'll prove this shortly).
- We will eventually prove that if $R$ is a UFD then so is $R[x]$. It follows that $F[x_1, \dots, x_n]$ is a UFD for all $n$. Note that if $n > 1$, this ring is not a PID and hence not a Euclidean domain.
***
#### Example – $\Z[x]$ not a PID
$\Z[x]$ is not a PID hence also not a Euclidean domain. For example, this can be seen because the ideal $(2,x)$ is not a principal ideal. It is a UFD because $\Z$ is a UFD (based on the result that if $R$ is a UFD then so is $R[x]$ which we will prove shortly).
***
#### Example – $\Z[\sqrt{-5}]$ not a UFD
$\Z[\sqrt{-5}]$ is a domain that is not a UFD, as $6=(1 + \sqrt{-5}) (1 - \sqrt{-5})=2\cdot 3$ and each of $1 + \sqrt{-5},1 - \sqrt{-5},2, 3$ are irreducible by a norm argument (exercise).
Notice also that $\Z[\sqrt{-5}]$ contains elements that are irreducible but not prime: $2$ is irreducible, by a norm argument. But it is not prime since $(1 + \sqrt{-5}) (1 - \sqrt{-5})  \in (2)$ but neither $1 + \sqrt{-5}$ nor $1 - \sqrt{-5}$ is in $(2).$
***
#### Example – The Evaluation Ring Homomorphism
Suppose the ring map $\phi$ is the inclusion of a subring $R$ into a commutative ring $S$, including even the case $R = S$.
Given $s_1, \dots, s_n \in S$. Then the map
$$\tilde{\phi}: R[x_1, \dots, x_n] \to  S$$
can be thought of as evaluation of polynomials in $x_1, \dots, x_n$ at $s_1, \dots, s_n$. 
***
#### Example – Applying Ring Homomorphism to Coefficients
Given a ring map $\phi: R \to S$ between commutative rings, we may apply the Proposition to the composition
$R \xra{\phi} S \hookrightarrow S[x]$ using the element $s = x$ of $S[x]$ to get an induced ring map
$$\tilde{\phi}: R[x] \to S[x]$$
that sends $\sum_i r_i x^i$ to $\sum_i \phi(r_i) x^i$. That is, the map $\tilde{\phi}$ applies $\phi$ to the coefficients of a polynomial.
This can be generalized to more than one variable in the obvious way.
***
#### Example – The Reduction Homomorphism
Continuing with the previous example, we could have $S = R/I$ for an ideal $I$ of $R$ and $\phi$ could be the quotient map. Then
$$\tilde{\phi}: R[x_1, \dots, x_n] \to (R/I)[x_1, \dots, x_n]$$
takes a polynomial and "reduces'' its coefficients modulo $I$.
We will usually denote the image of $f(x)$ through the reduction homomorphism by $\ov{f}(x)$.
***
#### Example – Multiplicatively Closed Sets
Two types of multiplicatively closed sets are most commonly used in practice:
- If $R$ is a field then $S=R\setminus \{0\}$ is a multiplicatively closed set of non zero divisors.
- If $R$ is an arbitrary ring with $1\neq 0$ and $x\in R$ is a non zero divisor then the set of non negative powers of $x$, $S=\{x^n \mid n\in \Z, n\geq 0\}$, is multiplicatively closed.
###### Solution
***
#### Example – Fields of Fractions
- For a specific example, the field of fractions of $\Z$ is of course $\Q$. 
- For another, if $d$ is a squarefree integer and $R = \Z[\sqrt{d}]$ is an integral domain and we will show soon that its field of fractions is (isomorphic to) the field $\Q(\sqrt{d})$.
- For yet another, $\R[x]$ is an integral domain. Its field of fractions, usually denoted $\R(x)$ consists of all *rational functions*. This last example could be generalized by replacing $\R$ with any field and also by using any number of variables.
***
#### Exercise – Opposite Ring
Given a ring $R$, let $R^{op}$, the 'opposite ring',  denote the same set with same rule for $+$, but with multiplication redefined as $a \cdot_{op} b := b a$ (where $ba$ on the right is the original multiplication ring). Then $R^{op}$ is also a ring – note that it coincides with $R$ if and only if $R$ is commutative. Given a left $R$-module $M$, show that $M$ is a right $R^{op}$-module via the rule for scaling given by $m r := rm$.

###### Solution
***
#### Example – Modules
- For any $R$, the trivial module is $0=\{0\}$ with $r0=0$ for any $r\in R$.
- Every ring $R$ is a left module over itself whit the rule for scaling given by the ring multiplication rule. It is also a right module over itself. 
- More generally, if $R$ is any ring and $I$ is a left ideal, then $I$ is a left-$R$-module.
- Let $F$ be a field and $R = \Mat_{n \times n}(F)$ (the ring of $n \times n$ matrices with entries in $F$). Let $M$ be the collection of column vectors with entries in $F$ having $n$ entries. The usual rules for adding column vectors and multiplying column vectors on the left by matrices make $M$ into a left $R$-module. Likewise if $N$ is the collection of all row vector with $n$ entries in $F$, the $N$ is a right $R$-module via addition and matrix multiplication.
***
#### Example – Standard Free Module
For a non-negative integer $n$, the  "standard'' free (left) $R$-module of rank $n$ is the set
$$
R^n=\left\{\begin{bmatrix} r_1\\ \vdots \\r_n \end{bmatrix} \mid r_i\in R, 1\leq i\leq n\right\}
$$
equipped with the operations
$$
\begin{bmatrix} r_1\\ \vdots\\r_n \end{bmatrix} +\begin{bmatrix} r'_1\\ \vdots\\r'_n \end{bmatrix} =\begin{bmatrix} r_1+r'_1\\ \vdots\\r_n +r'_n\end{bmatrix} \text{ and }
r\begin{bmatrix} r_1\\ \vdots\\r_n \end{bmatrix}=\begin{bmatrix} rr_1\\ \vdots\\ rr_n \end{bmatrix}. 
$$
***
#### Example – Complex Vector Spaces
For example, since $\R$ is a subring of $\C$, every complex vector space may be regarded as a real vector space, by restriction of scalars from $\C$ to $\R$. Likewise, any real vector space may be regarded as a rational vector space. Etc. 
***
#### Example – Homomorphisms and Restriction of Scalars
If $S$ and $R$ are rings and $\phi: S \to R$ is a ring homomorphism, then since $S$ is a left $S$-module,
it is also a left $R$-module via restriction of scalars. Note that the rule for scaling given by $r s := \phi(r) s$. 
As a special case of this, if $S$ is a subring of a ring $R$ then $R$ is an $S$-module (restriction of scalars along the inclusion map).

For instance, $R[x_1,\ldots,x_n]$ is a left $R$-module for any $n\geq 0$ via the evident injective ring homomorphism $R \into R[x_1, \ldots, x_n]$. 

Also, 
$\Mat_{n \times n}(R)$ is a left $R$-module for $n\geq 1$ given by the ring map $R \to \Mat_{n \times n}(R)$
  sending $r$ to $r \cdot I_n$. 
***
#### Example – $R/I$-Module and Restriction of Scalars 
- If $I$ is a (two-sided) ideal of a ring $R$ then applying restriction of scalars along the quotient homomorphism $q:R\to R/I$ gives that any left $R/I$-module is also a left $R$-module.  
- In particular, applying this to the $R/I$-module $R/I$ gives that $R/I$ is a left $R$-module. The rule for scaling is $r \cdot (r' + I) = rr' + I$. 
***
#### Example – Submodules are Ideals
A subset $I$ of a ring $R$ is a left submodule of $R$ if and only if it is a (left) ideal.
***
#### Example – Cyclic $\Z$-module
If $R = \Z$, then (recalling that a $\Z$-module is the same thing as an abelian group) we see that $M$ is a cyclic $\Z$-module if and only if $M$ is a cyclic group.
***
#### Example – Standard Free Module Finitely Generated
Let $R$ be a ring.
- The standard free $R$-module of rank $n$, $R^n$, is finitely generated, since it is generate by $e_1, \dots, e_n$ where $e_i := $\begin{bmatrix} 0 \\ \vdots \\ 0 \\ 1 \\  0 \\ \vdots \\ 0 \end{bmatrix}$, with a $1$ in the $i$-th position. This holds since given any element $v = \begin{bmatrix} r_1 \\ \vdots \\ r_n\end{bmatrix}$ of $R^n$ we have $v = \sum_i r_i e_i$. 
- In particular, taking $n = 1$, $R$ is cyclic as a module over itself, since $R = R \cdot 1$.
- More generally, for any (two sided) ideal $I$, $R/I$ is a cyclic left $R$-module, generated  by $\ov{1}$. 
***
#### Example – One Element Subsets of $R$-Modules
A one element subset $\{m\}$ of an $R$-module $M$ is linearly independent if and only if whenever $rm =0$, we have $r = 0$. 
But it is possible for one elements subsets to be linearly dependent: For example, let $R$ be any ring and $I$ and (two-sided) ideal such that $I \ne 0$.
Then I claim that every non-empty subset of $M = R/I$ is linearly dependent. For say $A$ is a such a nonempty subset. For any $a \in A$, pick any $r \in I$ such that $r \ne 0$. Then $ra = 0$ (since $a = y + I$ for some $y \in R$ and hence $ra = ry + I = I = 0_M$) and this shows $A$ is linearly dependent. In particular, even a one-element subset of $M$ is linearly dependent. 
***
#### Example – $\{3\}$ Linearly Independent in $\Z$ 
The singleton $\{3\}$ is a linearly independent subset of the $\Z$-module $M = \Z$. But it does not generate of $M$. The subset $\{3, 5\}$ does generate all of $M$, but it is not linearly independent, since $5 \cdot 3 + (-3) \cdot 5 = 0$. More on this later.
***
#### Example – Bases and Free Modules
Let $R$ be any ring.
- The zero module is free with $\emptyset$ as (its only) basis. This holds since the empty is vacuously linearly independent and it generates $\{0\}$. 
- $R$ is free since $\{1\}$ is a basis for $R$. It clearly generates and if $r \cdot 1 = 0$ then $r = 0$, so it is linearly independent. 
- More generally, $R^n$ is free since $e_1, \dots, e_n$ is a basis. This is called the "standard basis'' of $R^n$. We've already seen that $e_1, \dots, e_n$ generates $R^n$ as an $R$-module. Suppose $\sum r_i e_i = 0$. Then  $\begin{bmatrix} r_1 \\ \vdots \\ r_n \end{bmatrix} = \begin{bmatrix} 0 \\ \vdots \\ 0 \end{bmatrix}$ and hence $r_i = 0$ for all $i$. 
- As we shall prove later, every vector space over a field is free.
- For any ring $R$, if $I$ is a (two-sided) ideal such that $I \ne 0$ and $I \ne R$, then $M = R/I$ is not free. Since $I \ne R$, $R/I$ is not the zero module and hence the empty set isn't a basis. Let $A$ be any non-empty subset. Then since $I \ne 0$, as shown above $A$ is linearly dependent. We conclude that no subset of $M$ is a basis.
***
#### Example – Bases are not Unique
As you likely know from a class in linear algebra, bases of free modules are rarely unique. Indeed, if $R$ is any ring,  then any single unit forms a basis for $R$ as a module over itself. For another example, for any ring $R$ and any fixed element $r \in R$, the set
$$\left\{ \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \begin{bmatrix} r \\ 1 \end{bmatrix} \right \}$$ forms a basis for the free $R$-module $R^2$.
***
#### Example – Module with Infinite Basis
I have not yet given an example of a module with an infinite basis; here is one. Let $R$ be any ring and $M = R[x]$ (which, recall, is an $R$-module due to the evident ring map $R \to R[x]$). Then the countably infinite set $\{1,x,x^2,\dots, x^n,\dots\}$ is a basis. The fact that this set is a basis is essentially part of the definition of $R[x]$. The Lemma says that every polynomial is uniquely expressible as an $R$-linear combination
of (a finite subset of) $1,x,x^2,\dots$.
***
#### Example – $M\cong R^n$ as $R$-modules
If $M$ is a free $R$-module that has a basis of cardinality $n$, then $M \cong R^n$ as $R$-modules.
This holds since, as seen above, $R^n$ has a basis of cardinality $n$, namely the standard basis $e_1, \dots, e_n$.

More precisely, as the proof makes clear,
if $B = \{x_1, \dots, x_n\}$ is an (ordered) basis of $M$, there is an 
isomorphism $\phi_B: R^n \cong M$ that sends $\begin{bmatrix} r_1 \\ \vdots \\ r_n \end{bmatrix}$ to $\sum_i r_i x_i$. 
***
#### Example – $\Z$-modules and Quotients
Recall that $\Z$-modules are the same as abelian groups. Submodules and quotient $\Z$-modules are the same things as subgroups and quotients
of abelian groups.  
***
#### Example – Maximal Ideals and Vector Spaces
Suppose $I$ is a maximal ideal of a commutative ring $R$. Then $R/I$ is a field, and given an $R$-module $M$, $M/IM$ is a module over the field $R/I$; i.e., it is a vector space over this field. Moreover, if $f:  M \to N$ is an $R$-map then $\ov{f}: M/IM \to N/IN$ is an $R/I$-linear transformation.
***
#### Example – $R$ has a basis as a $\Q$-Vector Space
$\R$ has a basis as a $\Q$-vector space. Just don't ask me what it looks like.
***
#### Example – Maximal Ideals in Commutative Rings
As a reminder, one can use Zorn's Lemma to prove that every non-zero commutative ring has a maximal ideal. Let me sketch the proof: Let $\cA$ be the collection of proper ideals of a non-zero commutative ring $R$, regarded as a poset under containment.
Let us verify Zorn's Lemma applies to $\cA$: It is non-empty since $\{0\} \in \cA$ and $\{0\} \ne R$. Let $\cB$ be a totally ordered subset of $\cA$. If $\cB$ is empty, then $\cB$ is bounded above by $\{0\}$ (or any other member of $\cA$.) Assume $\cB$ is non-empty.  Let $I = \bigcup_{J \in \cB} J$.
I claim that $I$ is an ideal: It is non-empty since $\cB$ is non-empty. It is clear it is closed under scaling. Given $a, b\in I$ we have $a \in J$ and $b \in J'$ for some $J, J' \in \cB.$ Since $\cB$ is totally ordered, either $J \subseteq J'$ or $J' \subseteq J$. In the former case $a + b \in J' \subseteq I$ and in the latter $a+b \in J\subseteq I$.This proves $I$ is an ideal. $I$ is proper since if $1 \in I$ then $1 \in J$ for some $J \in \cB$ which is not possible. So, $I \in \cA$ and clearly $\cB$ is bounded above by $I$. We may thus apply Zorn's Lemma which gives that $\cA$ has at least one maximal element.
***
#### Example – Dimension of $F^n$ in $F$
$\dim_F(F^n)=|\{e_1,e_2,\dots,e_n\}|=n.$
***
#### Example – SubLemma and $\R^3$
For a visual interpretation of the sublemma, suppose $V = \R^3$ and $B =\{i,j,k\}$ is its standard basis.  Given $w \in\R^3$, if $w$ is a non-zero multiple of one of the members of $B$, say $w = r i$ for $r \ne 0$, then $\{w, j , k\}$ is also basis of $\R^3$.
If $w$ lies one of the coordinate planes but is not on a axis, say $w = ri + s j$ for $r, s \ne 0$, then both $\{w,j,k\}$ and $\{i,w,k\}$ are bases. If $w$ lies on none of the coordinate planes, then $w = ri + s j + tk$ for $r, s, t \ne 0$ and each of $\{w,j,k\}$, $\{i,w,k\}$ and $\{i,j,w\}$ is a basis. 
So, the sublemma is saying that we can swap in $w$ for any of the basis elements that occur with a non-zero coefficient in the unique expression of $w$ as a linear combination of the basis. (This includes the case when $w = 0$, since no such basis vectors occur.)
***
#### Example – $\R^\N$
Consider $V = \R^\N=\R\times \R\times \R \times \dots$, and define rules for addition and scaling degree-wise in the evident way.

It is not hard to see $V$ is a $\R$-vector space. It can be identified with the collection of all 
sequences $\{a_n\}$ of real numbers. One might be interested in a basis for this vector space. At first glance the most obvious choice would be $E=\{e_1,e_2,\ldots\}$, where $e_i$ is the sequence with a $1$ in the $i$-th position and $0$'s everywhere else. 

However, this set does not span $V$ as $v = (1,1,\ldots)$ can not be represented as a finite linear combination of these elements. (It turns out that $E$ is the basis for the direct sum $\bigoplus_{i\in \N}\R$, which may be identified with all sequences having only a finite number of non-zero terms.) 

Now, since we know since $v$ is not in $\Span(E)$, we have that $E \cup \{v\}$ is a linearly independent set. However, this does not span either as $(1, 2, 3, 4, \dots)$ is not in the span of this set. We know that $V$ has a basis, but it can be shown that no countable collection of vectors forms a basis for this space, in fact $\dim_\R \R^\N =|\R|$. An explicit basis of this vector space is impossible to describe.
***
#### Example – $\R$-Vector Space of Polynomials ($P_n$)
Let $P_n$ denote the the $\R$-vector space of polynomials of degree at most $n$ (including the zero polynomial) and consider the linear transformation $\phi :P_3\to P_2$ given by $\phi(f)=f'$, i.e. taking the derivative. Take $B=\{1,x,x^2,x^3\}$  for an ordered basis of $P_3$ and $C = \{1,x,x^2\}$ for an ordered basis of $P_2$.
Then for $p(x) = 5 + 3x + 2x^2 - 7x^3$ we have
$$
[p(x)]^B = \begin{bmatrix} 5 \\ 3 \\ 2 \\ -7\end{bmatrix}
$$
and
$$
[\phi]_B^C= 
\begin{bmatrix}
0 & 1 &0 & 0 \\
0 &0 & 2 & 0 \\
0& 0& 0& 3 \\
\end{bmatrix}.
$$
We have 
$$
[\phi]_B^C \cdot [p(x)]^B =  
\begin{bmatrix} 3 \\ 4 \\ -21 \end{bmatrix} = [p'(x)]^C = [\phi(p(x))]^C
$$
confirming in this example one of the assertions of the Lemma.

Let $\psi: P_2 \to P_3$ be the linear map $\psi(q(x)) = \int_0^x q(t) \, dt$.
Then
$$
[\psi]_C^B= 
\begin{bmatrix}
0 & 0 &0  \\
1 & 0 & 0 \\
0& 1/2&  0 \\
0 & 0  & 1/3 \\
\end{bmatrix}.
$$
Note that
$$
[\phi]_B^C \cdot [\psi]_C^B = I_3  = [\phi \circ \psi]_C^C
$$
and
$$
[\psi]_C^B \cdot [\phi]_B^C =
\begin{bmatrix}
0 & 0 &0 &0 \\
0 & 1 & 0 &0\\
0& 0& 1& 0 \\
0 & 0  & 0 & 1\\
\end{bmatrix} = [\psi \circ \phi]_B^B
$$
as predicted by \eqref{E218}.
***
#### Example – Identity Automorphism of Free $R$-Module
If $\id_V: V \to V$ is the identity automorphism of an $n$-dimensional free $R$-module $V$, then for any basis $B$ of $V$ we have $\id_V(b_i) = b_i$ for all $i$ and hence
$$
[\id_V]^B_B = I_n.
$$
***
#### Example – CoB Matrix and Standard Free Module
Say $V = R^n$, $B$ is the standard basis (so $b_i$ is a column vector with a $1$ in the $i$-th position and $0$'s elsewhere). Note that $[v]^B = v$ for all $v$. 

Let $B' = \{b'_1, \dots, b'_b\}$ be any other basis of $V$. Then $[b'_i]^B = b_i$ and so the change of basis matrix $[\id_V]_{B'}^{B}$ satisfies, on the one hand, $$[\id_V]_{B'}^{B} [b'_i]^{B'}=[\id_V]_{B'}^{B} b_i = \text{the $i$-th column of $[\id_V]_{B'}^{B}$}$$ and, on the other hand, $$[\id_V]_{B'}^{B} [b'_i]^{B'}=[b'_i]^B  = b'_i.$$
That is, $[\id_V]_{B'}^B$ is the matrix whose columns are $b_1', \dots, b_n'$. 
***
#### Example – CoB and $P_n$
Consider $V = P_2$, let $B = \{1, x, x^2\}$ and $B' = \{1,x-2,(x-2)^2\}$ be bases of $V$. We calculate the change of basis matrix. We have
$$\begin{aligned}\id_V(1) &=1 ,\\
\id_V(x) &=2\cdot1+1\cdot(x-2), \\
\id_V(x^2) &=4\cdot1 +4\cdot(x-2)+1\cdot(x-2)^2.
\end{aligned}
$$
Thus, the change of basis matrix is given by 
$$[\id_V]_B^{B'} = \begin{bmatrix}
1 & 2 & 4\\
0 & 1 & 4\\
0 & 0 & 1
\end{bmatrix}.$$
If we wish to represent $f(x) = 1 + x + x^2$ in the basis $B'$, we start by noting
$[f(x)]^B = (1,1,1)^\tau$ (where recall $\tau$ means to take the transpose) and compute $[\id_V]_B^{B'} \cdot (1,1,1)^\tau$ to get $(7, 5, 1)^\tau$. This tells us that
$$
1 + x + x^2 = 7 + 5(x-2) + (x-2)^2.
$$
***
#### Example – Representing Bases
Here is a concrete example. Let $R = \R$, $V$ the collection of polynomials in $x$ with coefficients in $\R$ of degree at most $m$. Let $D: V \to V$ be the map sending a polynomial to its derivative. The most obvious choice for a bases of $V$ is $1, x, \dots, x^m$. With respect to this basis, the map $D$ is represented by the $n \times n$ matrix 
$$
\begin{bmatrix}
0 & 1 & 0 & 0 & \cdots & 0 \\
0 & 0 & 2 & 0 & \cdots & 0 \\
0 & 0 & 0 & 3 & \cdots & 0 \\
0 & 0 & 0 & 0 & \ddots & 0 \\
0 & 0 & 0 & 0 &  \cdots & m \\
0 & 0 & 0 & 0 &  \cdots & 0 \\
\end{bmatrix}.
$$

If, when $m = 2$, we  instead used $1, x^2, 3x-7$ as a basis, then the matrix for $D$
would be
$$\begin{bmatrix}
0 &  \frac{14}{3} & 3 \\
0 &  0 & 0 \\
0 &  \frac23   & 0\\ 
\end{bmatrix}.$$
***
#### Example – Multilinear Maps when $n=1$
When $n=1$, a multi-linear map is the same thing as an $R$-module homomorphism.(The alternating condition is vacuous in this case.) 
***
#### Example – $R$-Bilinear Maps ($n=2$)
When $n= 2$, instead of "$R$-multilinear'' we say "$R$-bilinear''. If $\phi: V \times V \to R$ is $R$-bilinear then $$\phi(v+w, u+m) = \phi(v,u) + \phi(v,m) + \phi(w,u)+\phi(w,m).$$
Also $\phi(rv,w) = r\phi(v,w) = \phi(v, rw)$.
For any example of this, take $V = R^m$. Then the "dot product'' $\phi:V \times V \to R$ defined by $\phi((a_1, \dots, a_m)^\tau, (b_1, \dots,   b_m)^\tau) = \sum_i a_i b_i$ is $R$-bilinear. But the dot product isn't alternating.
***
#### Example – Determinant Formula Using Bilinear Map
For $n  =2$ and $V = R^2$, $\phi: V \times V \to R$ defined by $$\phi(\begin{bmatrix} x \\ y \end{bmatrix}, \begin{bmatrix} z \\ w \end{bmatrix}) = xw - yz$$is both $R$-bilinear and alternating. This is of course the familiar determinant formula. 
***
#### Example – Determinant when $n=2$
For $n = 2$ we have $$\det(\begin{bmatrix} a_{1,1} & a_{1,2} \\ a_{2,1} & a_{2,2} \end{bmatrix}) = a_{1,1} a_{2,2} - a_{2,1} a_{1,2}.$$
***
#### Example – Determinant of Upper Triangular Matrix
If $A$ is upper triangular, then $\det(A) = \prod_i a_{i,i}$. For note that for such a matrix the only non-zero terms in the formula for $\det(A)$ occur when $\s(i) \leq i$ for all $i$, and this can only happen when $\s = \id$. Similarly, if $A$ is lower triangular, then $\det(A) = \prod_i a_{i,i}$.

In particular, if $E$ is a type I elementary matrix, then $\det(E) = 1$
and if $E$ is a type II elementary matrix with scalar $u \ne 0$, then $\det(E) = u$. We'll look at the determinants of Type III elementary matrices later.

An even more special case is $\det(I_n) = 1$. 
***
#### Exercise – Determinant of Transpose
Prove $\det(A) = \det(A^\tau)$ where $\tau$ denotes transpose.

###### Solution
***
#### Example – Determinant and Multiplication by $x$
Let $V = F[x]/I$ where $F$ is a field, $I = F[x] \cdot f(x)$ with $f$ a monic polynomial. Say $f(x) = x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$.  
Recall that every element of $V$ is uniquely represented by a coset of the form
$$
\ov{p(x)} := p(x) + I
$$
where $p(x)$ is a polynomial of degree at most $n-1$. 

We will regard $V$ as just an $F$-vector space (via restriction of scalars along $F \into F[x]$). Then $V$ is a finite dimensional --- for instance, a basis of $V$ is given by $\ov{1}, \ov{x}, \dots, \ov{x^{n-1}}$.
  
Let $g: V \to V$ be the function given as multiplication by $x$. Then $g$ is an $F$-linear operator, since $g(v+v') = x(v+v') = xv + xv' = g(v) + g(v')$ and $g(cv) = x(cv) = c (xv) = c g(v)$. (In fact, $g$ is $F[x]$-linear, but we won't use that fact.) Relative to the ordered basis $\ov{1}, \ov{x}, \dots, \ov{x^{n-1}}$, the matrix of $g$ is
$$
C(f) :=
\begin{bmatrix}
  0 & 0 & \cdots & 0 & -a_0 \\
  1 & 0 & \cdots & 0 & -a_1 \\
   0 & 1 & \cdots & 0 & -a_2 \\
   \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 1 & -a_{n-1} \\   
\end{bmatrix}
$$
The right-most column is due to the fact that, since $\overline{f(x)} = 0$ in $V$, we have
$$
x \cdot \overline{x^{n-1}} =
\overline{x^n} = -a_{n-1} \overline{x^{n-1}} -a_{n-2} \overline{x^{n-2}} - \cdots - a_1 \overline{x} - a_0 \overline{1}.
$$

The matrix  $C(f)$ is known as  the {\em companion matrix of $f(x)$} – it is defined for any monic polynomials with entries in a field.

We have  $\det(C(f)) = (-1)^n a_0$, since the only permutation that gives a non-zero term in the formula for $\det$ is the $n$-cycle  $\s = (2 \, 3 \, \dots \, n \, 1)$, and its  has sign is $(-1)^{n-1}$. So $\det(g) = (-1)^n a_0$. 
***
#### Example – Trace and Multiplication by $x$
With the notation of  Example \ref{ex:228}, $\trace(g) = -a_{n-1}$. 
***
#### Example – Det and Trace of $\C$ and Linear Operator
Let $\C$ denote the complex numbers. We may regard $\C$ as  an $\R$-vector space. Given $z = a + bi \in \C$, multiplication by $z$ on $\C$ is an $\R$-linear operator. What are the determinant and trace of this operator?
Relative to the basis $1, i$ of $\C$ as a real vector space, multiplication by $z = a = ib$ is represented by the matrix
$$\begin{bmatrix}
    a & -b \\ 
    b & a   \\
  \end{bmatrix}$$
and hence the determinant of this operator is $a^2 + b^2$, the
square of the norm of $z$, The trace is $2a$. Note that the determinant of this operator is $\|z\|^2$ the square of the usual complex norm.
***
#### Example – Matrix of Field Extension
Similarly, we may consider the field extension $\Q \subseteq \Q(\sqrt{-2})$. For any $a + b \sqrt{-2}$ in the larger field, define $g: \Q(\sqrt{-2}) \to \Q(\sqrt{-2})$ to be multiplication by $a + b \sqrt{-2}$. Then $\Q(\sqrt{-2})$ is a $\Q$-vector space and $g$ is a $\Q$-linear operator. A $\Q$-basis of $\Q(\sqrt{-2}$ is given by $B = \{1, \sqrt{-2}\}$ and relative to this basis the matrix representing $g$ is
$$[g]_B^B = 
  \begin{bmatrix}
    a & -2b \\ 
    b & a   \\
  \end{bmatrix}$$
and hence $\det(g) = a^2 + 2b^2$, once again the square of the of usual complex norm of the element $a + b \sqrt{-2}$.
***
#### Exercise – $\charpoly(0)$
Show $\cp_g(0) = (-1)^n \det(g)$.

###### Solution
***
#### Exercise – CharPoly and Trace
Show that if $\dim_F(V) = n$, then the coefficient of $x^{n-1}$ in $\cp_g(x)$ is $-\trace(g)$.

###### Solution
***
#### Example – Triangular Matrix and CharPoly
If $A$ is upper or lower triangular, then $\cp_A(x) = \prod_i (x - a_{i,i})$. As you may recall from an undergraduate class, in this case $a_{1,1}, \dots, a_{n,n}$ are the eigenvalues of $A$. More on this later. 
***
#### Example – $\Z$-Module Presentation
What $\Z$-module $M$ is presented  by
$$
A =
\begin{bmatrix}
2 & 1 & 0 \\
3 & 9 & 5 \\
1 & -2 & 7 \\
0 & 1 & 2 \\
\end{bmatrix}?
$$
Formally, $M$  is the quotient module $M=\Z^4/\im(T_A)$, where $T_A:\Z^3\to \Z^4$ is defined by $T_A(v)=Av$. Since $\Z^4$ is generated by its standard basis elements
$\{e_1,e_2,e_3,e_4\}$, it follows that $M=\Z^4/\im(T_A)$ is generated by the cosets of the $e_i$. To keep the notation short, we set $m_i=e_i+\im(T_A)$. 

Let $N=\im(T_A)$ and note that $N$ is the submodule of $\Z^4$ generated by the columns of $A$, i.e.
$$
N=\Z \cdot \left\{\begin{bmatrix} 2 \\ 3 \\ 1\\
    0 \end{bmatrix}, \begin{bmatrix} 1 \\ 9 \\ -2
    \\1 \end{bmatrix},\begin{bmatrix} 0 \\ 5 \\
    7\\2 \end{bmatrix}\right\}=
\Z \cdot \{2e_1 + 3e_2 +
e_3,e_1 + 9e_2 -2 e_3 + e_4, 5e_2 + 7 e_3 + 2 e_4  \}.
$$ Since $N$ maps to $0$ under the quotient map  $q:\Z^4\to M=\Z^4/N$, we have that the relations of $M$ can be written as
$$
\begin{aligned}
2m_1 + 3m_2 + m_3 & = 0 \\
m_1 + 9m_2 -2 m_3 + m_4 & = 0 \\
5m_2 + 7 m_3 + 2 m_4 & = 0. 
\end{aligned}
$$
We can now see that this is a rather inefficient presentation, since we can clearly use the first equation to solve for for $m_3=-2m_1 - 3m_2$. This implies that $M$ can be generated using only $m_1, m_2$ and $m_4$, that is
$$
M=\Z \cdot \{m_1,m_2,m_3,m_4\}= \Z \cdot \{m_1,m_2,m_4\}.
$$
This eliminates the first equation, and by substituting $m_3 = -2m_1 -3m_2$ the latter two relations become
$$
\begin{aligned}
5m_1 + 15m_2 + m_4 & = 0 \\
-14m_2  -16m_2 + 2m_4 & = 0 \\
\end{aligned}
$$
Now we can also eliminate $m_4$, i.e  leaving just two generators $m_1, m_2$ that satisfy
$$
-24m_1 -46m_2 = 0.
$$
Let us notice that what we have really done is to perform certain transformations of the matrix
$A$. In detail, we can use elementary row operations to "make zeros'' on the 1st and 2nd columns as follows:
$$
A =
\begin{bmatrix}
2 & 1 & 0 \\
3 & 9 & 5 \\
1 & -2 & 7 \\
0 & 1 & 2 \\
\end{bmatrix}
\rightarrow
\begin{bmatrix}
0 & 5 & -14 \\
0 & 15 & -16 \\
1 & -2 & 7 \\
0 & 1 & 2 \\
\end{bmatrix}
\rightarrow
\begin{bmatrix}
0 & 0 & -24 \\
0 & 0 & -46 \\
1 & 0 & 13\\
0 & 1 & 0 \\
\end{bmatrix}
$$
Eliminating the generators $m_3$ and $m_4$ amounts to dropping the first two columns (which are the 3rd and 4th standard basis vectors) as well as the last two rows. As we will prove soon, this shows that the $\Z$-module presented by $A$ is  isomorphic to the $\Z$-module presented by
$$
B=
\begin{bmatrix} -24 \\ - 46
\end{bmatrix}.
$$
We can go further. Set $m_1' := m_1 + 2m_2$. Then $m_1'$ and $m_2$  also form a generating set of $M$. The relation on $m_1, m_2$ translates to
$$
-24m'_1  +2 m_2 = 0
$$
given by the matrix
$$
C = E_{1,2}(-2)B=
\begin{bmatrix} -24 \\ 2
\end{bmatrix}.
$$
Note that we have done a row operation (subtract twice row 1 from row 2) to get from $B$ to $C$.
Continuing in this fashion by subtracting 12 row 2 from row 1 we also form 
$$
D = E_{1,2}(12)C=
\begin{bmatrix} 0 \\ 2
\end{bmatrix},
$$
The last matrix $D$ presents the module $M'=\Z^2/\im(t_D)$ with generators $a, b$ $(a=e_1+\im(t_D), b=e_2+\im(t_D)$) and relation $2a = 0$. As we will see, this proves $M \cong \Z \oplus \Z/2$.
***
#### Example – Special Case of SNF
Suppose $R$ is a Euclidean domain and  $A = (x_1, \dots, x_n)$ is a $1 \times n$ matrix.  Column operations of type I in this case amount to adding a multiple of one element in this list to another one. 
The SNF Theorem in this case amounts to the Euclidean algorithm: 
By adding  a suitable multiple of the one entry in the first two positions to the other, in the usual back-and-forth way, we arrive at $(g_1, 0, x_3, \dots, x_n)$ where $g_1 = \gcd(x_1, x_2)$.  Repeat this for columns $1$ and $3$ to arrive at $(g_2, 0, 0, x_4, \dots, x_n)$ where $g_2 = \gcd(g_1, x_3) = \gcd(x_1, x_2, x_3)$. Continuing in this fashion we arrive at $(g, 0, \dots, 0)$ where $g  = \gcd(x_1, \dots, x_n)$. 

The proof of the SNF Theorem in general amounts to an extended version of the idea used in this special case. 
***
#### Exercise – Finding SNF
Consider the matrix with entries in $\Z$
 $$
 A=\begin{bmatrix}
 1 & 6 & 5 & 2 \\
 2 & 1 & -1 & 0 \\
 3 & 0 & 3 & 0
 \end{bmatrix}.
 $$
Do row and column operations to put $A$ into its Smith normal form: $$S=\begin{bmatrix}1 & 0 & 0 & 0 \\0 & 1 & 0 & 0 \\0 & 0 & 6 & 0 \\\end{bmatrix}.$$Conclude that the module presented by $A$ is isomorphic to $\Z/6$.

###### Solution
***
#### Example – Noetherian Rings
If $R$ is a PID then by definition every ideal is finitely generated (by a single element in fact) and hence $R$ is Noetherian.

Likewise every field is Noetherian.

If $R$ is Noetherian and $J$ is any ideal, then $R/J$ is also Noetherian: By the 4-th isomorphism theorem, 
an arbitrary ideal of $R/J$ has the form $I/J$ for some ideal $I$ of $R$ that contains $J$. Since $R$ is Noetherian,  $I$ is finitely generated as an $R$-module and since $I/J$ is a quotient of $I$, it is finitely generated as a $R/J$-module
***
#### Example – Most Useful Things Are Noetherian
Combining the facts above together gives that every ring of the form $A[x_1, \dots, x_n]/I$ where $A$ is a field or $\Z$ (or any Noetherian ring) and $I$ is any ideal is again a Noetherian ring. This includes a large collection of rings of the most interest in the fields of commutative algebra and algebraic geometry.
***
#### Example – Abelian Groups of Order $120$
How many abelian groups of order $120$ are there up to  isomorphism? There are three: $\Z/120$, $\Z/2 \oplus \Z/60$ and $\Z/2 \oplus \Z/2 \oplus \Z/30$.
***
#### Example – $k[x]$-Modules of Dimension $4$
Let $k$ be a field and $M$ a $k[x]$-module such that the dimension of $M$ as a $k$-vector space is $4.$ What are the possibilities for $M$ up to isomorphism?

We have
$$M \cong k[x]^r \oplus k[x]/(f_1(x)) \oplus \cdots \oplus k[x]/(f_s(x))$$ with $r, s, f_1, \dots, f_s$ as in the Corollary. But $r$ must be $0$ since $k[x]$ is infinite dimensional as a $k$-vector space. Moreover, $\dim_F k[x]/g = \deg(g)$ for any non-zero polynomial $g$. So we must have $\sum_i \deg(f_i) = 4$.
There are five possibilities:
1. $s = 1$ and $f_1$ is monic of degree $4$.
2. $s = 2$, $f_1$ is linear, $f_2$ is cubic and $f_1 \mid f_2$. (So if $f_1 = x-a$, then $a$ must be a root of $f_2$).
3. $s = 2$, $f_1 = f_2$ is quadratic.
4. $s = 3$, $f_1 = f_2$ is linear and $f_3$ is quadratic with $f_1 \mid f_3$.
5. $s = 4$, $f_1 = f_2 = f_3 = f_4$ is linear.
Now suppose $k = \Z/p$. What is the total number of possibilities? For case $1$, there are $p^4$ monic polynomial of degree $4$. For case $2$, there are $p$ choices for $f_1$ and $p^2$ choices for $f_2$ since $f_2 = f_1 \cdot q$ for a unique quadratic $q$, for a total of $p^3$ possibilities. For case $3$ there are $p^2$ choices. For case $4$ there are $p^2$ choices since there are $p$ choices for $f_1 = f_2$ and $f_3 = f_1 \cdot l$ for a unique linear $l$. For case $5$, there are $p$ choices for $f_1$. 
In total there are $2p + 2p^2 + p^4$ such modules up to isomorphism.
***
#### Example – $\Z/90$
Since $\Z/90 \cong \Z/9 \oplus \Z/2 \oplus \Z/5$, so the elementary divisors of $\Z/90$ are $9$, $2$ and $3$. The only invariant factor   of $\Z/90$ is $90$. 
***
#### Example – Direct Sums and $\Z$
Consider the group $G = \Z/90 \oplus \Z/9 \oplus \Z/6 \oplus \Z/3 \oplus \Z/4$. This is neither in IFF nor in EDF. Applying the Chinese Remainder Theorem, we have
$$G \cong \Z/9 \oplus \Z/2 \oplus \Z/5 \oplus \Z/9 \oplus \Z/2 \oplus \Z/3 \oplus \Z/3 \oplus \Z/4,$$
and this gives the EDF. The elementary divisors of $G$ are $9,2,5,9,2,3,3,4$ (ordering does not matter).

To find the IFF we start by finding the largest prime power order for each prime in the list of orders of the summands. These are  $9, 5, 4$. The
CRT gives $$G \cong \Z/(9 \cdot 4 \cdot 5) \oplus \Z/2 \oplus \Z/9 \oplus \Z/2 \oplus \Z/3 \oplus \Z/3.$$
Then we find the highest prime power orders for each prime among the left-over summands: $9, 2.$ By the CRT we have
$$G \cong \Z/(9 \cdot 4 \cdot 5) \oplus \Z/(2 \cdot 9) \oplus   \Z/2 \oplus \Z/3 \oplus \Z/3.$$
The highest orders of the prime power order not yet used are $2$ and $3$, and we have 
$$G \cong \Z/(9 \cdot 4 \cdot 5) \oplus \Z/(2 \cdot 9) \oplus   \Z/(2 \cdot 3)  \oplus \Z/3.$$ which can be rearranged to give $$G \cong \Z/3 \oplus \Z/6 \oplus \Z/18 \oplus \Z/180.$$
This is the IFF, and the invariant factors of $G$ are $3,6,18,180$.
***
#### Exercise – Finding IFs and EDs
Find the invariant factors form and the elementary divisors form of the  $k[x]$-module $$M = k[x]/(x^2-1) \oplus k[x]/(x-1) \oplus k[x]/(x^2 + 1) \oplus k[x]/(x^2 + 2x + 1)$$ first when (a) $k = \Z/2$, (b)  $k = \R$ and (c) $k = \C$.

###### Solution
***
#### Example – Special Case of $V_g$
We have the following special case (it isn't really special --- the general case reduces to this one upon choosing a basis):

Given a matrix $A \in \Mat_{n \times n}(F)$, then $F^n_A$ is the $F[x]$-module whose underlying abelian group is $F^n$ (column vectors) with the usual rule for addition and with the rule for $F[x]$ scaling given by
$$
(\sum_i c_i x^i) \cdot v := \sum c_i A^i v
$$
for any column vector $v$. For short, we write this rule as
$$
f(x) \cdot v = f(A) v
$$
for any polynomial $f(x) \in k[x]$, where $f(A)$ is the matrix obtained by evaluating $f(x)$ at $x = A$ in the evident sense. 
***
#### Example – $\Mat_{2\times 2}(\Q)$
Let $A=\begin{bmatrix} 1 & 1 \\ 0 & 1  \end{bmatrix}\in \Mat_{2 \times 2}(\Q)$ and let $M$ be the $\Q[x]$-module $\Q^2_A$. So $M = \Q^2$ as a $\Q$-vector space, and $x$ acts on $M$ by sending $\vectwo{a}{b} \in M$ to
$\vectwo{a+b}{b} \in M$. I claim there is an isomorphism
$$
M \cong \Q[x]/(x-1)^2
$$
of $\Q[x]$-modules.

Let $v = \vectwo{0}{1} \in M$. Note that $x \cdot v = \vectwo{1}{1}$ and that $v$ and $x \cdot v$ span $\Q^2$ as a $\Q$-vector space. It follows that $v$ generates $M$ as a $\Q[x]$-module; in detail, for any $\vectwo{a}{b} \in \Q^2$
we have $(b- a  + ax)v = \vectwo{0}{a} + \vectwo{a}{a} = \vectwo{a}{b}$.

Define a $\Q[x]$-module homomorphism
$$\pi: \Q[x] \onto M$$
by sending $1$ to $v \in M$ and hence $p(x)$ to $p(x) \cdot v$.  It is onto since $v$ generates $M$ as a $\Q[x]$-module. The kernel will be a (necessarily principle) ideal of $\Q[x]$; we just need to find it. Note that $x^2 v = \vectwo21$, $xv$ and $v$ are linearly dependent and in fact we have $$x^2 v = 2x v- v$$and hence $(x^2 -2x + 1)v  =0$. This gives that $x^2 -2x + 1$ is in the kernel of $\pi$ and hence, by the $0$-th Isomorphism Theorem we have an induced homomorphism of $\Q[x]$-modules $$\ov{\pi}: \Q[x]/(x^2 - 2x + 1) \onto M$$induced by $\pi$. The map $\ov{\pi}$  is onto since $\pi$ is onto. Since the source and target both have dimension two as $\Q$-vector spaces, $\ov{\pi}$ is $\Q$-linear, and $\ov{\pi}$ is onto, it must in fact be an isomorphism of $\Q[x]$-modules (by the rank-nullity Theorem).
***
#### Example – Back to $\Mat_{2\times 2}(\Q)$
Let us return to the example of $A = \begin{bmatrix} 1 & 1 \\ 0 & 1  \end{bmatrix}\in \Mat_{2 \times 2}(\Q)$ to illustrate the Theorem and its proof.
By the previous example we have an isomorphism of $\Q[x]$-modules
$$
\Q^2_A \cong \Q[x]/(x^2 - 2x + 1).
$$
Recall that $\lx$ (multiplication by $x$) on $\Q^2_A$ is given by multipcliation by the matrix $A$.
This is an isomorphism of $\Q[x]$-modules, and so $A$ corresponds to the operator $\lx$ on  $\Q[x]/(x^2 - 2x + 1)$. As we have seen before, relative to the basis $\{1, x\}$, the matrix for $\lx$ is 
 $$
C(x^2 - 2x + 1) = 
\begin{bmatrix} 
0 & -1 \\
1 & 2 \\
\end{bmatrix}.
$$
This is the Rational Canonical Form of $A$. $A$ has just one invariant factor, namely $x^2 - 2x + 1$.

By the way, tracking through the calculations that got us here, we see that the basis of $\Q^2$ that gives the RCF of $A$ if $\vectwo01, \vectwo11$ of $\Q^2$.
***
#### Example – Similarity Classes of $4\times 4$ Matrices
Let $F = \Z/p$ be the field with $p$ elements for some prime $p$. Up to similarity, how many $4 \times 4$ matrices are there with entries in $F$?

Each such matrix is similar to a unique one of the form
$$
C(f_1) \oplus \cdots \oplus C(f_k)
$$
with $f_1, \dots, f_k$ monic polynomials of positive degree such that $f_1 \mid \cdots \mid f_k$. Moreover, since $C(f)$ is a $d \times d$ matrix where $d = \deg(f)$, we must have $\deg(f_1) + \cdots + \deg(f_k) = 4$. So the goal becomes to count all such tuples $(f_1, \dots, f_k)$ of polynomials. We proceed by cases on
$k$. Note that $k \geq 5$ is not possible. 
- Case $k = 1$. Then $\deg(f_1) = 4$ and the number of such polynomials is $p^4$ (since $f_1 = x^4 + a_3 x^3 + a_2 x^2 + a_1 x + a_0$ and $F$ has $p$ elements).
- Case $k = 2$:  Note that $\deg(f_1) \geq 3$ is not possible. If $\deg(f_1) = 2$ then $f_1 = f_2$, and there are $p^2$ possibilities. If $\deg(f_1) = 1$, then $\deg(f_2) = 3$ and $f_2 = f_1 \cdot g$ with $g$ monic and $\deg(g) = 2$. There are $p$ possibilities for $f_1$ and $p^2$ for $g$, for a total of $p^3$ in this subcase. The total for this case is thus $p^2 + p^3$. 
- Case $k= 3$: The only possibilities are $\deg(f_1) = 1$, $\deg(f_2) = 1$ and $\deg(f_3) = 2$ so that $f_2 = f_1$ and $f_3 = f_1 \cdot g$ with $\deg(g) =1$. We get $p^3$ possibilities.
- Case $k  = 4$. We must have $f_1 = f_2 = f_3 = f_4$ with each of degree $1$, for a total of $p$ possibilities.  
The total is $$p^4 + p^2+ p^3 + p^3 + p.$$
***
#### Example – Once More to Back to $\Mat_{2\times 2}(\Q)$
Let's find the invariant factors of the matrix $A= \begin{bmatrix} 1 & 1 \\ 0 & 1  \end{bmatrix}\in \M_{2 \times 2}(\Q)$ we looked at before, but this time using the Theorem and its Corollary.

We have 
$$
xI_2-A= \begin{bmatrix} x-1 & -1 \\ 0 & x-1  \end{bmatrix}.
$$
To find the invariant factors of $A$ we just need to find the Smith Normal Form  of $xI_2-A$. I'll do this two ways:

Method I: Do row and column operations using the generalized Euclidean algorithm:
$$
\begin{bmatrix} x-1 & -1 \\ 0 & x-1  \end{bmatrix} \mapsto
\begin{bmatrix} x-1 & -1 \\ (x-1)^2 & 0   \end{bmatrix} \mapsto
\begin{bmatrix} 0 & -1 \\ (x-1)^2 & 0   \end{bmatrix} \mapsto
\begin{bmatrix} 1 & 0 \\ 0 & (x-1)^2  \end{bmatrix}.
$$
Tossing out the unit, we see that the only invariant factor is $(x-1)^2$, as before.

Method II: Call $d_1, d_2$ the entries on the diagonal of the SNF of $xI_2-A$. Recall from 
Theorem \ref{thm324} that $d_1$ is the gcd of the entries of $xI_2-A$ and $d_1d_2=\det(xI_2-A)$. Thus $d_1=1$ and $d_2=\det(xI_2-A)=(x-1)^2$. Therefore the only invariant factor of $A$ is $(x-1)^2$.
***
#### Example – Finding IFs and RCF
Let 
$$
A = 
\begin{bmatrix} 
1 & -1 & 1 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{bmatrix}.
$$
Let us find the invariant factors and Rational Canonical Form of $A$ by finding the Smith Normal Form of $xI_3 - A$.


We have 
$$
xI_3 - A =
\begin{bmatrix} 
x-1 & 1 & -1 \\
0 & x & -1 \\
0 & -1 & x \\
\end{bmatrix}.
$$
A sequence of messy row and column operations yields
$$
\begin{bmatrix} 
1 & 0 & 0 \\
0 & x-1 & 0 \\
0 & 0 & x^2-1 \\
\end{bmatrix}.
$$
Note that this is indeed in Smith Normal Form. 
It follows that the invariant factors of $A$ are $x-1, x^2-1$ and the RCF of $A$ is 
$$
C(x-1) \oplus C(x^2-1) = 
\begin{bmatrix} 
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{bmatrix}.
$$

For an alternative approach, we could use that the diagonal entries $d_1, d_2, d_3$ of the Smith Normal Form of $xI_3  - A$ satisfy $d_1 = \gcd(xI_3 - A)$, $d_1d_2$ is the gcd of the $2 \times 2$ minors of $xI_3 - A$, and  $d_1d_2d_3 = \det(xI_3 - A)$.
It's clear that $d_1 = 1$ and an easy calculation gives that $\det(xI_3 - A) = (x-1)(x^2 -1)$.
There are nine $2 \times 2$ minors of $xI_3 - A$, and a tedious check reveals that each of them is one of $x^2 -1$, $x(x-1)$, $x-1$ or $0$ (up to signs). 
So $d_1d_2 = x-1$. We get that
$$
d_1 = 1, d_2 = x-1, d_3 = x^2 -1
$$
as before.
***
#### Example – Finding Minimum Polynomial
Let's find the minimum polynomial of 
$$
\begin{bmatrix}
1 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 \\
0 &  0 & 1 & 1 \\
0 &  0 & 0 & 1 \\
\end{bmatrix}
$$

We apply the Cayley-Hamilton Theorem:  $\mp_A(x) \mid \cp_A(x)$. The polynomial $\cp_A(x)$ is easy to compute since this matrix is upper-triangular:
$\cp_A(x) =\det(xI_4 - A) = (x-1)^4$. So $\mp_A(x) = (x-1)^j$ for some $j \leq 4$. By brute-force, we verify that $(A-I_4)^3 \ne 0$ and thus it must be the case that $\mp_A(x) = \cp_A(x) = (x-1)^4$. 
***
#### Example – Finding Minimum Polynomial (2)
Let's find the minimum polynomial of 
$$
\begin{bmatrix}
1 & 1 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 &  0 & 1 & 1 \\
0 &  0 & 0 & 1 \\
\end{bmatrix}
$$
As in the previous example, $\cp_A(x) = (x-1)^4$ and so by the Cayley-Hamilton Theorem
$\mp_A(x) = (x-1)^j$ for some $j \leq 4$. This time we notice that $(A-I_4)^2 = 0$ and so, since $(A-I_4) \ne 0$, $\mp_A(x) = \cp_A(x) = (x-1)^2$. 
***
#### Example – Companion Matrix and Jordan Blocks
Let us consider the companion matrix of $(x-2)^3 = x^3 -6x^2 + 12x -8$:
$$
A =
\begin{bmatrix}
0 & 0 & 8 \\
1 & 0 & -12 \\
0 & 1 & 6 
\end{bmatrix}=C((x-2)^3)\in \M_{3 \times 3}(\Q).
$$
We can interpret this matrix as arising from the linear transformation $g$ on 
$$
V := \Q[x]/(x-2)^3
$$
defined as multiplication by $x$. Recall that the ordered basis of $V$ that gives the matrix $A$ is the "obvious one'':
$$
B=\{\ov{1}, \ov{x}, \ov{x^2}\}.
$$
But notice that 
$$
B'=\{\ov{1}, \ov{x-2}, \ov{(x-2)^2}\}
$$
is also a basis of $V$.
Let us calculate what the operator $g$ does to this alternative basis. We could work this out by brute force, but a cleaner way is to first compute what the operator $g -2 \cdot \id_V$ does. Since $g - 2 \cdot \id_V$ is multiplication by $x-2$, it sends each basis element to the next one, except for the last one,  which is sent to $0$. It follows that the matrix of this operator relative to the ordered basis $B'$ is 
$$
[g - 2 \cdot \id_V]_{B'}^{B'} = 
\begin{bmatrix}
0 & 0 & 0 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{bmatrix}
$$
and hence the matrix for $g$ itself for this basis is
$$
[g]_{B'}^{B'} = 
\begin{bmatrix}
2 & 0 & 0 \\
1 & 2 & 0 \\
0 & 1 & 2 \\
\end{bmatrix} =: J_3(2).
$$
This is what's known as a  "Jordan Block''. 
***
#### Example – Finding JCF
Let us find the Jordan canonical form of 
$$
A = 
\begin{bmatrix} 
1 & -1 & 1 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{bmatrix}
\in \Mat_{3 \times 3}(\Q).
$$

We found the Rational Canonical Form of this matrix before. In the process we showed that we have an isomorphism of $\Q[x]$-modules.
$$
\Q^3_A \cong \Q[x]/(x-1) \oplus \Q[x]/(x^2-1).
$$
By the Chinese Remainder Theorem
$$
\Q[x]/(x-1) \oplus \Q[x]/(x^2-1) \cong \Q[x]/(x-1) \oplus \Q[x]/(x-1) \oplus \Q[x]/(x+1)
$$
and thus the Elementary Divisors of $\Q^3_A$ are $x-1, x-1, x+1$. By the Theorem this shows that the JCF of $A$ is $$
J_1(1) \oplus J_1(1) \oplus J_1(-1) = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & -1 \end{bmatrix}.$$
***
#### Example – Does it Have Roots?
Does $x^4 + 8x^3 + 21x^2 + 20x + 13 \in \Q[x]$ have any roots? No. The only possible roots are $\pm 1$ and $\pm 13$, and a careful check rules these out.
Is $x^4 + 8x^3 + 21x^2 + 20x + 13 \in \Q[x]$ irreducible? No, it factors as $x^2 + x + 1$ times $x^2 + 7x + 13$
***
#### Example – Irreducibility and Gauss
Let's prove $f = x^4 + 7x^3 + 16 x^2 + 124 x + 23 \in \Q[x]$ is irreducible. By Gauss's Lemma, we just need to show it is irreducible in $\Z[x]$.

If $f$ did factor in $\Z[x]$ as a product of monic polynomials, then $\ov{f} \in \Z/2[x]$ would also factor in this way. Now $\ov{f} = x^4 + x^3 + 1 \in \Z/2[x]$. This has no roots (the only possibilities are $0$ or $1$)
and so if it did factor it would have to factor as a product of two quadratic, irreducible polynomials. The only such polynomial in $\Z/2[x]$ is $q = x^2+ x + 1$ (the others all have roots). But $q^2 \ne \ov{f}$. This proves $\ov{f}$ is irreducible in $(\Z/2)[x]$ and hence $f$ must be irreducible in $\Z[x]$. 
***
#### Example – Using Eisenstein
For instance, $5x^{11} - 30 x^4 +60 x^3 +360 x- 30$ is irreducible in $\Q[x]$ thanks to Eisenstein applied with $p = 2$. (Note that it isn't irreducible in $\Z[x]$ since it does not have unit content.) 
***
#### Example – Monic is Necessary 
The assumption that $f$ be monic in this Proposition is necessary. Consider for instance $f(x) = (3x+1)(x+1) = 3 x^2 + 4x + 1 \in \Z[x]$. Modding out by $3$ yields a linear polynomial in $(\Z/3)[x]$ which is thus irreducible. But clearly $f$ isn't irreducible in $\Z[x]$. (The Proposition can be generalized to non-monic polynomials by adding the assumption that $p$ does not divided the leading coefficient of $f$.) 
#### Example – Classic Field Extensions
$\Q \subseteq \R$ and $\R \subseteq \C$ are basic examples of field extensions.

Recall (perhaps from 817) that $\Q[\sqrt{2}] = \{a + b \sqrt{2} \mid a, b \in \Q\}$ is 
a field. So $\Q \subseteq \Q[\sqrt{2}]$ is another example of a field extension.
***
#### Example – More Field Extensions
Consider $x^3 - 2 \in \Q[x]$. It is irreducible (e.g., by Eisenstein) and has roots $\a = \sqrt[3]{2}$, $\beta = e^{2 \pi i/3} \sqrt[3]{2}$ and $\g = e^{4 \pi i/3} \sqrt[3]{2}$ in $\C$. So there are three ways in which we could "adjoin a root'' to $\Q$:
First we could form the field
$$
\Q[\a] = \{a + b \a + c \a^2 \mid a,b,c \in \Q\}.
$$
It is not completely obvious this is a field, but we'll prove it latter.
The reason that we don't need third or higher powers is that, e.g., $\a^3 = 2 \in \Q$.
Or we could instead form the field $\Q[\beta]$ or the field $\Q[\gamma]$. 
There are clearly not all equal since, for example, $\Q[\a] \subseteq \R$ but $\beta$ is not in $\R$. However, they are {\em isomorphic} field extensions as we will prove below.
***
#### Example – $\Q[\sqrt{2}]$
Take $F = \Q$ and $\a = \sqrt{2}$. Then any expression of the form $\sum_i r_i \a^i$ with $r_i \in \Q$ is equal to one of the form $a + b \sqrt{2}$ for $a, b \in \Q$.
If $c + d \sqrt{2} \ne 0$, then
$$
\frac{1}{c + d \sqrt{2}} = \frac{c-d \sqrt{2}}{c^2 - 2 d^2}
=
c' + d' \sqrt{2}
$$
with $c' = \frac{c}{c^2 - 2d^2}$ and $d' = \frac{-d}{c^2 - 2d^2}$ both in $\Q$. 
This proves that $\Q[\sqrt2] = \Q(\sqrt2) = \{a + b \sqrt2 \mid a,b \in \Q\}$ and in particular that $\Q[\sqrt{2}]$ is a field. 
***
#### Example – $\Q[\pi]$
$\Q[\pi]$ is not a field (and so in particular it is not equal to $\Q(\pi)$ since, for example, $\frac{1}{\pi} \notin \Q[\pi]$. (If it were, then we would have $\frac{1}{\pi} = \sum_{i=0}^n q_i \pi^i$ for some $q_i \in \Q$, and hence $\sum_i q_i \pi^{i+1} - 1 = 0$, which would imply $\pi$ is the root of a polynomial with rational coefficients. This is known to be not true.) 
***
#### Example – Degrees of Common Extensions
We have that $[\C: \R] = 2$ and $[\R:\Q] = \infty$. (We could in fact say $[\R:\Q]$ is the cardinality of $\R$, but in general we lump all infinite field extensions together when talking about degree.) We have $[\Q[\a]: \Q] = 3$ where $\a = \sqrt[3]{2}$.
***
#### Example – $\R[x]/(x^2+1)$
The last part of the proposition is notationally confusing to prove in general but clear in examples. So let's do a simple one: Say $F = \R$ and $p(x)= x^2 +1$. Then $L = \R[x]/(x^2+1)$. The assertion is that $\ov{x} := x + (x^2 + 1) \in L$ is a root of the polynomial $x^2 + 1$ viewed as having coefficients in $L$. In other words, this element has the property that its square is $-1$. Let's check: Since $\ov{x^2 + 1} = 0$ and $\ov{x^2 + 1} = \ov{x}^2 + 1$ we have $\ov{x}^2 = -1$. Indeed, there is a field isomorphism $L \cong \C$ sending $\ov{x}$ to $i$ and more generally $\ov{f}$ to $f(i).$
***
#### Example – $\sqrt{2}$ Primitive
$\sqrt{2}$ is a primitive element of the extension $\Q \subseteq\Q[\sqrt{2}] = \Q(\sqrt{2})$. So is $1 + \sqrt{2}$ and, more generally, $a + b \sqrt{2}$ for any $a, b \in \Q$ with $b \ne 0$.
***
#### Example – $\Q(\sqrt2,\sqrt3)$
Regard $\Q$ as a subfield of $\C$ and let $F = \Q(\sqrt{2}, \sqrt{3})$.
We may also describe $F$ as $F = E(\sqrt{3})$ where we set $E =\Q(\sqrt{2})$. 

I claim that $F$ is in fact a simple extension of $\Q$. For example, say $\g = \sqrt{2} + \sqrt{3}$. I claim that $\Q(\sqrt{2} + \sqrt{3}) = F$. Note that $\g^2 = 5 + 2 \sqrt{6}$ and
$$\g^3 = 5 \sqrt{2} + 5 \sqrt{3} + 4 \sqrt{3} + 6 \sqrt{2} = 11 \sqrt{2} + 9 \sqrt{3}.$$
So $\frac12(\g^3 - 9 \g) = \sqrt{2}$, and hence $\sqrt{2} \in \Q(\g)$. Likewise, $$\sqrt{3} = -\frac12(\g^3 - 11 \g) \in \Q(\g).$$So $\Q(\g) = \Q(\sqrt{2},\sqrt{3})$.
This example is an illustration of the Primitive Element Theorem (which we might or might not have time to prove this semester): Every finite extension of $\Q$ is generated by a single element (or, in other words, is simple). This example shows $\Q(\sqrt{2}, \sqrt{3})/\Q$ is simple and $\sqrt{2} + \sqrt{3}$ is a primitive element of this field extension.
***
#### Example – $i$ Algebraic over $\R$
$i \in \C$ is algebraic over $\R$. Indeed, every element of $\C$ is algebraic over $\R$. (E.g., $z = a + bi$ is a root of $x^2 -2ax +a^2 + b^2$.) $e^{2 \pi i/n} \in \C$ ia algebraic over $\Q$. So is $\sqrt{m}$ for any $m \in \Z$. 
The numbers $\pi$ and $e$ of $\R$ are transcendental over $\Q$; these are deep facts.
***
#### Example – Primitive Roots of Unity
For any prime integer $p$, set $\mu_p = e^{2 \pi i/p}$, a so-called "primitive $p$-th root of unity''. Let us find $m_{\mu_p, \Q}(x)$. Note that $\mu_p$ is a root of $x^p -1$ which factors as $(x-1) g(x)$ where $g(x) = x^{p-1} + \cdots + x + 1$. As we showed before, $g(x)$ is irreducible in $\Q[x]$. Since $\mu_p$ is not a root of $x-1$, it must be a root of $g(x)$, and since $g(x)$ is irreducible, it must be $m_{\mu_p, \Q}(x)$ (see the Remark).
***
#### Example – $\Q(\sqrt2)\cong\Q(-\sqrt2)$
A simple example illustrating the Corollary is that $\Q(\sqrt{2})$ and $\Q(-\sqrt{2})$ are isomorphic fields. In fact, the are equal: $\Q(\sqrt2) = \Q(-\sqrt{2})$. But the Corollary gives that there is an interesting isomorphism $\phi: \Q(\sqrt2) \xra{\cong} \Q(-\sqrt2) = \Q(\sqrt{2})$ that sends $\sqrt2$ to $-\sqrt{2}$. In general, we have $\phi(a + b \sqrt2) = a - \sqrt2$ for $a,b \in \Q$. This previews the central idea of Galois theory.
***
#### Example – Cube Roots
Let $\a=\sqrt[3]{2}$ (the unique real cube-root of $2$) and $\beta = e^{2\pi i/3} \sqrt[3]{2}$ (one of the two imaginary cube roots of $2$). 

Then by the Corollary (applied with $L = L' = \C$) there is an isomorphism $\Q(\a) \cong \Q(\beta)$ of fields that restricts to the identity map on $\Q$. Note that these two fields are not equal since the former is contained in $\R$ and the latter is not. 
***
#### Example – $\R(w)=\C$ for all $w\not\in\R$
Say $F \subseteq L$ is a field extension of prime degree $p$. Given $w \in L \setminus F$, by the Degree Formula we have $[L:F(w)][F(w):F] = [L:F] = p$. Since $w \notin F$, $F \subsetneq F(w)$ and so $[F(w): F] > 1$. It follows that $[L: F(w)] = 1$, whence $L = F(w)$. As a (very simple) example of this, since $[\C: \R]$ is prime, $\R(w) = \C$ for any complex number $w$ that is not real.
***
#### Example – Degree and $x^2-5$ 
Let $F$ be the result of adjoining to $\Q$ all of the roots in $\C$ of $x^2 - 5$. That is, $F = \Q(\a_1, \a_2, \a_3, \a_4)$ where $\a_1 = \sqrt[4]{5}$, $\a_2 = i \sqrt[4]{5}$, $\a_3 = -\sqrt[4]{5}$, and $\a_4 = - i \sqrt[4]{5}$. As we shall see later, $F$ is an example of a "splitting field''. Let's find $[F: \Q]$. 

First, let us note that we can also describe $F$ as $F = \Q(\sqrt[4]{5}, i)$. This holds since each of $\a_1, \dots, \a_4$ belongs to $\Q(\sqrt[4]{5}, i)$ and hence $F \subseteq \Q(\sqrt[4]{5}, i)$. The opposite containment holds because $\sqrt[4]{5}, i \in F$, with the latter being true because $i = \a_2/\a_1$.

Set $E = \Q(i)$. Then $[E: \Q] = 2$. Since $F = E(\sqrt[4]{5})$ and $\sqrt[4]{5}$ is a root of $x^4-5$, we have $[F : E]$ is at most $4$ and it will be exactly $4$ if and only if $x^4 -5$ is irreducible in $\Q(i)[x]$. This is unclear.

So instead let's try a different approach. Let $L = \Q(\sqrt[4]{5})$. Then since $x^4 - 5$ is irreducible in $\Q[x]$ by Eisenstein, we have $[L: \Q] = 4$. Since $F = L(i)$ and $i$ is a root of $x^2 +1$, we have $[F:L] \leq 2$. But $F \ne L$ since $F \subseteq \R$. Note that $[F:L] = 1$ if and only if $F = L$. Thus $[F:L] = 2$.

By the degree formula we conclude that
$$
[F: \Q] = [F:L][L:\Q] = 2 \cdot 4 = 8.
$$
Note that, in hindsight, it must have been true that $x^4 - 5$ is irreducible in $\Q(i)[x]$, since otherwise the degree formula would give that $[F: \Q] < 8$. 
***
#### Example – Infinite Algebraic Extension
Let $E_n = \Q(\sqrt[n]{2})$ and set $F = \bigcup_n E_n$. Then $F$ is a subfield of $\C$: To see this, note first that $E_n \subseteq E_m$ provided $n \mid m$. Given $a, b \in F$, we have $a \in E_n$ and $b \in E_m$ for some $n$ and $m$ and hence $a,b$ are both in $E_{mn}$. Since $E_{mn}$ is a field, we have $a + b$, $a-b$, $a \cdot b$ and (provided $a \ne 0$) $\frac{1}{a}$ all belong to $E_{mn}$ and hence to $F$. This proves $F$ is field extension of $\Q$. It is algebraic over $\Q$ since each $E_n$ is. But it is not a finite extension of $\Q$, since $[E_n: \Q] = n$ (since $x^n - 2$ is irreducible in $\Q[x]$ by Eisenstein) and hence $[F: \Q] \geq n$ for all $n$.
***
#### Example – $\C$ is Closed
$\C$ is algebraically closed. This is the Fundamental Theorem of Algebra.
***
#### Example – $\C$ is the Algebraic Closure of $\R$
$\C$ is an algebraic closure of $\R$. This follows from the fact that $\R \subseteq \C$ is a finite extension, hence algebraic, and the Fundamental Theorem of Algebra, which we will not prove. 
***
#### Example – Common Splitting Fields
- As a silly example, if $f(x)$ already splits into linear factors over $F[x]$, then $F$ itself is the splitting field of $f(x)$ over $F$.
- The splitting field of $x^2 + 1$ over $\R$ is $\C$. 
- If $q(x)$ is any irreducible quadratic polynomial in $\R[x]$, then the splitting field of $q(x)$ is $\C$.
- In general, given $f(x) \in \Q[x]$, a splitting field of $f(x)$ is given by $\Q(\a_1, \dots, \a_n)$ where $\a_1, \dots, \a_n \in \C$ are all of the roots of $f(x)$ in $\C$. 
- ***
#### Example – Splitting Fields and $(x^3-2)$
The splitting field $L$ of $x^3 -2$ over $\Q$ is $L = \Q(\sqrt[3]{2}, \zeta_3 \sqrt[3]{2}, \zeta_3^2 \sqrt[3]{2})$, where $\zeta_3 = e^{\frac{2 \pi i}{3}}$.
It is not hard to see that $L = \Q(\sqrt[3]{2}, \zeta_3)$. We have $[\Q(\sqrt[3]{2}): \Q] = 3$ since $x^3 - 2$ is irreducible in $\Q[x]$ (by Eisenstein). Since $\Q(\sqrt[3]{2}) \subseteq \R$ and thus $\Q(\sqrt[3]{2}) \ne L$, the degree formula gives that $[L: \Q] \geq 6$. By the Theorem, $[L: \Q] \leq 6$ and hence $[L: \Q] = 6$. (We could also have proven this without appealing to the Theorem.)
***
#### Example – Splitting Fields and $(x^4-5x^2+6)$
The splitting field of $f(x) = x^4 - 5x^2 + 6$ is 
$$
\Q(\sqrt{2}, -\sqrt{2}, \sqrt{3}, -\sqrt{3}) = \Q(\sqrt{2}, \sqrt{3}) = \Q(\sqrt{2} + \sqrt{3}).
$$
This holds since $f(x) = (x^2-3)(x^2-2)$. It is not too hard to see that the degree of this splitting field over $\Q$ is $4$, far smaller than the $4!$ upper bound given by the Theorem.
***
#### Example – Splitting Fields and $(x^n-1)$
Let $f(x) = x^n -1 \in \Q[x]$. Then $f(x)$ splits completely in $\C[x]$ and its roots are the $n$ $n$-th roots of $1$. One of these is $\zeta_n := e^{2 \pi i/n}$. Notice that every other $n$-th root of $1$ is a power of this one. We thus see that $\Q(\zeta_n)$ is the splitting field of $x^n-1$ over $\Q$. This field is called the {\em cyclotomic field} of $n-th$ roots of 1 over $\Q$. This is a somewhat special example: upon joining one of the roots of $f$ we got all the others for free. This happens in other examples too, but is certainly {\em not} a general principle.

In particular, we see that the degree of $\Q \subseteq \Q(\zeta_n)$ is at most $n$, far less than the bound of $n!$ given by the Proposition above. In fact, it is at most $n-1$ since $f$ factors as $(x-1)(x^{n-1} + \cdots + x + 1)$, and hence the minimum polynomial of $\zeta_n$
is a divisor of $x^{n-1} + \cdots + x + 1$. 

When $n = p$ is prime, then $x^{p-1} + \cdots + x + 1$ is irreducible, as we proved before, and hence it must equal the minimum polynomial of $\zeta_p$. So, in this case, the degree of $\Q \subseteq \Q(\zeta_p)$ is exactly $p-1$, but it can be smaller than $n-1$ in general; for example, when $n = 4$, $\zeta_4= i$ and $[\Q(i): \Q] = 2$. Note that $x^3 + x^2 + x + 1$ factors as $(x^2+1)(x+1)$ and of course $m_{i, \Q}(x) = x^2 + 1$.

The irreducible polynomial $m_{\zeta_n, \Q}(x)$ is known as the {\em $n$-th cyclotomic polynomial}.
***
#### Example – Porism and $(x^3-2)$
Let $L$ be the splitting field of $x^3 - 2$ over $\Q$; so $L = \Q(\sqrt[3]{2}, e^{2 \pi i/3}\sqrt[3]{2}, e^{4 \pi i/3}\sqrt[3]{2})$.

The Porism gives that there is a field automorphism $\s$ of $L$ such that $\s(e^{2 \pi i/3}\sqrt[3]{2}) = e^{4 \pi i/3}\sqrt[3]{2}$. This one is clear – complex conjugation gives such an isomorphism.

It also gives there is a field automorphism $\tau$ of $L$ such that $\tau(\sqrt[3]{2}) = e^{2 \pi i/3}\sqrt[3]{2}$. This is less obvious.
***
#### Example – $\char(\Z)$
$\char(\Z)=0$ and $\char(\Z/n)=n$ for any $n \geq 0$. 
***
#### Example – Derivatives in Characteristic $p$
If $\chr(F) = p$ and $f(x) = x^p +c$ for $c \in F$, then $f'(x) = 0$. So beware that non-constant polynomials can have $0$ derivatives! Observe, however, that this cannot occur in characteristic $0$.
***
#### Example – Separability and $(x^4-x^3-x+1)$
$x^4 -x^3 -x + 1$ is not separable sine $x-1$ is a double root (it factors as $(x^3-1)(x-1) = (x^2+x+1)(x-1)^2$). As predicted by the Theorem, it fails to be relatively prime to its derivative, which is $4x^3 - 3x^2 -1$, since each are divisible by $x-1$. 

$x^3-1$ is separable in $\R[x]$ because it has 3 distinct roots in $\C$, namely $1,\zeta_3,\zeta_3^2$. As predicted by the Theorem, it is relatively prime to its derivative $3x^2$.

Now interpret $x^3 - 1$ as belonging to $(\Z/3)[x]$. Then $x^3 - 1 = (x-1)^3$ is not separable. As predicted by the Theorem, it is not relatively prime to its derivative, which is $0$. 
***
#### Example – $\Z/p(y)$
Let $F$ be a field of characteristic $p > 0$ and assume $a \in F$ is an element such that $a \ne b^p$ for all $b \in F$.Then $x^p - a$ is irreducible but not separable. It is not separable since in $\ov{F}$ we have $x^p - a= (x-b)^p$ where $b^p = a$. Also note that its derivative is $px^{p-1} = 0$. 

It is less obvious that it is irreducible, but we can see that this is indeed the case in a specific example: Take $F = \Z/p(y)$ (the field of fractions of the polynomial ring $\Z/p[y]$) and let $a = y$. In this case, $x^p - y$ is seen to be irreducible, by Eisenstein, but not separable. 
***
#### Example – $F = (\Z/p)(y) \subseteq (\Z/p)(z) = L$
Let $y$ and $z$ be indeterminants. The extension of fields $F = (\Z/p)(y) \subseteq (\Z/p)(z)= L$ given by identifying $y$ with $z^p$ is not separable. Somewhat more precisely, $F$ is isomorphism to the subfield of $L$ consisting of elements of the form $\frac{\sum_i a_i z^{ip}}{\sum_j b_j z^{jp}}$,
with the isomorphism given by sending $\frac{\sum_i a_i y^{i}}{\sum_j b_j y^{j}}$ to $\frac{\sum_i a_i z^{ip}}{\sum_j b_j z^{jp}}$.

Then $z \in L$ is a root of the polynomial $x^p - y \in F[x]$. Moreover since $F$ is the field of fractions of the PID $R = (\Z/p)[y]$ and $y$ is a prime element of $R$, we may apply Eisenstein (and Gauss) to conclude that $x^p - y$ is irreducible in $F[x]$. This proves that
$m_{z, F}(x) = x^p - y$. This polynomial is not separable since in $L[x]$ it is equal to $(x-z)^p$ and hence has a repeated root. (Or, you may use that its derivative is $0$.)
***
#### Example – $\Aut(\C/\R)$
I claim $\Aut(\C/\R)$ has two elements (and so is a cyclic group of order $2$): the identity map on $\C$ and the element $\s$ given as complex conjugation. It is easy to see each of these is an element of $\Aut(\C/\R)$ --- for $\s$, this amounts to the fact that complex conjugation commutes with addition and multiplication of complex numbers (and that it sends $1$ to $1$).

To see these are the only elements of $\Aut(\C/\R)$, suppose $\tau \in \Aut(\C/\R)$. For any $z = a + ib \in \C$, we have $\tau(z) = a + b \tau(i)$ since $\tau|_\R = \id_\R$. Moreover, $-1 = \tau(-1) = \tau(i \cdot i) = \tau(i) \cdot \tau(i)$ and so $\tau(i) = \pm 1$. Thus $\tau = \id$ or $\tau = \s$.
***
#### Example – $\Aut(\Q(\sqrt d)/\Q)$
For any square-free integer $d$, $\Aut(\Q(\sqrt{d})/\Q)$ has order $2$, and its two elements are the identity and the map sending $a + b \sqrt{d}$ to $a - b \sqrt{d}$. Checking that each really is an element of this group and that there are the only two elements in this group is done similarly to the previous example.
***
#### Example – $\Aut$ and $(x^3-2)$
For a more complicated example, let $K$ be the splitting field of $x^3 - 2$ over $\Q$. Recall
$$
K= \Q(\a_1, \a_2, \a_3)
$$
$$
\a_1 = \sqrt[3]{2}, \a_2 = e^{2 \pi i/3}\sqrt[3]{2}, \a_3 = e^{4 \pi i/3}\sqrt[3]{2}.
$$
Let us ponder how big $\Aut(K/\Q)$ could be. Pick any $\s \in \Aut(K/\Q)$.
Since $\s$ is a ring homomorphism, for any $i$ we have 
$$
\s(\a_i)^3 = \s(\a_i^3) = \s(2) = 2
$$
and thus $\s(\a_i)$ is also a root of $x^2 - 2$. In other words, for each $i$ we have $\s(\a_i) = \a_j$ for some $j$.
Moreover, since $K$ is generated as a field extension of $\Q$ by $\a_1, \a_2, \a_3$, 
the action of $\s$ on the three roots completely determines the action of $\s$ on all of $K$. In more detail, every element of $K$ is given taking $\Q$-linear combinations of sums and products and quotients of these roots, and any element of $\Aut(K/\Q)$ preserves
sums, products and $\Q$-linear combinations. 

To summarize, we have proven that there are {\em at most} $3! = 6$ possibilities for $\s$. 
In fact, more is true: The function
$$
\phi: \Aut(K/\Q) \to \Perm(\{\a_1, \a_2, \a_3\})
$$
given by sending $\s \in \Aut(K/\Q)$ to its restriction to the subset $\{\a_1, \a_2, \a_3\}$ is an injective group homomorphism. 
Thus $\Aut(K/\Q)$ is isomorphic to a subgroup of $S_3$. 
I claim that $\# \Aut(K/\Q) = 6$ and hence $\Aut(K/\Q) \cong S_3$.
I will prove this directly – we will learn of fancier methods to do so later.

First we notice that the field automorphism of $\C$ given by complex conjugation, namely $\C \to \C, z \mapsto \overline{z}$, permutes the roots of $x^3 - 2$ and hence it restricts to a field map from $K$ into $K$. Since this map is $\Q$-linear and injective (as are all field maps) and $K$ is a finite dimensional $\Q$-vector space, this map must be onto as well. So, we obtain
an element $\a \in \Aut(K/\Q)$ given by $\a(z) = \overline{z}$ for all $z \in K$. 
It corresponds $(2 \, 3) \in S_3$. 

Next, we apply Porism \ref{por418}, which gives $\gamma \in \Aut(K/\Q)$ such that $\gamma(\sqrt[3]{2})=e^{2 \pi i/3} \sqrt[3]{2}$. 
So, in the numbering above, $\gamma$ corresponds to either $(1 \, 2)$ or $(1 \, 2 \, 3)$ in $S_3$. We don't really know which of these it is. (In fact, both will occur --- the map $\gamma$ is not unique.)
But either way we have proven the claim: For notice that both subsets $\{ (2 \, 3), (1 \, 2)\}$ and $\{ (2 \, 3), (1 \, 2 \, 3)\}$ of $S_3$ generated all of $S_3$. 

In other words, every possible permutation of roots of $x^3 - 2$ arises as a field automorphism of its splitting field over $\Q$. This is what I meant before when I said that the roots of $x^3 - 2$ are "as symmetric as possible''.
***
#### Example – $[L:\Q]$ and $(x^4-2)$
Let $L$ be the splitting field of the irreducible polynomial $q(x) = x^4 - 2 \in \Q[x]$. 
So $L = \Q(R)$ where $R = \{z_1 = \sqrt[4]{2}, z_2 = i \sqrt[4]{2}, z_3= - \sqrt[4]{2}, z_4 = - i\sqrt[4]{2})\}$. 
By the Corollary above, the action of $\Aut(L/\Q)$ on $R$ is faithful so that we have an injective group homomorphism $\Aut(L/\Q) \to \Perm(R)$.

Note that this map cannot possibly be onto: there is no $\s \in \Aut(L/\Q)$ such that 
$\s(z_1) = z_2$, $\s(z_2) = z_1$, $\s(z_3) = z_3$, and $\s(z_4) =z_4$; i.e., the permutation $(1 \, 2)$ of these roots is not realizable by a field automorphism. To see this note that if $\s(z_1) = z_2$ then $\s(z_3) = \s(-z_1) = - \s(z_1) = - z_2 = z_4$. So, any field automorphism that interchanges $z_1$ and $z_2$ would have to also interchange $z_3$ and $z_4$.
In fact, as we shall see, $\# \Aut(L/\Q) = 8$, considerably smaller than $4!$.

Let us compute $[L:\Q]$.
Note that $i \in L$ since $i = z_2/z_1$ and in fact $L = \Q(z_1, i)$. In the chain of extensions
$$
\Q \subset \Q(z_1) \subset L = \Q(z_1)(i)
$$
the first one has degree $4$, since $x^4 - 2$ is irreducible by Eisenstein, and the second has degree at most $2$ since $i$ is a root of $x^2 + 1$. It would be less than two if $x^2+1$ factors in $\Q(z_2)[x]$. But since $\Q(z_1) \subset \R$ and $L$ is not contained in $\R$, the second extension cannot be trivial and so must have degree exactly $2$. We conclude $[L:\Q] = 8$. It follows from Proposition \ref{prop421} that $\# \Aut(L/\Q) \leq 8$.
(In fact, since $L$ is the splitting field of a separable polynomial, the Theorem below will tell us that $\# \Aut(L/\Q) = 8$. But we won't appeal to this fact here.)

We claim $\# \Aut(L/\Q) = 8$ and $\Aut(L/\Q)$ is isomorphic to the subgroup $H$ of $S_4$ generated by $(2 \, 4)$ and $(1 \,2 \, 3 \,4)$. (This is isomorphic to $D_8$.)

The map $\C \to \C$ given by complex conjugation permutes the roots of $x^4 - 2$ and it restricts to an automorphism of $L$ --- specially, it fixes $z_1, z_3$ and interchanges $z_2$ and $z_4$. It follows that complex conjugation determines an element $\s \in \Aut(L/\Q)$ that corresponds to $(2 \, 4) \in H \leq S_4$.

By the degree formula we get $[L: \Q(i)] = 4$. Since $L = \Q(i)(z_1)$, the degree of $m_{z_1, \Q(i)}(x)$ must be $4$. This shows that $x^4 - 2$ must remain irreducible as a polynomial in $\Q(i)[x]$; this is not obvious, but we have now proven it, and this fact will
be useful in what we do next.

To construct another element of $\Aut(L/\Q)$, we use that that $L$ is the splitting field of the polynomial $x^4 - 2$ over $\Q(i)$ and that, as we just showed, $x^4 - 2$ is irreducible in $\Q(i)[x]$. We may thus apply Porism \ref{por418} (also stated in the Corollary) to get that there is an element $\tau \in \Aut(L/\Q(i))$ such that $\tau(z_1) = z_2$. We may regard $\tau$ as an element of $\Aut(L/\Q)$ since, by definition, $\Aut(L/\Q(i))$ is a subgroup of $\Aut(L/\Q)$.
We have
$$
\tau(z_2) = \tau(i z_1) = \tau(i) \tau(z_1) = i z_2 = z_3
$$
since $\tau(i) = i$ by construction. A key point here is that if we had merely specified $\tau$ to be an element of $\Aut(L/\Q)$ sending $z_1$ to $z_2$, then we would have no idea what $\tau$ does to $z_2$ --- it was key to define $\tau \in \Aut(L/\Q(i))$ as we did. We then also get $\tau(z_3) = z_4$ and $\tau(z_4) = z_1$. So $\tau$ corresponds to the permutation $(1 \,2 \, 3 \,4)$.

We have proven that $\Aut(L/\Q)$ is isomorphic to a subgroup of $S_4$ having order at most $8$ (by the Proposition above) and that it contains $(2 \, 4)$ and $(1 \,2 \, 3 \,4)$. Since the subgroup generated by these two elements has order $8$, the claim follows.
***
#### Example – Normal Extension
$L = \Q(\sqrt[3]{2}, e^{2 \pi i/3})$ is a normal extension of $\Q$ since it is the splitting field of $x^3-2$.
***
#### Example – $\Q(\sqrt[3]2)$ not Normal
Is $\Q(\sqrt[3]{2})$ normal? It isn't the splitting field of $x^3 -2$ clearly, but maybe it somehow is the splitting field of some other polynomial. It in fact is not normal,
but it is not so obvious that it isn't. The next Theorem will allow us to prove it isn't normal.
***
#### Example – Galois Extension
$L = \Q(\sqrt[3]{2}, e^{2 \pi i/3})$ is a Galois extension of $\Q$, since it the splitting field of $x^3 - 2$. We proved above that $\Aut(L/\Q)$ has six elements and $[L: \Q] = 6$, as the Theorem predicts. 
***
#### Example – $\Q(\sqrt[3]2)$ not Galois
I claim $L = \Q(\sqrt[3]{2})$ is not a Galois extension of $\Q$. Let $R$ be the set of all roots of $x^3-2$ in $L$. Since $L \subseteq \R$, $R$ has just one element: $R = \{\sqrt[3]{2}\}$. Since $L = \Q(R)$, the function $\phi: \Aut(L/\Q) \to \Perm(R)$ is injective by Proposition \ref{prop423} and so since $\# R = 1$, we have $\# \Aut(L/\Q) = 1$. Thus it isn't Galois. Since it is separable, $L$ must not be a normal extension of $\Q$. 
***
#### Example – Galois and Characteristic $p$
Let $F$ be a field of characteristic $p$, for a prime integer $p$, and assume $L$ is a finite field extension of $F$ such that there exists an element $a$ of $L$ with $a \notin F$ but $a^p \in F$. Then $F \subseteq L$ is not Galois since $\# \Aut(L/K) < [L:K]$ in this case. You will prove this in the Homework.
***
#### Example – FTGT and $(x^4-2)$
Let $L$ be the splitting field of $x^4 - 2$ over $\Q$. Let's use the fundamental theorem to list all intermediate fields for $\Q \subseteq L$ and to determine which are Galois over $\Q$. Notice that without the theorem, it isn't even obvious that there are only a finite number of such intermediate fields. 

We know $G := \Gal(L/\Q)$ corresponds to the $8$ element subgroup of $S_4$
generated by $\s = (2 \, 4)$ and $\tau = (1 \, 2 \,3 \, 4)$ where we number the roots as $\a_1 = \sqrt[4]{2}, \a_2 = i \a_1, \a_3 = -\a_1, \a_4 =-i\a_1$.

This group is isomorphic to $D_8$ and we can make this isomorphism
explicit by labeling the four corners of a square by $\a_1, \dots,\a_4$, counter-clockwise. So, $\tau$ is rotation by $90$ degrees and $\s$ is reflection about the line joining vertices $1$ and $3$.

The subgroup lattice and intermediate field lattice are represented below, with normal subgroups and Galois extensions highlighted (boxed).

The subgroups are
$$
\begin{aligned}
G &= \langle (2 \, 4), (1 \, 2 \, 3 \,4) \rangle \\
\{e\} & \\
H_1 &= \langle (2 \, 4) \rangle \\
H_2 &= \langle (1 \, 3)\rangle \\
H_3 &= \langle (1 \, 2)(3 \, 4)\rangle \\
H_4 & = \langle (1 \,4)(2 \, 3)\rangle \\
H_5 &= \langle (1 \,3)(2 \, 4)\rangle \\
H_6 & = \langle (1 \, 2 \, 3 \,4) \rangle \\
H_7 &= \langle(1 \, 3), (2 \, 4)\rangle \\
H_8 &= \langle (1 \, 2)(3 \, 4), (1 \,4)(2 \, 3)\rangle \\
\end{aligned}
$$
 and the lattices are
 INSERT IMAGE
The intermediate fields are the fixed subfields of $L$ associated to
each of these subgroups. In some sense, this answers the quesiton, but
let's find explicit generators for at least some of these.

$G$ corresponds to $\Q$ and $e$ corresponds to $L = \Q(\a_1, i)$.

Set $E_i = L^{H_i}$. $E_1$ has degree $4 = [G:H_1]$ over $\Q$. It is clear $\a_1$ (and
$\a_3$) belongs to $E_1$ and since $[\Q(\a_1):\Q]=4$, we must have $E_1 = \Q(\a_1)$.

Likewise $E_2 = \Q(\a_2)$.

$E_3$ also has degree four over $\Q$. Let $\beta = \a_1 + \a_2 = (1+i)\sqrt[4]{2}$ and note $\beta \in E_3$. If $[\Q(\beta):\Q] = 2$, then $\beta$ would be fixed by a subgroup of index $2$ that contains $(1 \,2)(3 \, 4)$, and the only possibility is $H_8$. But $(1 \, 4)(2 \, 3)$ sends $\beta$ to $\a_4 + \a_3 = - \beta \ne \beta$. So we must have $[\Q(\beta):\Q] = 4$ and hence $E_3 = \Q(\beta)$.

I'll skip the details on $E_4$ and $E_5$, but they are $E_4 =\Q((1-i)\a_1)$ and $E_5 = \Q(\sqrt{2},i)$.

$E_6$ has degree equal to $[G:H_6] = 2$ over $\Q$ and so we merely need to find a single, non-rational element of $L$ fixed by $\tau$. Since $\tau(i) = i$ (which can be seen by looking back at how we built $\tau$ originally or by noting that $\tau(i) = \tau(\a_2/\a_1) = \a_3/\a_2= i$), we get $E_6 = \Q(i)$.

I'll skip the details on $E_7$, but it is $E_7 = \Q(\sqrt{2})$.

$E_8$ also has degree two over $\Q$ and so we just need to find a single non-rational element fixed by the two generators of $H_8$. Note that $\a_1\a_2 = \a_3\a_4 = i \sqrt{2}$ and so $i \sqrt{2}$ is fixed by both $(1 \, 2)(3 \, 4)$ and $(1 \,4)(2 \, 3)$. Thus $E_8 = \Q(i \sqrt{2})$.

Finally, we note that $G, \{e\}, H_5, H_6, H_7, H_8$ are normal subgroups of $D_8$, since $H_5$ is the center of $D_8$ and each of $H_6, H_7, H_8$ has index two. Some messy checking reveals these to be the only normal subgroups. It follows from the Fundamental Theorem that $\Q, L, E_5, E_6, E_7, E_8$ are the only intermediate fields that are Galois over $\Q$. As an example, to see directly that $E_3$ is not Galois over $\Q$, note that $(1+i)\sqrt[4]{2}$ is a root of $x^4 + 4$, which is irreducible. But $(1-i)\sqrt[4]{2}$ is also a root of this polynomial and it is not in $E_3$. We conclude from Proposition \ref{prop429} that $E_3$ is not a normal extension of $\Q$. 
***
#### Example – Cyclotomic Extensions Revisited
Let $F$ be a field, let $n$ be a positive integer such that $\char(F)$ does not divide $n$, and let $\ov{F}$ be the algebraic closure of $F$. If $\zeta\ov{F}$ is a primitive $n$-th root of 1 over $F$, then $F(\zeta)/F$ is a finite Galois extension, and $\Gal(F(\zeta)/F)$ is a cyclic group that is isomorphic to a subgroup of $(\Z/n,+)$.
***
#### Example – Two Complex Roots and $S_n$
Let $f$ be an irreducible, fifth degree polynomial in $\Q[x]$ with exactly three real roots and let $L$ be its splitting field over $\Q$. Let the real roots be $\a_1, \a_2, \a_3$ and the imaginary ones be $\a_4$ and $\a_5$. Then $G = \Gal(L/\Q)$ is isomorphic to $S_5$. You will prove this on one of the final exam problems (for a specific case), but let me get you started with a couple {\em tips}: Show that $G$ is isomorphic to a subgroup $H$ of $S_5$ with $5 \mid \#H$. You may use (without justifying it) that if $\tau$ is a $2$-cycle in $S_5$ and $\s$ is any five cycle in $S_5$, then the subgroup of $S_5$ they generate is all of $S_5$.
***
#### Example – Finding Unique Intermediate Field
If $F \subseteq L$ is a finite Galois extension of degree $21$, then I claim there is a unique intermediate field $E$ with $[E:F] = 3$ and that $E$ must be a Galois extension over $F$.

To see this, set $G= \Gal(L/F)$. Then $\#G = 21 = 3 \cdot 7$ and by the Sylow theorems, there is a unique Sylow $7$-subgroup, call it $H$, and hence $H$ is normal in $G$. It follows from the Fundamental Theorem that $E := L^H$ is an intermediate field that (a) is Galois over $F$ and (b) satisfies $[E: F] = [G :H] = 3$. Moreover, it is unique since $G$ has just one subgroup of index $3$. 

In fact, there are exactly two groups of order $21$ up to isomorphism, the cyclic one and one that is a (non-trivial) semi-direct product of $\Z/7$ by $\Z/3$. So, there are just two possible lattices of intermediate fields for such a field extension.
***
#### Example – Pre-Calc Example
As every pre-calculus student should know, $f(x) = ax^2 + bx + c \in \Q[x]$ is solvable by radicals. To see this, take $m=1$ and $F_1$ the splitting field of $x^2 - (b^2 - 4ac)$.
***
#### Example – Solvable Quadratic
$f(x) = ax^4 + bx^2 + c \in \Q[x]$ is solvable by radicals over $\Q$.
To see this, note that the roots of $f(x)$ are
$$
\pm \sqrt{\frac{-b \pm \sqrt{b^2 - 4ac}}{2}}.
$$
So, let $m = 3$, set $F_1$ to be the splitting field of $x^2 - (b^2 - 4ac)$ over $\Q$, $F_2$ to be the splitting field of $x^2 - \left(\frac{-b + \sqrt{b^2 - 4ac}}{2}\right)$ over $F_1$, and $F_3$ to be the splitting field of $x^2 - \left(\frac{-b - \sqrt{b^2 - 4ac}}{2}\right)$ over $F_2$. It is not clear if $F_3 = F_2$ or $F_2 \subset F_3$, but, either way, this gives a tower that shows that $f(x)$ is solvable by radicals.
#### Example – $S_5$ and $A_5$ not Solvable
$S_5$ and $A_5$ are not solvable. Every groups of order $< 60$ is solvable.
***