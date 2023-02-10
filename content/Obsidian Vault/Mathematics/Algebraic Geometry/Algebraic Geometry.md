## Affine Varieties
### Definition and Basic Properties
#### $\defn$ – Affine Space
![[Affine Space]]
#### $\defn$ – Zero Locus
![[Zero Locus]]
#### $\defn$ – Affine Variety
![[Affine Variety]]
#### Exercise – Drawing Variety
Draw $V_\R(x^2+y^2-z,x+y+z-1)$ (when $k = \R$). (Yes, I realize $\R$ is not [[Algebraically Closed|algebraically closed]]; one instance in which we drop this assumption is when we wish to draw a variety.)
***
#### Exercise – An Affine Variety
Let $V=\{(t,t^2,t^3)|t\in k\}\sse \A^3_k$. Prove $V$ is an [[Affine Variety|affine variety]].

###### Solution:
$V=V(y-x^2,z-x^3,y^3-z^2)$
***
#### Exercise – Not an Affine Variety
Let $V =\{(t,e^t)|t\in\C\}\sse\A^2_\C$. Prove $V$ is not an [[Affine Variety|affine variety]].

###### Solution:
If $f(x,y)\in\C[x,y]$ and $f(t,e^t)=0$ for all $t$, then $f(x,y)=0$, not obvious.
***
#### $\ex$ – Singletons are Affine Varieties
Any singleton $\{(a_1,\dots,a_n)\}$ is an [[Affine Variety|affine variety]], since it is the [[Zero Locus|zero locus]] of the set  
$\{x_1-a_1,\dots,x_n-a_n\}$.
***
#### Exercise – Finite Sets of Points are Affine Varieties
Prove that any finite set of points of $\A^n_k$ for any $n\geq 1$ is an [[Affine Variety|affine variety]].
***
#### Exercise – Are Countable Sets Affine Varieties?
Is a countably infinite set of points in $\A^n_\C$ an [[Affine Variety|affine variety]]?

###### Solution:
No countably infinite subset of an affine space can be a variety. Over the reals we see that no polynomial can have infinite roots. 
***
#### Exercise – Every Subspace is an Affine Variety
Thinking of $\A^n_k$ as a [[Vector Space|vector space]] for once, prove that every linear subspace is an [[Affine Variety|affine variety]]. More generally, show every translate of a linear subspace is an affine variety.
***
#### Exercise – Nonzero "Twople" Not Affine in Infinite Space
Show $S = \A^2_k\setminus \{(0,0)\} = \{(a,b) \in \A^2_k | (a,b)\neq(0,0)\}$ is not an affine variety whenever $k$ is an infinite field. (We will eventually define the more general notion of a “variety”, and we will see that this is a (non-affine) variety.) Is this true when $k$ is a finite field?

###### Solution:
Suppose $f(x,y)\in k[x,y]$ is  $V(f)\supseteq \A^2\setminus\{(0,0\}$ then $f(x,0)=0$ for all $x\neq 0$ and $f(0,y)=0$ for all $y\neq 0$. (if you vanish everywhere except possibly the origin, then $V(f)$ must also contain the origin.
***
#### $\defn$ –Radical Ideal
![[Radical Ideal]]
#### $\prop$ – Locus of a Set and Radical are Equal
![[Proposition – Locus of a Set and Radical are Equal]]
#### $\prop$ – Properties of Zero Loci
![[Proposition – Properties of Zero Loci]]
#### $\thm$ – Hilbert's Basis Theorem
![[Theorem – Hilbert’s Basis Theorem]]
#### $\cor$ – Affine Variety is Zero Locus
![[Corollary – Affine Variety is Zero Locus]]
#### $\defn$ – Vanishing Set
![[Vanishing Set]]
#### $\prop$ – Vanishing Set is Radical
![[Proposition – Vanishing Set is a Radical Ideal]]
#### $\prop$ – Unions of Vanishing Sets
![[Proposition – Unions of Vanishing Sets]]
#### Exercise – 
Find a counter-example to the “obvious guess” that $I(W\cap W') = I(W) + I(W')$ for $k=\R$.
***
#### $\prop$ – Compositions of Vanishing Sets and Zero Loci
![[Proposition – Compositions of Vanishing Sets and Zero Loci]]
### Hilbert's Nullstellensatz
#### $\thm$ – Strong Nullstellensatz
![[Theorem – Strong Nullstellensatz]]
#### Exercise – 
Prove: If $k$ is algebraically closed, then for any set $S$ of polynomials we have $I(V (S)) = \sqrt{\langle S\rangle}$. In particular, $I(V(J))=\sqrt{J}$ for any ideal $J$. Moreover, if $T$ is any subset of  $\A^n_k$, $V(I(T))$ is the unique smallest affine variety in $\A^n_k$ that contains $T$.
***
#### $\rem$ 
The key part of the Theorem is the following statement: Suppose $f$ is a polynomial and $J$ is an ideal such that $f\in I(V(J))$. Then some power of $f$ belongs to $J$. A more classical form of this is the following:

Suppose $f$ and $g_1,\dots,g_m$ are polynomials such that whenever $P$ is a zero of each of  $g_1,\dots,g_m$, $P$ is also a zero of $f$. Then $f^{k}=\sum_{i}h_{i}g_{i}$ for some $k\geq1$ and some $h_i$’s.

In other words, if, starting with the system of equations $g_1 = 0,\dots,g_m = 0$, adding on $f = 0$ has no effect on the solution set, then it is because the new equation is an “algebraic consequence” of the previous — that is, some power of $f$ is a $k[x_1,\dots,x_n]$-linear combination of the $g_i$’s. (Note that the converse is obvious, and holds for any field: if $f = 0$ is an “algebraic consequence” of the previous equation, then adding it has no effect on the solution set.)
***
#### $\ex$ – 
Let us show that the assumption that $k$ be algebraically closed is necessary in the Nullstellensatz. Take $J = (x^2 + 1)\sse \R[x]$. Then $J$ is a prime ideal (why?) and hence radical, and yet $V(J) = \emptyset$. So $I(V(J))=\R[x]\neq J$. For an Example –  where $n > 1$, take $J = (x^{2} + y^{2} + 1)\sse \R[x,y]$. Then $J$ is a prime ideal (why?) and yet $V(J)$ is empty, so that $I(V(J))=\R[x,y].$
***
#### Exercise – 
Prove that $I(V(J))=J$ holds for all radical ideals if and only if $k$ is algebraically closed.
#### $\thm$ – Abstract Nullstellensatz
![[Theorem – Abstract Nullstellensatz]]
#### $\rem$
When $n = 1$, the Abstract Nullstellensatz Theorem is clear, since every maximal ideal of $k[x]$ has the form $\langle p(x)\rangle$ for an irreducible polynomial $p$.
***
#### $\rem$
An even more abstract but equivalent form of this theorem is: Given a field extension $k\sse L$, if $L$ is finitely generated as a $k$-algebra then $[L : k] < \infty$.
***
#### $\cor$ – Maximal Ideals in Algebraically Closed Fields
![[Corollary – Maximal Ideals in Algebraically Closed Fields]]
#### $\rem$
When $n = 1$, the Corollary –  holds essentially by definition of “algebraically” closed: If $m$ is any maximal ideal of $k[x]$, then $m= \langle p(x)\rangle$ for a unique irreducible, monic polynomial $p(x)$. If $k$ is algebraically closed, $p(x)$ must be linear and thus of the form $(x-a)$ for some $a\in k$.
***
#### $\rem$
The proof shows, more generally, that for any field $k$, there is a bijection between $\A^n_k$ and the subset of those maximal ideals $m$ in $k[x1,...,xn]$ for which the canonical map of fields $k \to k[x_{1},\dots,x_{n}]/m$(defined by composition) is an isomorphism.
***
#### $\cor$ – Ideals in Algebraically Closed Fields
![[Corollary – Ideals in Algebraically Closed Fields]]
***
#### $\rem$
Since $V(J)=V(\sqrt{J})$ the Corollary implies that $$\operatorname{mSpec}(k[x_{1},\dots,x_{n}]/J)\cong \operatorname{mSpec}(k[x_{1},\dots,x_{n}]/\sqrt{J}).$$This can be proven via more elementary means.
***
#### $\cor$ – Weak Nullstellensatz
![[Corollary – Weak Nullstellensatz]]
***
#### $\lem$ – Algebras and Localizations
![[Lemma – Algebras and Localizations]]
#### $\cor$ – Vanishing Set of Intersection of Varieties
![[Corollary – Vanishing Set of Intersection of Varieties]]
#### $\ex$
The Corollary is false over $\R$: Take $W = V(y-x^2)$ and $W' = V(y+1)$ in $\A^2_\R$. Then $I(W) = \igen{y-x^2}$ and $I(W') = \igen{y+1}$ (why?) and hence 
$\sqrt{I(W) + I(W')} \subsetneq k[x,y]$ (since $$k[x,y]/(y-x^2, y+1) \cong k[x]/(x^2+1) \ne 0).$$But  $W \cap W' = \emptyset$ and so $I(W \cap W') = k[x,y]$.
#### $\defn$ – Coordinate Ring
![[Coordinate Ring]]
#### $\prop$ – Coordinate and Polynomial Ring
![[Proposition – Coordinate and Polynomial Ring]]
#### $\cor$ – Relative Nullstellensatz
![[Corollary – Relative Nullstellensatz]]
### The Zariski Topology
#### $\defn$ – Zariski Topology
![[Zariski Topology]]
#### $\rem$
The Zariski topology on $\A^n_k$ is not Hausdorff (provided $n > 0$). Indeed, the intersection of any two non-empty open sets is non-empty. This is equivalent to the assertion that the union of any two proper closed subset is proper. Using the Nullstellensatz, this is equivalent to the assertion that if $I$ and $J$ are any two non-zero ideals of $k[\xdots]$ then $I \cap J$ is non-zero, and that holds since $k[\xdots]$ is a domain.
#### $\prop$ – Affine Varieties are Compact
![[Proposition – Affine Varieties are Compact]]
#### $\prop$ – Affine Varieties are Noetherian
![[Proposition – Affine Varieties are Noetherian]]
#### $\defn$ – Irreducible Affine Variety
![[Irreducible Affine Variety]]
#### Exercise
Assume $f \in k[\xdots]$ is a polynomial without repeated factors. Prove $X = V(f)$ is irreducible if and only if $f$ is irreducible. Why did I assume $f$ has no repeated factors?
#### Exercise
Show an affine variety $X$ is irreducible iff every non-empty open subset $U$ of $X$ is dense in $X$ (i.e., the intersection of $U$ with any other non-empty open subset of $X$ is non-empty). 

##### *Solution:*
If $U\cap V$ was empty, $(U\cap V)^{C}=U^{C}\cup V^{C}=X$. Since $U^{C}$ and $V^{C}$ are closed, this shows that 𝑋 is reducible. 
#### $\prop$ – AV Irreducible iff Coor. Integral Domain
![[Proposition – AV Irreducible iff Coor. Integral Domain]]
#### $\cor$ – AV Finite Union of Irreducible Closed Subsets
![[Corollary – AV Finite Union of Irreducible Closed Subsets]]
#### $\rem$
In general, if $X$ is any noetherian topological space (i.e., a space with dcc for closed subsets), then the conclusion of the previous Corollary holds. The existence is given as follows: If $X$ is irreducible, then we may take $m = 1$ and $X_1 = X$. If not, then $X = X_1 \cup X_2$ for two proper closed subsets $X_1$ and $X_2$ of $X$. If both $X_1$ and $X_2$ are irreducible, we are done; otherwise we can decompose at least one of them. This process must stop after a finite number of steps since $X$ is noetherian, and thus $X = X_1 \cup \cdots \cup X_m$ for some irreducible closed subsets $X_1, \dots, X_m$. If $X_i \subseteq X_j$ for some $i \ne j$, delete $X_i$ from the list. 
I'll skip a proof of uniqueness.
#### $\ex$
Consider $X = V(xy, xz) = V(x) \cap V(y,z)$ in $\A^3_k$. That is $X$ is the union of a line and a plane, specifically the the $x$-axis and the $yz$-plane. Then $X$ has two irreducible components, the line and the plane.
#### $\ex$
For $f \in k[\xdots]$, the irreducible components of $V(f)$ are $V(g_1), \dots, V(g_m)$ where $f = \prod_i g_i^{e_i}$ for $e_i \geq 1$ and $g_i$ irreducible. 
#### $\defn$ – Distinguished Open Set
![[Distinguished Open Subset]]
#### Exercise
Let $X$ be any [[Affine Variety|affine variety]]. Show the intersection of any two [[Distinguished Open Subset|distinguished]] open subsets of $X$ is again distinguished. Show that the collection of distinguished open subsets of an affine variety $X$ form a "basis'' for the Zariski topology on $X$. Recall that a collection of subsets $\cB$ for a set $T$ is a *basis* for a topology if:
- for every point $P$ there is a $U \in \cB$ with $P \in U$ and
- whenever $P \in U_1 \cap U_2$ for some $U_1, U_2 \in \cB$, there is a $U_3 \in \cB$ such that $P \in U_3 \subseteq U_1 \cap U_2$.
and the topology generated by such a basis is the collection of subsets of $T$ that are arbitrary unions of members of $\cB$. So, you are being asked to show the above two properties hold for the collection of distinguished open sets and that every Zariski open set is a union of distinguished ones. 
### Dimension
#### $\defn$ – Dim (Noetherian Topological Space)
![[Dim (Noetherian Top Space)]]
#### $\defn$ – Codimension
![[Codimension]]
#### $\rem$
Topologize $\N$ by declaring a subset to be closed if and only if it is of the form $\{0, 1, \dots, n\}$ for some $-1 \leq n \leq \infty$. Then $\N$ is a noetherian space but has infinite dimension. There exist noetherian commutative rings $R$ such that $\dm \Spec(R) = \infty$. (This cannot occur for local rings nor for rings tha are finitely generated as $k$-algebras.) 
#### $\rem$
Observe that every maximal chain of irreducible closed subsets (i.e., every chain that cannot be made longer and inserting new terms) of $X$ has $Y_n$ equal to an irreducible component of $X$ and has $Y_0$ equal to a single point. In particular, $$\dm(X) = \max \{\dm(Y) \mid \text{$Y$ is an irreducible component of $X$}\}$$and $$\dm(X) = \max \{\codim_X(P) \mid \text{$P$ is any point of $X$}\}.
$$
#### $\ex$
Let $X = V(xy,xz)$, the union of the $x$-axis and the $yz$-plane. The dimension of $X$ is two. It is clearly at least two, since we have the chain with $Y_0$ being any point on the $yz$-plane, $Y_1$ being any line in this plane and containing this point, and $Y_2$ being the whole plane. It is harder to see that it is at most two. 

This is an example of a variety that fails to be equidimensional–the variety has two irreducible components, but they have different dimensions.

Let $Y = V(x) \subseteq X$, the $yz$-plane. Then $\codim_X(Y) = 0$ since the only closed subsets strictly between $Y$ and $X$ are given by $Y$ together with a finite set of  points on the line. 

Let $Z = V(y,z)$, the $x$-axis. Then $\codim_X(Z)$ is also $0$ by similar reasoning. Since $\dm(Z)  = 1$, this is a bit counter-intuitive. 

Let $W = V(x,y,z)$. When $\codim_X(W) = 2$. It's at least two since we have the chain $W \subsetneq V(x,y) \subsetneq Y \subseteq X$; it is less obvious, but true, that it is exactly two. 

According to Remark \ref{rem131}, what is $\codim_{\A^3}(X)$? 
#### $\ex$
The dimension of $\A^n_k$ is clearly at least $n$ since $$
\emptyset \ne \A^0_k \subsetneq \A^1_k \subsetneq \A^3_k \subsetneq \cdots \subsetneq \A^{n}_k. $$It is much less obvious that it is exactly $n$.
#### $\prop$ – Dim of AV Equal to Dim of Coord. Ring
![[Proposition – Dim of AV Equal to Dim of Coord. Ring]]
#### $\thm$ – Properties of Dimension
![[Theorem – Properties of Dimension]]
#### Exercise
What goes wrong if we don't assume $X$ and $Y$ are irreducible?
#### $\cor$ – Dimension of Affine Space
![[Corollary – Dimension of Affine Space]]
#### $\cor$ – Codimension of Points
![[Corollary – Codimension of Points]]
#### $\cor$ – Dimension and Irreducible Components
![[Corollary – Dimension and Irreducible Components]]
#### $\ex$
Take $X = V(xy, xz)$. Let $f = x-1$. Then $\dm V_X(f) = 0 = \dm(X) - 2$. Why doesn't this contradict the Corollary? Let $g = x$. Then $\dm V_X(g) = 2 = \dm(X)$. Why doesn't this contradict the Corollary? Let $h = y-z$. Then the Corollary does apply, and we have $V_X(h) = 1 = \dm(X) -1$.  
#### $\ex$
Note that if $X = V_{\R}(z - x^2 - y^2)$ and $f = z$, then $X \cap V_{\R}(f) = \{(0,0,0)\}$. Why does this not contradict Krull's Theorem?
#### Exercise
Assume $X$ be any affine variety. Let us an element $f \in A(X)$ {\em geometrically regular} if the assumptions of the Corollary hold: $\emptyset \subsetneq V_X(f) \cap Y \subsetneq Y$ for each irreducible component $Y$ of $X$. Call a sequence of elements $f_1, \dots, f_c \in A(X)$ a {\em geometrically regular sequence} if $f_i$ (or, more accurately, its image in $A(V_X(f_1, \dots, f_{i-1}))$) is geometrically regular on $V_X(f_1, \dots, f_{i-1})$ for each $1 \leq i \leq c$. 

Prove that if $X$ is an equidimensional affine variety (i.e., each irreducible component of $X$ has the same dimension), then 
$$\dm(X) = \min\{d \mid \text{$V_X(f_1, \dots, f_d)$ is a finite set for some geometrically regular sequence $f_1, \dots, f_d \in A(X)$}\}.$$
*Tip*: You might need to use prime avoidance.
### Regular Functions
#### $\defn$ – Regular Function
![[Regular Function]]
#### $\prop$ – Regularity and Finite Open Covers
![[Proposition – Regularity and Finite Open Covers]]
#### $\ex$
Every element of $A(X)$ determines a regular function on every open subset of $X$. (In the notation of Proposition \ref{prop127}, given $f \in A(X)$ and $U$, take $m = 1$, $U_1 = U$, $g_1 = 1$ and $f_1 = f$.) 
That is, there is a ring map $$A(X) \to \cO_X(U).$$
Moreover, so long as $U$ is dense (e.g., if $X$ is irreducible and $U$ is non-empty), then this map is injective. (Proof: If $f$ is in the kernel, then $V_X(f) \supseteq U$ or equivalently $D_X(f) \cap U = \emptyset$. Since $U$ is dense, $D_X(f) = \emptyset$ and thus $V_X(f) = A(X)$. By the Relative Nullstellensatz,   this can only occur when $f = 0$ in $A(X)$.)

We will prove below that this map is in fact an isomorphism when $U = X$ --- that is, there are no "interesting'' regular functions on affine varieties.
#### $\ex$
Suppose $U = D_X(g)$ is a distinguished open subset of an affine vareity $X$ for some $g \in A(X)$. Then every element of the ring $A(X)[1/g]$ deteremines a regular function on $U$. (In the notation of Proposition \ref{prop127}, given
$\frac{f}{g^m}$ with $f \in A(X)$, take $m = 1$, $U_1 = U$ and $f_1 = f$ and $g_1 = g^m$.) This gives a ring map $$A(X)[1/g] \to \cO_X(D_X(g))$$Moreover, it is injective. (Proof: If $\frac{f}{g^m}$ determines the zero function on $U$, then $D_X(f) \cap D_X(g) = \emptyset$ and hence $X = V_X(f) \cup V_X(g) = V_X(fg)$. By the Relative Nullstellensatz, $fg = 0$ in the ring $A(X)$. This implies $\frac{f}{g^m} = 0$ for all $m$ in the ring $A(X)[1/g]$.)

This map will also be shown to be onto below, so that the only regular functions on a distinguished open subset are the "obvious ones''.
#### $\ex$
Let $X = V(xw - yz) \subseteq \A^4_k$ and $U$ be the open subset of $X$ given by 
$$U = X \setminus V(y, w) = X \setminus (V(y) \cup V(w)) = \{(x,y,z,w) \in \A^4_k \mid \text{$xz = yw$ and ($y \ne 0$ or  $w \ne 0$)}\}.$$
Define $\alpha: U \to \A^1_k$ by the following rule: Set $U' = U \setminus V(y) = \{(x,y,z,w) \in U \mid y \ne 0\}$ and $U'' = U \setminus V(w) = \{(x,y,z,w) \in U \mid w \ne 0\}$, and note that $U = U' \cup U''$. Define $$\alpha(x,y,z,w) =
\begin{cases}
\frac{x}{y} & \text{if $(x,y,z,w) \in U'$ and } \\
\frac{z}{w} & \text{if $(x,y,z,w) \in U''$;}\\
\end{cases}$$that is, $$\alpha(x,y,z,w) =
\begin{cases}
\frac{x}{y} & \text{if $y \ne 0$, and} \\
\frac{z}{w} & \text{if $w \ne 0$.} \\
\end{cases}$$Then $\alpha$ is a well-defined function, since whenever $y\ne 0$
and $w \ne 0$ (i.e., for points in $U' \cap U''$) we have $\frac{x}{y} = \frac{z}{w}$ thanks to the defining equation  for $X$. Moreover, $\alpha$ is regular since $U = U' \cup U''$ and on each of $U'$ and $U''$ it is given by a quotient of polynomials.
  
But $\alpha$ **cannot** be represented by any polynomial or even any rational function; that is, there do not exist $f, g \in A(X)$ such that $\alpha(P) = \frac{f(P)}{g(P)}$ for all $P \in U$. In other words, in the notation of Proposition \ref{prop127}, the smallest value of $m$ that can be used to describe $\alpha$ is $m = 1$. I will perhaps prove this later.
