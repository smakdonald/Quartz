## Symmetry
#### $\defn$ – Orthogonal Transformation
A linear transformation $\s : \R^2\to \R^2$ is called *orthogonal* if it is distance preserving; that is, if $|U - V|$ denotes the distance between points $U$ and $V$, then $$|\s(U)-\s(V)|=|U-V|.$$
#### $\lem$ – Orth Transformation Preserves Angles
Every orthogonal transformation $\s$ preserves angles: if $A$, $V$ and $B$ are points, then $\angle AVB=\angle A'V'B'$ where $A' = \s(A)$, $V' =\s (V)$, and $B' = \s(B)$.

#### $\defn$ – Symmetry Group
Given a figure $F$ in the plane, its *symmetry group* $\Sigma(F)$ is the family of all orthogonal transformations $\s:\R^2\to \R^2$ for which $$\s(F)=F.$$The elements of $\Sigma(F)$ are called *symmetries*.

#### $\lem$ – Orth Transformation Permutes Vertices
If $P$ is a polygon, then every orthogonal transformation a $\s\in\Sigma(P)$ permutes $V(P),$ the set of vertices of $P$.

#### $\thm$ – Symmetry Grp Iso to Subgroup of Sn
If $P$ is a polygon with n vertices $V(P)=\{V_1,\dots,V_n\}$, then $\Sigma(P)$ is isomorphic to a subgroup of the symmetric group $S_n$.

#### $\cor$ – Symmetry Groups of Triangles
Let $\triangle$ be a triangle with vertices $A, B$, and $C$. If $A$ is equilateral, then $\Sigma(\triangle)\cong S_3$; if $\triangle$ is only isosceles, then $\Sigma(\triangle)\cong \Z_2$; if $\triangle$ is scalene, then $\Sigma(\triangle)$ has order $1$.

#### Problem
(a) If F is a square, prove that $\Sigma(F)\cong D_8$, the dihedral group of order $8$.
(b) If F is a rectangle that is not a square, prove that $\Sigma(F)\cong \Z_{2}\times\Z_{2}$, 
(c) Give an example of quadrilaterals $Q$ and $Q'$ with $\Sigma(Q)\cong\Z_2$ and $\Sigma(F)=\{e\}$

##### *Proof.*
#### Problem
A polygon is *regular* if all the angles at its vertices are equal. Prove that a polygon $P$ is regular if and only if $\Sigma(P)$ acts transitively on $V(P)$.

##### *Proof.*
#### Problem
Prove that if $P_n$ is a regular polygon with $n$ vertices, then $\Sigma(P)\cong D_{2n}$. 

##### *Proof.*
#### Problem
Prove that if $F$ is a circular disk, then $\Sigma(F)$ is infinite.

##### *Proof.*
## Rings
#### $\defn$ – Ring
![[Ring]]
#### $\defn$ – Commutative Ring
![[Commutative Ring]]
#### $\ex$ – Common Rings
#### $\ex$ – Modular Arithmetic
#### $\ex$ – Polynomial Ring
#### $\defn$ – Root
Let $f(x)=\sum c_{i}x^{i}$ be a polynomial over a ring $R$. A *root* of $f(x)$ in $R$ is an element $\a\in R$ such that $$c_0+c_1\a+\cdots+c_{n}\a^{n}=0.$$
#### $\thm$ – Ring Properties
![[Proposition – Ring Arithmetic]]
#### $\defn$ – Subring
![[Subring]]
#### Problem – Intersection of Subrings
Show that the intersection of any family of subrings of R is a subring.

##### *Proof.*
#### Problem – Binomial Theorem
Prove that the binomial theorem holds in any ring $R$: if $n\geq 1$, then $$(a+b)^{n}=\sum\limits {n \choose i} a^{i}b^{n-1},$$where ${n\choose i}$ denotes the binomial coefficient $\frac{n!}{i!(n-i)!}$. Hint: First prove $${n-1\choose i-1}+{n-1\choose i}={n\choose i}.$$

##### *Proof.*
#### Problem – Primes and Binomial Coefficients
If $p$ is a prime, prove that $p$ is a divisor of $p\choose i$ for $i\neq 0$ and $i\neq p$. (Note
that $4$ is not a divisor of ${4\choose 2}=6$. 

##### *Proof.*
#### Problem – Derivative Properties
If $R$ is a ring and $f(x)\in R[x]$, say, $f(x)=r_{0}+r_{1}x+\dots+r_{n}x^{n}$, define its *derivative* by $$f'(x)=r_{1}+2r_{2}x+\dots+nr_{n}x^{n-1}.$$
Prove that $$(f+g)'=f'+g'$$and $$(fg)'=fg'+f'g$$

##### *Proof.*
#### Problem – Ring of Functions
If $R$ is a ring and $S$ is a set, let $R^{S}$ denote the set of all functions $S\to R$. Equip $R^{S}$ with the operations of pointwise addition and multiplication; that is, if $f,g:S\to R$, then $$f+g:s\to f(s)+g(s)$$and $$fg:s\to f(s)g(s).$$Prove that $R^{S}$ is a ring. (Hint: "Zero" is the constant function $z$ with $z(s)=0$ for all $s\in S$, and "one" is the constant function $e$ with $e(s)=1$ for all $s\in S$.)

##### *Proof.*
## Domains and Fields
#### $\defn$ – Integral Domain
![[Integral Domain]]
#### $\ex$
#### $\thm$ – Cancellation Law in Domains
A ring R isa domain if and only if it satisfies the cancellation law: if $ra = rb$ and $r\neq 0$, then $a = b$.
#### $\thm$ – Domains and Mod
$\Z_n$ is a domain if and only if $n$ is prime.
#### $\defn$ – Unit
![[Unit]]
#### $\defn$ – Field
![[Field]]
#### $\ex$
#### $\thm$ – $\Z_p$ a Field
If $p$ is prime, then $\Z_p$ is a field.
#### $\thm$ – Existence of Fraction Field
#### $\defn$ – Field of Fractions
![[Field of Fractions]]
#### Problem – Group of Units is a Group
Let $R$ be a ring.
(a) Prove that $R^{\times}$, the set of all units in $R$, is a group under multiplication. 
(b) Prove that $R$ is a field if and only if $R\setminus\{0\}$ is a group under multiplication. 

##### *Proof.*
#### Problem – Order of Group of Units
Prove that if $a\in\Z$, then $a$ is a unit in $\Z_n$ if and only if $\gcd(a,n)=1$. Conclude that the group of units, $\Z_{n}^{\times}$ has order $\varphi(n),$ where $\varphi$ is Euler's function. 

##### *Proof.*
#### Problem – Constant Terms in Polynomial Products
Let $f(x),g(x)\in R[x]$. Show that the constant term of $f(x)g(x)$ is the product of the constant terms of $f(x)$ and of $g(x)$.

##### *Proof.*
#### Problem
Let $R$ be an integral domain.

(a) Prove that the leading coefficient of $f(x)g(x)$ is the product of the leading coefficients of $f(x)$ and of $g(x)$. Conclude that if $f(x)$ and $g(x)$ are nonzero polynomials in $R[x]$, then $$\partial(fg)=\partial(f)+\partial(g).$$
(b) Prove that $R[x]$ is also an integral domain.
(c) If $R=\Z_{4}[x]$, show that $(2x+1)^{2}=1$. Conclude that the formula $\partial(fg)=\partial(f)+\partial(g)$ may be false in $R[x]$ when $R$ is not a domain.  
(d) Show that there is a factorization $x=f(x)g(x)$ in $R=\Z_{4}[x]$ in which neither $f(x)$ nor $g(x)$ is a constant.

##### *Proof.*
#### Problem – Polynomial Rings and Domains
Define the ring of polynomials in two variables over $R$, denoted by $R[x,y]$, as $A[y]$, where $A = R[x]$. Define polynomials in several variables over $R$ by induction, and show that if $R$ is a domain, then so is $R[\xdots]$ (one usually denotes $\Frac(F[\xdots])$ by $F(\xdots)$ when $F$ is a field).

##### *Proof.*
#### Problem
Let $R$ be a domain, and let $f, g\in R$ be nonzero elements satisfying $$f=ug\quad \text{ and }\quad g=vf,$$where $u,v\in R$. Prove that $uv=1$ and that $u$ and $v$ are units.

##### *Proof.*
#### Problem – Units in Polynomial Rings
(a) Prove that if $F$ is a field, then the units in $F[x]$ are the nonzero constants.
(b) Show that $\Z_{2}[x]$ is an infinite ring having exactly one unit.
(c) Give an example of a non constant polynomial in $\Z_{4}[x]$ that is a unit.

##### *Proof.*
#### Problem – Division Algorithm for Polynomials
(a) Prove the division algorithm for polynomials: If $R$ is a ring, if $f(x), g(x)\in R[x]$, and if the leading coefficient of $g(x)$ is a unit (in particular, if $g(x)$ is monic), then there are polynomials $q(x)$ and $r(x)\in R[x]$ (quotient and remainder) with $$f(x)=q(x)g(x)+r(x)$$ and either $r(x)=0$ or $\partial(r)<\partial(g)$. 
(b) If $R$ is a domain, then the quotient and remainder occurring in the division algorithm are unique. (There are rings $R$, e.g. $\Z_{4}$, for which the corresponding assertion is false.)

##### *Proof.*
#### Problem – Subfield Test
A *subfield* $F$ of a ring $R$ is a subring of $R$ that is a field. Show that a subset $X$ of a ring $R$ is a subfield if and only if $X$ contains $1$ and $X$ is closed under subtraction, multiplication, and inverses.

##### *Proof.*
#### Problem – Intersections of Subfields
Prove that the intersection of any family of subfields is itself a subfield. (Note that this intersection is not (0) because it contains 1.)

##### *Proof.*
#### Problem – Infinite Domains and Subfields
(a) Show that $\Z_{p}[x]$ is an infinite domain containing $\Z_{p}$ as a subfield.
(b) Show that there exists an infinite field containing $\Z_{p}$ as a subfield.

##### *Proof.*
#### Problem – Polynomial Rings are Not Fields
Show that $R[x]$ is never a field.

##### *Proof.*
#### Problem – Mod Field if Prime
Show that $\Z_n$ is a field if and only if $n$ is prime. 

##### *Proof.*
## Homomorphisms and Ideals
#### $\defn$ – Ring Homomorphism
![[Homomorphism#$ defn$ – Ring Homomorphism]]
#### $\defn$ – Ring Isomorphism
![[Isomorphism#$ defn$ – Ring Isomorphism]]
#### $\ex$
#### $\ex$
#### $\defn$ – Kernel
![[Kernel]]
#### $\defn$ – Image
Image
#### $\defn$ – Ideal
![[Ideal]]
#### $\thm$ – Ideals and Kernels
#### Problem – Properties of Canonical Map in Frac
If $R$ is a field, prove that the map $R\to\Frac(R)$, given by $a\to \frac{a}{1}$, is an isomorphism. Conversely, prove that if $R$ is a domain and the map $a\to \frac{a}{1}$ is an automorphism, then $R$ is a field. 
#### Problem – Isomorphism of Fraction Fields
If $\varphi:R\to S$ is an isomorphism between domains, prove that $\Frac(R)\cong\Frac(S)$, namely $\frac{a}{b}\to\frac{\varphi(a)}{\varphi(b)}$.
#### Problem – Minimality of Fraction Field
Let $R$ be a subring of a field $F$, and let $K$ be the intersection of all the subfields of $F$ that contain $R$. Prove that $K\cong\Frac(R)$.

##### *Proof.*
#### Problem – Composition and Inverse Ring Maps
(a) If $\varphi:R\to S$ is an isomorphism, then If $\varphi\inv:S\to R$ is also an isomorphism
(b) If $\varphi:R\to S$ and $\psi:S\to T$ are ring homomorphisms, then so is their composition.

##### *Proof.*
#### Problem – Ring Maps Preserve Units
If $a\in R$ is a unit and $\varphi:R\to S$ is a ring map, then $\varphi(a)$ is a unit in $S$.

##### *Proof.*
#### Problem – Constant Term Function is Ring Map
(a) If $R$ is a ring, prove that  $\varphi:R[x]\to R$, where $\varphi:f(x)\mapsto c_0$, the constant term of $f(x)$, is a ring map.
(b) What is $\ker(\varphi)$?

##### *Proof.*
#### Problem
(a) #empty 
(b) If $\tau: S\to T$ is a ring map, prove that $(\tau\sigma)^{*}:R[x]\to T[x]$ is equal to $\tau^{*}\s^{*}$.
(c) Prove that if $\s$ is an isomorphism, then so is $\s^{*}$.

##### *Proof.*
#### Problem
(a) The intersection of any family of ideals in $R$ is an ideal in $R$. Conclude that if $X$ is any subset of a ring $R$, there is a smallest ideal, denoted by $(X)$, containing X. One calls $(X)$ the ideal generated by $X$, namely, the intersection of all the ideals in $R$ that contain $X$.
(b) Prove that $(X)$ is the "smallest" ideal containing $X$ in the following sense: $(X)$ is an ideal containing $X$ and, if $J$ is any ideal in $R$ containing $X$, then $(X)\sse J$.

##### *Proof.*
#### Problem #empty 
(a)
(b)

##### *Proof.*
#### Problem – Ideals and Units
Let $u$ be a unit in a ring $R$.
(a) Prove that if an ideal $I$ contains $u$, then $I= R$.
(b) If $r\in R$, then $(ur) = (r)$. In particular, every nonzero principal ideal $(f(x))\sse R=F[x]$, where $F$ is a field, can be generated by a monic polynomial.
(c) If $R$ is a domain and $r,s\in R$, then $(r)=(s)$ if and only if $s=ur$ for some unit $u\in R$.

##### *Proof.*
#### Problem – Fields Have Two Ideals
Prove that a ring $R$ is a field if and only if it has only one proper ideal.

##### *Proof.*
#### Problem #empty 
(a)
(b)

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Quotient Rings
#### $\defn$ – Canonical Map
![[Canonical Map]]
#### $\thm$ – Canonical Map Surjective Homomorphism
![[Lemma – Quotient Map is Surjective Homomorphism]]
#### $\defn$ – Quotient Ring
![[Quotient Ring]]
#### $\ex$
#### $\ex$
#### $\thm$ – First Isomorphism Theorem
![[Theorem – First Isomorphism Theorem#$ thm$ – First Isomorphism Theorem for Rings]]
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Polynomial Rings over Fields
#### $\thm$ – Ideals in $F[x]$ are Principal
#### $\defn$ – PID
![[Principal Ideal Domain]]
#### $\defn$ – Divides
![[GCD]]
#### $\defn$ – Greatest Common Divisor
#### $\thm$ – Euclid's Lemma for Polynomials
#### $\ex$
#### $\cor$ – Euclid's Lemma
![[Lemma – Euclid's Lemma]]
#### $\cor$ – Principal Ideals and GCDs
#### $\thm$ – Euclidean Algorithm
![[Theorem – The Euclidean Algorithm]]
#### $\cor$ – GCDs and Field Extensions
#### $\defn$ – Least Common Multiple
#### $\thm$ – LCM and Field Intersections
#### $\thm$ – Polynomial Division Algorithm
#### $\cor$ – Roots and Factors
#### $\thm$ – Factor Theorem
#### $\ex$
#### $\ex$
#### $\cor$ – Infinite Fields and Polynomial Functions
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Prime Ideals and Maximal Ideals
#### $\defn$ – Irreducible Polynomial
![[Irreducible]]
#### $\defn$ – Prime Ideal
![[Prime Ideal]]
#### $\ex$
#### $\thm$ – Irreducible Polynomials & Prime Ideals
#### $\defn$ – Maximal Ideal
![[Maximal Ideal]]
#### $\thm$ – Prime, Maximal, Domain, Field
![[Theorem – Prime, Maximal, Domain, Field]]
#### $\cor$ – Maximal Ideals are Prime
#### $\thm$ – Prime Ideals Maximal in PIDs
#### $\cor$ – Irreducible Quotients
#### $\defn$ – Splits
#### $\thm$ – Existence of Splitting Field
#### $\defn$ – Repeated Roots
#### $\defn$ – Prime Field
![[Prime Field]]
#### $\thm$ – Characteristic and Prime Fields
![[Proposition – Characteristic and Prime Fields]]
#### $\defn$ – Ring Characteristic
![[Ring Characteristic]]
#### $\lem$ –Properties of Characteristic $p$
#### $\thm$ – Existence of Prime Power Fields
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Irreducible Polynomials
#### $\thm$ – Irreducibility and Ring Maps
#### $\rem$
#### $\ex$
#### $\defn$ – Primitive Polynomial
#### $\lem$ – Gauss's Lemma
#### $\lem$ – Unique Primitive Factorization
#### $\defn$ – Content
![[Content]]
#### $\cor$ – Integer Content
#### $\cor$ – Factorization and Content
#### $\thm$ – Gauss (Irreducible)
#### $\rem$
#### $\thm$ – Eisenstein's Criterion
![[Theorem – Eisenstein's Criterion]]
#### $\rem$
#### $\defn$ – Cyclotomic Polynomial
#### $\cor$ – Prime Cyclotomic Polynomial Irreducible
#### $\cor$ – $x^n-a$ and Irreducibility
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Classical Formulas
#### $\defn$ – Reduced Polynomial
#### $\lem$ – Making Reduced Polynomials
#### $\ex$
#### $\ex$
#### $\rem$
#### $\ex$
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Splitting Fields
#### $\defn$ – Field Extension
![[Field Extension]]
#### $\lem$ – MinPoly is Unique
Let $E/ F$ be a field extension, let $\a\in E$, and let $p(x)\in F[x]$ be a monic irreducible having $\a$ as a root.
(a) $\deg p\leq \deg f$ for every $f\in F[x]$ having $\a$ as a root. 
(b) $p$ is the only monic polynomial in $F[x]$ of degree $\deg(p)$ that has $\a$ as a root.
#### $\defn$ – Degree of Field Extensions
![[Degree of Field Extension]]
#### $\thm$ – Degree of Extension and Basis of Vector Space
Let $p(x) \in F[x]$ be an irreducible polynomial of degree $d$. Then $E = F[x]/(p(x))$ is a field extension of $F$ of degree $d$. Indeed, $E$ contains a root $\a$ of $p(x)$, and a basis of $E$ as a vector space over $F$ is $$\{1\a,\a^{2},\dots,\a^{d-1}\}.$$
#### $\defn$ – Simple Extension
![[Simple Extension and Primitive Element]]
#### $\defn$ – Algebraic Element
![[Algebraic Element]]
#### $\thm$ – Finite Extensions Algebraic
![[Proposition – Finite Extensions are Algebraic]]
#### $\thm$ – The MinPoly Theorem
![[Theorem – Properties of Algebraic Elements]]
#### $\defn$ – Minimum Polynomial
![[Minimum Polynomial]]
#### $\defn$ – Splitting Field
![[Splitting Field]]
#### $\ex$
#### $\thm$ – Existence of Splitting Field
If $F$ is afield, then every polynomial $f(x)\in F[x]$ has a splitting field.
#### $\lem$ – Degree Formula
![[Proposition – The Degree Formula]]
#### $\ex$
#### $\lem$ – UMP for Polynomial Rings
Let $\s:F\to F'$ be an isomorphism of fields, let $\s^{*}:F[x]\to F'[x]$, defined by $\sum r_{i}x^{i}\mapsto\sum\s(r_{i})x^{i}$, be the corresponding isomorphism of rings, let $p(x)\in F[x]$ be irreducible, and let $p^{*}(x)=\s^{*}(p(x))\in F'[x]$. If $\beta$ is a root of $p(x)$ and $\beta'$ is a root of $p^{*}$, then there is a unique isomorphism...
#### $\defn$ – Separable
![[Separable]]
#### $\ex$
#### $\rem$
#### $\thm$ – UMP of Field Extensions
#### $\cor$ – Splitting Fields are Isomorphic
If $f(x)\in F[x]$, then any two splitting fields of $f(x)$ over $F$ are isomorphic via a function fixing fixing $F$ pointwise. 
#### $\cor$ – Unique Prime Power Field
Any two finite fields of order $q=p^{n}$ are isomorphic. 
#### Problem
(a) Let $E/F$ be an extension, and let $\a,\beta\in E$ be algebraic elements over $F$. If $\a\neq0$, prove that $\a+\beta,\a\beta,$ and $\a\inv$ are all algebraic over $F$. (Hint. Use Lemma 49 to prove that $F (\a,\beta)$ is a finite-dimensional vector space over F.)
(b) If $E / F$ is an extension, prove that the subset $$K=\{\a\in E|
\a\text{ is algebraic over }F\}$$is a subfield of $E$ containing $F$.
(c) Define the *algebraic numbers* $\A$ to be the set of all those complex numbers that are algebraic over $\Q$. Prove that $\A/\Q$ is an algebraic extension that is not finite.

##### *Proof.*
#### Problem
Let $F$ be afield. Prove that if $\s$ is an isomorphism of $F(\a_{1},\dots,\a_{n})$ with itself such that $\s(\a_{i})=\a_{i}$ for $i = 1,\dots,n$, and $\s(c)=c$ for all $c\in F$, then $\s$ is the identity. Conclude that if $E$ is a field extension of $F$ and if $\s\tau:F(\a_{1},\dots,\a_{n})\to E$ fix $F$ pointwise and $\s(\a_{i})$ for all $i$, then $\s = \tau.$

##### *Proof.*
#### Problem
if $F\sse B\sse E$ are fields and $E/F$ is finite, then both $E/B$ and $B/F$ are finite, and $[E:F]=[E:B][B:F]$.

##### *Proof.*
#### Problem
If $K=\Z_{p}(t)$, prove that $f(x)=x^{p}-t$ is irreducible in $K[x]$. (Hint. If $E/K$ is a splitting field of $f(x)$, then $x^{p}-t=(x-\a)^{p}$ for some $\a\in E$.)
#### Problem
Show that a field $F$ of characteristic $p$ is perfect if and only if every element of $F$ has a $p\th$ root in $F$.
#### Problem
Show that every finite field $F$ is perfect. (Hint: The function $a\mapsto a^{p}$ is always an injection $F\to F$)
## The Galois Group
#### $\defn$ – Automorphism
![[Automorphism]]
#### $\lem$ – Aut Preserves Roots
Let $f(x)\in F[x]$ and let $E/F$ be an extension field of $F$. If $\s:E\to E$ is an automorphism fixing $F$ pointwise, and if $\a\in E$ is a root of $f(x)$, then $\s(\a)$ is also a root of $f(x)$.
#### $\defn$ – Galois Group
![[Galois Extension]]
#### $\thm$ – Gal Iso to Subgroup of Symmetric Group
If $f(x)\in F[x]$ has $n$ distinct roots in its splitting field $E$, then $\Gal(E/ F)$ is isomorphic to a subgroup of the symmetric group $S_{n}$, and so its order is a divisor of $n!$.
[[Proposition – Automorphisms and Permutations (Fields)]]
#### $\ex$
#### $\thm$ – |Gal| is Degree of Extension
If $f(x) \in F[x]$ is a separable polynomial and if $E / F$ is its splitting field, then $$|\Gal(E/F)|=[E:F].$$
#### $\ex$
#### $\ex$
#### $\lem$ – Gal and Intermediate Fields
#### $\thm$ – Normal Subgroups of Gal
#### $\rem$
The hypothesis that $E/ F$ is a splitting field enters only in showing that $Y$ is surjective. Without this hypothesis, one can prove only that the quotient group is isomorphic to a subgroup of $\Gal(B/ F)$.
#### $\ex$
#### Problem 
Let $f(x)\in F[x]$ be an irreducible polynomial of degree $n$, and let $E/ F$ be a splitting field of $f(x)$.

(a) Prove that $n\, |\, [E : F]$.
(b) Prove that if $f(x)$ is separable, then $n\, |\,|\Gal(E/F)|.$

##### *Proof.*
Let $f(x)\in F[x]$ be an irreducible polynomial of degree $n$, and let $E/ F$ be a splitting field of $f(x)$.
###### Part (a)
Let $\a$ be a root of $f$. As $f$ is irreducible, an associate of it must be the minimum polynomial of $\a$, meaning that $[F(\a):F]=n$. As $E$ is created by adjoining all of these roots to $F$. By the Degree Formula we are gucci. 
###### Part (b)
If $f$ is separable then $[E:F]=|\Gal(E/F)|$ by this Theorem, hence the result follows from Part (a).
#### Problem
Let $f(x)\in F[x]$, let $E/F$ be a splitting field, and let $G=\Gal(E/F)$ be the Galois group.

(a) If $f(x)$ is irreducible, then $G$ acts transitively on the set of all roots of $f(x)$ (if $\a$ and $\beta$ are any two roots of $f(x)$ in $E$, there exists $\s\in G$ with $\s(\a)=\beta$. (Hint: Lemma 50.)
(b) If $f(x)$ has no repeated roots and $G$ acts transitively on the roots, then $f(x)$ is irreducible. Conclude, after comparing with Exercise 2, that irreducible polynomials are analogous to regular polygons. (Hint: If $f(x)=g(x)h(x)$, then the $\gcd(g(x),h(x))= 1$; if $\a$ is a root of $g(x)$ such that $\s(\a)$ is a root of $h(x)$, then $\s(\a)$ is a common root of $g(x)$ and $h(x).$)

##### *Proof.*
Let $f(x)\in F[x]$, let $E/F$ be a splitting field, and let $G=\Gal(E/F)$ be the Galois group.
###### Part (a)
[[Corollary – Automorphisms and Group Actions (Fields)]]
###### Part (b)
Suppose that $G$ acts transitively on the roots of $f(x)$, all of which are distinct. Suppose $f(x)=g(x)h(x)$. Since $f$ has no repeated roots we see $\gcd(g(x),h(x))= 1$. Suppose $\a$ is a root of $g(x)$ and $\beta$ is a root of $h(x)$. As our action is transitive there exists some $\s\in G$ such that $\s(\a)=\beta$. However, $g(x)$ is irreducible, and thus from Part (a) we see that $\s(\a)$ is a root of $g(x)$ as well, contradicting that $g(x)$ and $h(x)$ were relatively prime.
#### Problem
Let $E$ be the splitting field of $f(x)=x^{4}-10x^{2}+1$ over $\Q$. Find $\Gal(E/\Q)$. (Hint. See Exercise 67 and Example 20. The roots of $f$ are $\pm \sqrt{2}\pm \sqrt{3}.)$

##### *Proof.*
Let $F=\Q(\sqrt{2})$ and $K=\Q(\sqrt{3})$. Notice that $x^{2}-2$ is irreducible polynomials in $\Q[x]$ by Eisenstein's Criterion, and thus $[F:\Q]=2$. Notice that $x^2-3$ is irreducible in $F$ as it is a degree 2 polynomial with no roots in $F$. Thus by the degree formula we have $[E:\Q]=4$. 

## Roots of Unity
#### $\lem$ – Unique Subgroups of Cyclic Groups
#### $\thm$ – Integers and Euler's Function
#### $\thm$ – Divisors of Order and Cyclic Groups
#### $\thm$ – Finite Subgroup of Field Units is Cyclic
#### $\cor$ – Roots of Unity form a Cyclic Group
#### $\cor$ – Finite Fields and Cyclic Group of Units
#### $\rem$
#### $\defn$ – Primitive Element
![[Primitive Element]]
#### $\cor$ – Squares in Finite Fields
#### $\ex$
#### $\lem$ – Primitive Elements and Irreducible Polys
#### $\thm$ – Frobenius Automorphism
#### $\rem$
#### $\lem$ – Characteristic and Distinct Roots
#### $\defn$ – Primitive Root of Unity
#### $\thm$ – Extension of Primitive Root is Galois
#### $\ex$
#### $\thm$ – Gal Injection
#### $\cor$ – Prime Degree and Galois Group
#### $\cor$ – Prime Degree and Char $0$
#### Problem
Prove that if $F$ is an infinite field, then its multiplicative group $F^{\times}$ is never cyclic. (Hint. To eliminate the possibility $F^{\times} = \langle w\rangle$, consider the cases of characteristic $0$ and characteristic $p > 0$ separately; the latter case should be further subdivided into cases: $u$ transcendental over the prime field $\Z_{p}$ and $u$ algebraic over $\Z_{p}$.)

##### *Proof.*
Let $F$ be an infinite field, and let $F^{\times}$ denote the group of units of $F$. 

First, suppose $F$ has characteristic $0$. Assume by way of contradiction $F^{\times} = \langle x\rangle$. Let $u\in F^\times$. Thus $u$ has an inverse, $v$, such that $uv=e$. 
## Solvability by Radicals
#### $\defn$ – Radical Extension
#### $\defn$ – Solvable by Radicals
![[Solvable by Radicals]]
#### $\lem$ – Radical Extensions and Primitive Roots
#### $\thm$ – Gal Solvability
#### $\thm$ – Existence of Unsolvable Quintic
#### $\rem$
#### Problem
If $E/ F$ is a radical extension over $F$, then there is a radical tower $$F=B_{0}\sse B_{1}\sse\dots\sse B_{t}$$ with each $[B_{i+1} : B_{i}]$ a pure extension of prime type. (Hint. If $\a^{n}$ and $n= pm$, then there is a tower of fields $F\sse F(a^{p})\sse F(x).)$

##### *Proof.*
#### Problem
Let $B / F$ be a finite extension. Prove that there is an extension $K / B$ so that $K/F$ is a splitting field of some polynomial $f(x) e F[x]$. (Hint. Since $B/ F$ is finite, it is algebraic, and there are elements $\a_{1},\dots,\a_{n}$ with $B = F(\a_{1},\dots,\a_{n})$. If $p_{i}(x)\in F[x]$ is the irreducible polynomial of $\a_{i}$, take $K$ to be a splitting field of $f(x)= p_{1}(x)\cdots p_{n}(x)$.)

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem
Using Exercise 84, prove that any splitting field $K/F$ containing a radical extension $R_{t} / F$ (as in Exercise 83) is itself a radical extension. Conclude that, in the definition of solvable by radicals, one can assume that the last field $B_{t}$, is a splitting field of some polynomial over F.

##### *Proof.*
## Independence of Characters
#### $\defn$ – Character
#### $\defn$ – Independent Characters
#### $\lem$ – Distinct Characters are Independent
#### $\cor$ – Field Automorphisms are Independent
#### $\defn$ – Fixed Field
![[Fixed Field]]
#### $\ex$
#### $\ex$
#### $\lem$ – Degree of Fixed Field Extensions
#### $\thm$ – Degree of Fixed Field and Aut
#### $\cor$ – Uniqueness of Fixed Fields
## Galois Extensions
#### $\thm$ – Equivalent Galois Definitions
![[Theorem – Galois Extension Equivalencies]]
#### $\defn$ – Galois Extension
![[Galois Extension]]
#### $\rem$
#### $\defn$ – Intermediate Field
![[Intermediate Field]]
#### $\defn$ – Conjugate (Intermediate Field)
#### $\thm$ – Conjugates and Galois Extensions
#### $\ex$
#### Problem
If $E / F$ is a Galois extension and $B$ is an intermediate field, then $E/ B$ is a Galois extension.

##### *Proof.*
#### Problem
If $F$ has characteristic $\neq2$ and $E/ F$ is a field extension with $[E : F]= 2$, then $E/F$ is Galois.

##### *Proof.*
#### Problem
Show that being Galois need not be transitive; that is, if $F\sse B \sse E$ and $E/B$ and $B/F$ are Galois, then $E/ F$ need not be Galois. (Hint: Consider $\Q \sse \Q(\a) \sse Q(\beta)$, where a is a square root of $2$ and $\beta$ is a fourth root of $2$.)

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem
Let $E/F$ be a Galois extension and let $p(x)\in F[x]$ be irreducible. Show that all the irreducible factors of $p(x)$ in $E[x]$ have the same degree. (Hint: Use Exercise 84.)

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## The Fundamental Theorem of Galois Theory
#### $\defn$ – Lattice
![[Poset and Lattice]]
#### $\ex$
#### $\ex$
#### $\ex$
#### $\ex$
#### $\lem$ – Order Reversing Bijection and Lattices
#### $\thm$ – FTGT
## Applications
#### $\cor$ – Finite Int. Fields in Gal Ext.
#### $\thm$ – Finite Int. Fields and Simple Extensions
#### $\cor$ – Transitivity of Simple Extensions
#### $\cor$ – Primitive Element Theorem
#### $\cor$ – Gal example
#### $\cor$ – Int. Fields and Abelian Gal
#### $\cor$ – Linearly Disjoint
#### $\thm$ – Fundamental Theorem of Algebra
#### $\cor$ – Polynomials Split in $\C$
#### $\rem$
#### Problem
Let $E/F$ be a Galois extension with $[E:F]>1$. 
(a) Must there be an intermediate field of prime degree over F? (Hint: The alternating group $A_6$ has no subgroups of prime index (see Theorem G.37).)
(b) Same question as in (a) with the added hypothesis that $Gal(E/ F)$ is a solvable group.

##### *Proof.*
#### Problem
Show that $\Z_{p}(x,y)$ is a finite extension of its subfield $\Z_{p}(x^{p},y^{p})$, but it is not a simple extension. 

##### *Proof.*
#### Problem
Let $K=\Z_{p}(t)$ be the field of rational functions, let $f(x)=x^{p}-x-t\in K[x]$, and let $E/K$ be a splitting field of $f(x)$. Prove that $\Gal(E/K)\cong\Z_p$ but that $f(x)$ is not solvable by radicals.

##### *Proof.*
## Galois's Great Theorem
#### $\lem$ – Accessory Irrationalities
#### $\defn$ – Norm (Gal)
#### $\lem$ – Hilbert's Theorem
#### $\cor$ – Prime Gal Ext and Primitive Roots
#### $\cor$ – Primitive Roots and Conjugate Gal
#### $\thm$ – Gal Solvable iff Imbedded in Radical Ext.
#### $\cor$ – Quartics and Below Solvable
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Discriminants
#### $\rem$
#### $\defn$ – Discriminant
#### $\defn$ – Reduced Polynomial
#### $\thm$ – Disc of Poly and Reduced Poly
#### $\cor$ – Disc. and Depressed Cubic
#### $\thm$ – Casus Irreducibilis
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Galois Groups of Quadratics, Cubics, and Quartics
#### $\lem$ – 
#### $\thm$ – Galois Group of Cubics
#### $\ex$
#### $\defn$ – Resolvent Cubic
#### $\thm$ – Finding Resolvent Cubic
#### $\thm$ – Galois Group of Quartic
#### $\rem$
#### $\ex$
#### $\ex$
#### $\rem$
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
#### Problem #empty 

##### *Proof.*
## Group Theory Dictionary
#### $\defn$ – Abelian Group
![[Abelian Group]]
#### $\defn$ – Alternating Group
![[Alternating Group]]
#### $\defn$ – Associativity
For all $x, y, z,$ one has $(xy)z = x(yz)$. It follows that one does not need parentheses for any product of three or more factors.
#### $\defn$ – Automorphism
![[Automorphism]]
#### $\defn$ – Commutativity
For all $x, y$, one has $xy = yx$.
#### $\defn$ – Conjugate Elements
![[Conjugacy Class]]
#### $\defn$ – Conjugate Subgroup
#### $\defn$ – Coset
![[Coset]]
#### $\defn$ – Cyclic Group
![[Cyclic]]
#### $\defn$ – Dihedral Group
![[Dihedral Group]]
#### $\defn$ – Even Permutation
A permutation that is a product of an even number of transpositions. Every $r$-cycle, for $r$ odd, is an even permutation.
#### $\defn$ – Factor Groups
#### $\defn$ – Factor Group V
#### $\defn$ – Generator of Cyclic Group
#### $\defn$ – Group
![[Group]]
#### $\defn$ – Homomorphism
![[Homomorphism]]
#### $\defn$ – Image
![[Image]]
#### $\defn$ – Index
![[Index]]
#### $\defn$ – Isomorphism
![[Isomorphism]]
#### $\defn$ – Kernel
![[Kernel]]
#### $\defn$ – Canonical Map
![[Canonical Map]]
#### $\defn$ – Normal Series
A sequence of subgroups $$\{e\}=G_{n}\sse\dots\sse G_{1}\sse G_{0}=G$$is a *normal series* if each $G_{i+1}$ is a normal subgroup of $G_{i}$. (A subgroup $G_{i}$ may not be a normal subgroup of G.)
#### $\defn$ – Normal Subgroup
![[Normal Subgroup]]
#### $\defn$ – Order
![[Order]]
#### $\defn$ – $p$-group
![[p-group]]
#### $\defn$ – Permutation
![[Cycle]]
#### $\defn$ – Quotient Group
![[Quotient Group]]
#### $\defn$ – Simple Group
![[Simple Group]]
#### $\defn$ – Solvable Group
![[Solvable Group]]
#### $\defn$ – Subgroup
![[Subgroup]]
#### $\defn$ – Generated Subgroup
![[Generator]]
#### $\defn$ – Sylow $p$-Subgroup
![[Sylow p-Subgroup]]
#### $\defn$ – Symmetric Group
[[Symmetric Group]]
## Group Theory Used in the Text
#### $\thm$ – Subgroups of Cyclic Groups are Cyclic
#### $\thm$ – 
#### $\thm$ –
#### $\lem$
#### $\thm$
#### $\lem$
#### $\thm$
#### $\thm$
#### $\thm$
#### $\defn$
#### $\defn$
#### $\thm$
#### $\cor$
#### $\lem$
#### $\thm$
#### $\defn$
#### $\cor$
#### $\lem$
#### $\thm$
#### $\cor$
#### $\lem$
#### $\defn$
#### $\lem$
#### $\thm$
#### $\thm$
#### $\defn$
#### $\lem$
#### $\thm$
#### $\thm$
#### $\lem$
#### $\lem$
#### $\lem$
#### $\rem$
#### $\lem$
#### $\thm$
#### $\lem$
#### $\thm$
#### $\lem$
#### $\cor$
#### $\thm$
#### $\thm$
#### $\lem$
#### $\thm$
#### $\lem$
#### $\thm$
#### $\thm$
## Ruler-Compass Constructions
#### $\defn$
#### $\ex$
#### $\defn$
#### $\lem$
#### $\defn$
#### $\lem$
#### $\thm$
#### $\cor$
#### $\lem$
#### $\lem$
#### $\thm$
#### $\cor$
#### $\rem$
#### $\thm$
#### $\rem$
#### $\cor$
#### $\thm$
## Old-fashioned Galois Theory
#### $\defn$
#### $\thm$
#### $\cor$
#### $\lem$
#### $\defn$
#### $\defn$
#### $\thm$
#### $\cor$
#### $\cor$
#### $\cor$
#### $\cor$
#### $\thm$