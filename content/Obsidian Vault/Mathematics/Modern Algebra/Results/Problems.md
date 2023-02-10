## Fall 2022
### Homework 1
#### Problem – Center of Dihedral Groups
Find $Z(D_{2n})$ for $n \geq 3$. Your answer will depend on whether $n$ is even or odd.

##### *Proof.*
***
#### Problem
Let $G, H$ be [[Group|groups]] and let $x, y$ be elements of $G$.
(a) Prove that $|x|=\left|\{x^n \ | n\in \Z \}\right|$ and in particular $|x| \leq |G|$. (Defs: [[Order]], [[Subgroup]])
(b) Prove or disprove: if $x,y$ have finite order then $xy$ has finite order.
(c) Prove that if $f:G \to H$ is a group [[Isomorphism|isomorphism]], then $|x| = |f(x)|$.

##### *Proof.*
###### Part (a)
Let $G$ be a group and let $x\in G$. Suppose $|x|=m$. Thus $x^m=e$. 

Suppose by way of contradiction $x^k=x^\ell$ with $k,\ell<m$. Without loss of generality, let $k<\ell$. Notice 
$$\begin{aligned} x^k &=x^\ell\\ (x^k)\inv\cdot x^k &=(x^k)\inv\cdot x^\ell\\ e&=x^{\ell-k},\end{aligned}$$
Contradicting the fact that $m$ is the smallest power of $x$ that yields the identity. Thus each $x^k$ with $k<m$ is distinct, making $\left|\{x^n \ | n\in \Z \}\right|\geq |x|$. 

Notice now that $x\inv=x^{m-1}$, given that multiplying either by $x$ yields $e$ and that inverse elements are [[Proposition – Unique Inverse|unique]].  

Suppose $\left|\{x^n \ | n\in \Z \}\right|> |x|$. Then there exists some $n\in \Z$ such that $x^n$ is distinct 

***
###### Part (b)
***
###### Part (c)
***
#### Problem 
Let $G$ be a group.
1. Let $g \in G$ be an element of finite order. Show that $g^m$ has finite order for any integer $m \geq 0$, and in fact $$ |g^m| = \frac{\lcm(m,|g|)}{m} = \frac{|g|}{\gcd(m, |g|))}.$$
2. Prove that for all $g, h$ in $G$, $|gh| = |hg|$ holds.

##### *Proof.*
***
#### Problem 
Decide whether the groups $Q_8$ and $D_8$ are isomorphic or not, with justification.

##### *Proof.*
***
#### Problem 
1. Find, with justification, an injective group homomorphism $f:S_n \to \GL_n(\R)$.
2. Find, with justification, an injective group homomorphism $g:D_{2n}\to S_n$.

##### *Proof.*
***
### Homework 2
#### Problem – Done
Prove that, for any [[Group|group]] $G$, the set $\Aut(G)$ is a group under composition of functions.

##### *Proof.*
Let $G$ be a group, and consider the set of automorphisms of $G$, denoted $\operatorname{Aut}(G)$. We will show that $\operatorname{Aut}(G)$, is a group under composition.

First, let $f,g$ be functions in $\operatorname{Aut}(G)$. To show that $\operatorname{Aut}(G)$ is closed, we will show that the function the $g\circ f$ is an automorphism of $G$. Let $a,b\in G$, and observe: 
$$\begin{align*}
    g\circ f(ab) & =g(f(ab)\\
    & =g\big(f(a)f(b)\big)\\
    & =g\big(f(a)\big)g\big(f(b)\big)\\
    & =g\circ f(a)g\circ f(b),
\end{align*}$$
showing that the function $g\circ f$ is operation preserving.

Now we will show that $g\circ f$ is injective. Let $x,x'$ be elements in $G$ such that $g\circ f(x)=g\circ f(x')$. Thus $g(f(x))=g(f(x'))$. As $g$ is an automorphism, it is injective, thus $f(x)=f(x')$. As $f$ is an automorphism, it is injective, thus $x=x'$. Therefore $g\circ f(x)=g\circ f(x')$ implies that $x=x'$, proving that $g\circ f$ is injective.

Next, we show that $g\circ f$ is surjective. Let $x\in G$. As $g$ is surjective, there exists some element $x'\in G$ such that $g(x')=x$. As $f$ is also surjective, there exists some element $x''\in G$ such that $f(x'')=x'$. Thus $g\circ f(x'')=g(f(x''))=g(x')=x$, proving that $g\circ f$ is surjective.

Therefore, it follows that $g\circ f$ is an automorphism of $G$, meaning $g\circ f\in\operatorname{Aut}(G).$

The binary operation on $\operatorname{Aut}(G)$ is associative since composition of functions is associative, so that one's easy.

For the identity of $\operatorname{Aut}(G)$, consider the identity function $1_G:G\rightarrow G$. It is easily seen that the identity function is an automorphism of $G$. Let $f$ be a function in $\operatorname{Aut}(G)$. We will show that $f\circ 1_G=f=1_G\circ f$. As all functions share the same domain and co-domain, we need only show that the functions map elements equally, Let $x \in G$, and observe:
$$\begin{align*}
    f\circ 1_G(x) & =f(1_G(x))\\
    & =f(x)\\
    & =1_G(f(x))\\
    & =1_G\circ f(x),
\end{align*}$$
proving that $1_G$ is the identity element of $G$.

Thus, all that remains is to show that every element of $G$ has an inverse in $G$. Let $f\in G$. As $f$ is an automorphism it is a bijective function, meaning it has some inverse $f\inv:G\rightarrow G$. As $f\inv$ is also bijective on $G$, all that remains is to show that $f\inv$ is operation preserving. Let $a,b\in G$. As $f$ is bijective, there exist distinct $x,y\in G$ such that $f(x)=a$ and $f(y)=b$. Thus we see that $f\inv(a)=x$ and $f\inv(b)=y$. With that in mind, consider: 
$$\begin{align*}
    f\inv(ab)& =f\inv(f(x)f(y))\\
    & =f\inv(f(xy))\\
    & =xy\\
    & =f\inv(a)f\inv(b),
\end{align*}$$
proving that $f\inv$ is operation preserving as well. Hence $\operatorname{Aut}(G)$ is closed, associative, has an identity, and contains inverses for each element. Thus $\operatorname{Aut}(G)$ is a group under composition.
***
#### Problem 
Prove that if groups $G$ and $H$ are isomorphic then:
1. $Z(G)\cong Z(H)$ and
2. $\Aut(G)\cong \Aut(H)$.

##### *Proof.*
***
#### Problem
Assume that a [[Group|group]] $G$ [[Group Action|acts]] on a set $S$ via a an action denoted $\cdot$.
1. Prove that the relation $\sim$ on $S$ defined by $$s \sim s' \text{ if and only if } g \cdot s = s' \text{ for some } g \in G$$is an equivalence relation on $S$.
2. Prove that for any $s,s'\in S$ either $\Orb_G(s)=\Orb_G(s')$ or $\Orb_G(s)\cap \Orb_G(s')=\emptyset$. (See: [[Orbit]])
3. Prove that $S$ is a union of pairwise disjoint orbits of the given action.

##### *Proof.*
***
#### Problem – Done
Prove [[Theorem – Lagrange's Theorem|Lagrange's Theorem]]: If $H$ is a [[Subgroup|subgroup]] of a finite group $G$, then $|H|$ (See: [[Order]]) divides $|G|$.
*Hint*: Let $H$ [[Group Action|act]] on $G$ by left multiplication, that is, define $h \cdot g= hg$ for any $h\in H$ and $g\in G$. You may use without checking that this is a group action. Apply the previous problem.

##### *Proof.*
Let $G$ be a finite group, suppose $H\leq G$, and let $H$ act on $G$ by left multiplication. Let $h\in H$. By its definition, the orbit of $h$ under this action is the set $\Orb_H(g)=\{hg|h\in H\}$. Notice that under this action, each of the orbits corresponds to a left coset of $H$ in $G$.  By part (c) of this [[Lemma – $bigcap$s and $bigcup$s of Orbits|lemma]], $G$ is the union of pairwise disjoint orbits of this action. and thus $|G|=\sum_{g\in G}|\Orb_H(g)|$ for distinct orbits. By this [[Lemma – Cosets Partition the Group|lemma]], all cosets have the same cardinality (the cardinality of $H$ itself), and thus each of the orbits in this relation have the same order, and thus we have $|G|=\sum_{g\in G}|H|$ for distinct orbits. Let $x$ denote the number of distinct orbits in this action. Thus we have $|G|=|H|\cdot x$. Hence $|H|$ divides $|G|$. 
***
#### Problem 
1. Prove that any permutation is a product of pairwise disjoint cycles.
2. Prove that the order of a permutation is the least common multiple of the lengths of the cycles it is a product of.
{\em Hint}: Let $S_n$ act on $S=\{1,\ldots, n\}$ in the obvious way, that is, $\sigma\cdot i=\sigma(i)$ for $\sigma\in S_n, i\in S$. You may use without checking that this is a group action. You may also use without proof the fact stated in class that disjoint cycles commute.

##### *Proof.*
***
### Homework 3
#### Problem 
Prove that if $f:G\to H$ is a group homomorphism and $K\leq H$ then the preimage of $K$, defined as $f^{-1}(K)=\{g\in G | f(g)\in K\}$, is a subgroup of $G$.
##### *Proof.*
***
#### Problem 
Consider the set $\mu=\{z\in \C \setminus \{0\} \mid z^n = 1 \text{ for some integer }n \geq 1\}$, which is a subgroup of $( \C \setminus \{0\} , \cdot)$ (a fact you need not prove).
1. Prove that for each integer $m \geq 1$, there is a unique subgroup $H_m\leq \mu$ with $|H_m|=m$ and that $H_m$ is cyclic.
2. Prove that every finitely generated subgroup of $\mu$ has finitely many elements.
3. Prove that $\mu$ is not finitely generated.

##### *Proof.*
***
#### Problem
Prove that if $m,n$ are positive integers such that $\gcd(m,n)=1$ then there is a group [[Isomorphism|isomorphism]] $C_{mn}=C_m\times C_n$.

##### *Proof.*

***
#### Problem 
Find an example of groups $G,H$ such that there is an isomorphism $G\times H\cong G$ but $H$ is not trivial. Note: since $G\times H\cong G$ can be rewritten as $G\times H\cong G\times \{e\}$, the above shows that in general one cannot cancel groups in isomorphisms between direct products.

##### *Proof.*
***
#### Problem 
For each natural number $n$, let $V_n$ be the subset of the symmetric group $S_n$ defined by $$V_n = \{(i j)(k l) | i,j,k,l \in \{1,\ldots, n\}, i \neq j, \text{ and } k \neq l\},$$ that is, $V_n$ is the set of all products of two 2-cycles. Let $A_n$ be the subgroup of $S_n$ generated by $V_n$; the group $A_n$ is called the {\em alternating group of degree} $n$. For any $\sigma\in S_n$ define the set $$\sigma A_n\sigma^{-1}=\{\sigma \tau \sigma^{-1} \mid \tau\in A_n\}.$$ Prove that $\sigma A_n\sigma^{-1}=A_n$ for any $\sigma\in S_n$ (that is, $A_n$ is a normal subgroup of $S_n$).

### Homework 4

A [[Group|group]] is called {\em Hamiltonian} if every subgroup of the group is a [[Normal Subgroup|normal]] subgroup. Prove that $Q_8$, the [[Quaternions|quaternion]] group, is Hamiltonian.

#### Problem 
1. Prove that if $f:G\to H$ is a group homomorphism and $K\norm H$ then the preimage of $K$, $f^{-1}(K)=\{g\in G | f(g)\in K\}$, is a normal subgroup of $G$.
2. Show that if $f:G\to H$ is a group homomorphism and $L \norm G$ then $f(L)$ need not be a normal subgroup of $H$.

##### *Proof.*
***
#### Problem 
Show that any subgroup of index two is normal. This means: show that if $G$ is a group, $H$ is a subgroup and $[G:H]=2$, i.e the number of left (or right) cosets of $H$ in $G$ is two, then $H$ is normal.

##### *Proof.*
***
#### Problem 
For a group $G$ and elements $x,y \in G$, we define the {\em commutator} of $x, y$ to be $[x,y] = xyx^{-1}y^{-1}$. The {\em commutator subgroup} $G'$ is defined as the subgroup generated by $\{[x,y] \mid x,y \in G\}$.
1. Prove that $G'$ is normal.
2. For $N \norm G$, prove that $G/N$ is abelian if and only if $G' \subseteq N$.

##### *Proof.*
***
#### Problem 
Let $G$ be a group and let $A \subseteq G$ be a set. The {\em normal subgroup of $G$ generated by $A$}, denoted $\langle A \rangle ^N$, is the intersection of all the normal subgroups of $G$ that contain $A$.
1. Show that $\langle A \rangle ^N$ is a normal subgroup of $G$.
2. Show that the elements of $\langle A \rangle ^N$ can be described as $$\langle A \rangle ^N= \{ g_1a_1^{i_1}g_1^{-1} \dots g_ma_m^{i_m}g_m^{-1} \mid m \geq 0, a_j \in A, g_j \in G, i_j \in \{1,-1\}, \forall 1\leq j\leq m\}.$$

##### *Proof.*
***
### Homework 5
#### Problem 
Let $H$ be a [[Subgroup|subgroup]] of $G$ and fix some element $g\in G$.
(a) Prove that $gHg^{-1}=\{ghg^{-1} \mid h\in H\}$ is a subgroup of $G$ of the same [[Order|order]] as $H$.
(b) Deduce that if $H$ is the unique subgroup of $G$ of order $|H|$ then $H\norm G$ (See: [[Normal Subgroup|Normal]]).

##### *Proof.*
Let $H$ be a subgroup of $G$ and fix some element $g\in G$.

###### Part (a)
Let $gHg^{-1}=\{ghg^{-1} \mid h\in H\}$, and $h,k\in H$. Consider $$(ghg\inv)(gkg\inv)=gh(gg\inv)kg\inv=g(hk)g\inv,$$which is contained in $gHg\inv$ as $hk\in H$ by the definition of subgroup. Thus $gHg\inv$ is multiplicatively closed. 

Next, observe $$(ghg\inv)(gh\inv g\inv)=gh(g\inv g)h\inv g\inv=ghh\inv g\inv=e,$$
making $gh\inv g\inv$ the inverse of $ghg\inv$. As $h\inv\in H$ (by the definition of subgroup), we see $gh\inv g\inv\in gHg\inv$, making $gHg\inv$ a subgroup of $G$ by the subgroup test. 

Consider the function $f_g:H\to gHg\inv$ defined by $f_g(h)=ghg\inv$. Suppose that there exist $x,y\in H$ such that $f_g(x)=f_g(y)$. Then $gxg\inv=gyg\inv$, and by multiplying on the left and right by $g\inv$ and $g$, respectively, we see $x=y$, making $f_g$ injective.

Let $ghg\inv\in gHg\inv$ and consider $h\in H$. As $f_g(h)=ghg\inv$, we see that $f_g$ is surjective as well, making $f_g$ a bijective correspondence between $H$ and $gHg\inv$. Thus $gHg^{-1}=\{ghg^{-1} \mid h\in H\}$ is a subgroup of $G$ of the same order as $H$.
***
###### Part (b)
Suppose $H$ is the unique subgroup of $G$ of order $|H|$. Let $g\in G$. From part (a), $gHg\inv$ is a subgroup of order $H$. Since $H$ is unique, this means that $H=gHg\inv$ for all $g\in G,$ making $H$ normal in $G$. 
***
#### Problem – HK and KH
Let $G$ be a group with subgroups $H, K$. Recall the notation $$HK=\{hk \mid h\in H, k\in K\}.$$
(a) Prove that $HK\leq G$ if and only if $HK=KH$.
(b) Prove that if either one of $H$ or $K$ is a normal subgroup of $G$, then $HK\leq G$ and $HK=KH=\langle H\cup K\rangle$ (See: [[Generator]]).

##### *Proof.*
Let $G$ be a group with subgroups $H, K$.

###### Part (a)
First, suppose $HK\leq G$. 
Let $hk\in HK$. Notice that $(hk)\inv=k\inv h\inv$. As $H,K\leq G$ we have $h\inv\in H$ and $k\inv\in K$, making $k\inv h\inv\in KH$. However, as $HK\leq G$, we have $k\inv h\inv\in HK$ as well. This means that $k\inv h\inv =h'k'$ for some $h',k'\in HK$. By the same argument we see that $hk$ must be contained in $KH$ as well, as it is the inverse of $h'k'$. Thus $HK\subseteq KH$.

Let $kh\in KH$. We know $(kh)\inv=h\inv k\inv\in HK$. As $HK\leq G$ we know that  $h\inv k\inv)\inv=kh\in HK$ as well. Thus $KH\subseteq HK$ and $HK=KH$. 
Note: This only used the closure of inverses of $HK$.

Next, suppose $HK=KH$. Let $hk, h'k'\in HK$, and notice $(hk)(h'k')=h(kh')k'$. However, as $HK=KH$ we know $kh'=xy$ for some $x\in H, y\in K$. Thus we have $h(xy)k'=(hx)(yk')$, where $hx\in H$ and $yk'\in K$. Thus $HK$ is closed under multiplication. 

Let $hk\in HK$. Notice that $(hk)\inv=k\inv h\inv$. As $H,K\leq G$, we see that $k\inv\in K$ and $h\inv\in H$. Thus $k\inv h\inv\in KH=HK$, making $HK\leq G$ by the subgroup test. 
***
###### Part (b)
Suppose without loss of generality that $H\nsg G$. 
Let $hk\in HK$, and observe $$(hk)\inv=k\inv h\inv=k\inv h\inv (kk\inv)=(k\inv h\inv k)k\inv.$$As $k\inv\in G$, we have $k\inv H(k\inv)\inv=k\inv Hk=H$, and thus $k\inv h\inv k=h'$ for some $h\in H$. Substituting, we get $h'k\inv$, an element of $HK$. 

Using the same argument used in Part (a), we find $HK=KH$, making $HK\leq G$. 

As $\langle H\cup K\rangle$ is the intersection of all subgroups containing $H$ and $K$, we see $\langle H\cup K\rangle\subseteq HK$, as $H,K\subseteq HK$. Let $hk\in HK$. Let $N$ be any subgroup containing both $H$ and $K$. Then $h,k\in N$ and therefore $hk\in N$ as well. Thus $HK\subseteq\langle H\cup K\rangle$, completing the proof.
***
#### Problem 
Let $G$ be a group and let $N$ be a normal subgroup of $G$. Prove the following:

(a) If $G$ is abelian then $G/N$ is abelian.
(b) If $G$ is cyclic then $G/N$ is cyclic.
(c) If $G/Z(G)$ is cyclic then $G$ is abelian.

##### *Proof.*
Let $G$ be a group and let $N$ be a normal subgroup of $G$. 
###### Part (a)
Suppose $G$ is abelian. Let $xN, yN\in G/N$. As $G$ is abelian, we have $$xNyN=(xy)N=(yx)N=yNxN,$$making $G/N$ abelian as well.
***
###### Part (b)
Suppose $G$ is cyclic, so $G=\langle x\rangle$ for some $x\in G$. 
If $x\in N$ then $N=G$ and $G/N=\{e\}$, one of my favorite cyclic groups.
If $x\not\in N$ then let $gN\in G/N$. Notice that as $g=x^n$ for some $n\in \N$ we have $gN=x^nN$, meaning that every element in $G/N$ is generated by $xN$. Thus $G/N$ is cyclic.
***
###### Part (c)
Suppose $G/Z(G)$ is cyclic. Let $x\in G$ and suppose by way of contradiction that $x\not\in Z(G)$. Thus there exists some $y\in G$ such that $xy\neq yx$. Note: this means $y\not\in Z(G)$ either. As $G/Z(G)$ is cyclic there exists some $g\in G$ such that $xN=g^nN$ and $yN=g^mN$ for $n,m\in\N$. But then $$xNyN=g^nNg^mN=g^ng^mN=g^{n+m}N=g^{m+n}=g^mg^nN=g^mNg^nN=yNxN.$$As coset multiplication is defined as $xNyN=(xy)N$, this means that $xy=yx$, a contradiction. Thus $G$ is abelian.
***
#### Problem 
Prove that there are group isomorphisms between the following pairs of groups: 
(a) $\left(\Q/\Z, +\right)\cong \left(\mu,\cdot\right)$, where $\mu=\{z\in \C \mid z^n=1 \text{ for some integer } n\}$.
(b) $(\C^\times,\cdot)/\mu_m\cong (\C^\times,\cdot)$ for any integer $m\geq 1$, where $\mu_m=\{z\in \C \mid z^m=1\}$.

##### *Proof.*
***
#### Problem – Done
Let $G$ be a finite [[Group|group]], $H$ and $N$ [[Subgroup|subgroups]] such that $|H|$ (See: [[Order]]) and $[G : N]$ (See: [[Index]]) are relatively prime and $N\norm G$ (See: [[Normal Subgroup|Normal]]). Prove that $H \subseteq N$.

##### *Proof.*
Let $G$ be a finite group, $H$ and $N$ subgroups such that $|H|$ and $[G : N]$ are relatively prime and $N\norm G$. 

Let $h\in H$ and suppose $h\not\in N$. Let $[G:N]=n$. Then $hN\neq N$ in $G/N$. By [[Theorem – Lagrange's Theorem|Lagrange's Theorem]] we have $|h|\big||H|$. However, 

By Corollary, $[G:N]=\frac{|G|}{|N|}$, so $|hN|\big|n$. So $hN^n=h^nN=N$. But $hN^{|H|}=N$ as well, so one of the orders has to divide the other, which is a big no-no in the world relatively prime.
***
### Homework 6
#### Problem 
Let $H$ be a subgroup of a group $G$. Then $G$ acts on the set $G/H$ of left cosets by left multiplication $g \cdot (g'H) = (gg')H$. You need not check that this is an action.
Let $\rho: G\to \Perm(G/H)$ denote the permutation representation associated to this action. Prove

(a) the action described above is transitive
(b) $\ker(\rho) = \bigcap_{g \in G} gHg^{-1}$
(c) the subgroup described in (a) is the largest (with respect to containment) normal subgroup of $G$ contained in $H$.

##### *Proof.*
###### Part (a)

***
###### Part (b)
***
###### Part (c)
***
#### Problem 
Let $G$ be a group, and let $H$ be a subgroup of $G$ of finite index $|G:H| = n$. Show that there exists a normal subgroup $N\norm G$ such that $N \leq H$ and $|G:N| \leq n!$. {\em Hint: use problem 1.}

##### *Proof.*

***
#### Problem 
Prove that if $G$ is a finite group of order $n$ and $p$ is the smallest prime dividing $|G|$, then any subgroup $H$ of $G$ of index $p$ is normal in $G$. {\em Hint: use problem 1.}

##### *Proof.*
***
#### Problem 
Let $G$ be the group of orientation preserving isometries of the dodecahedron.
1. Prove that $|G| = 60$.
2. Prove that $G$ is isomorphic to a subgroup of $S_5$. You may use without proof that there are $5$ inscribed cubes in a dodecahedron (see Figure 1 below).
3. Prove that $G$ is in fact isomorphic to $A_5$. You may assume known that $A_5$ has no normal subgroups other than $A_5$ and the trivial subgroup, a fact that we will eventually prove in class.
(need figure)

##### *Proof.*
***
#### Problem – Done
Prove that if $G$ is non-abelian and $|G| = 21$, then there is only one possible class equation for $G$, meaning that the numbers appearing in the class equation are uniquely determined up to permutation.

##### *Proof.*
Let $G$ be a non-abelian group of order $21$. Recall the class equation:
$$|G|=|Z(G)|+\sum_{g\in G}[G:C_G(g)],$$
where $C_G(g)$ denotes the conjugacy classes of elements of $G$ that are non-trivial. Since $G$ is not abelian, we know $|Z(G)|\neq 21$ and there exists some $x\not\in Z(G)$. In fact, if $Z(G)$ is not trivial then it has order $3$ or $7$, and thus $G/Z(G)$ would be cyclic, making $G$ abelian. 
We examine $C_G(x)$. From this Corollary we have $[G:C_G(x)]=\frac{|G|}{|C_G(x)|}=\frac{21}{C_G(x)}$, and so the possibilities for $|C_G(x)|$ are $1,3,7,$ and $21$. As $x\not\in Z(G)$ we know $|C_G(x)|\neq21$. If the order was one then it would be in the center, so all we need consider are orders $3$ and $7$. 
Luckily, there is only one way to sum to $20$ using $3$s and $7$s ($3+3+7+7$), and thus our class equation is unique. 
***
### Homework 7
#### Problem – Converse of Lagrange's Theorem False
Prove the converse to Lagrange's theorem is false: find a group $G$ and an integer $d>0$ such that $d$ divides the order of $G$ but $G$ does not have any subgroups of order $d$. *Hint*: Take $G=A_5$.

##### *Proof.*
Consider $G=A_4$, and note that $|G|=12$. 
Suppose by way of contradiction that $H$ is subgroup of $G$ such that $|H|=6$. 
Notice that $[G:H]=2$, the smallest prime dividing the order of $G$, making $H$ normal in $G$. 

As there are eight $3$-cycles in $G$, there exists some $3$-cycle, $\sigma$, such that $\s\not\in H$. Consider then $H, \s H,$ and $\s^2 H$ in $G/H$. Since $|G/H|=\frac{|G|}{|H|}=2$, it must be the case that either $\s^2H=\s H$ or $\s^2H=H$. 

- If $\s^2 H=H$ then $\s^2\in H$. As $|\s|=3$ we have $\s^2=\s\inv$, but as $H$ is a subgroup this would mean $(\s\inv)\inv=\s\in H$, which is not the case.
- If $\s^2 H=\s H$ then $\s\inv\s^2\in H$, but $\s\inv\s^2=\s$, and so we have a contradiction.
Thus $H$ cannot exist, and $G$ has no subgroup of order $6$. 
***
#### Problem – Ask Justin
Let $G$ be a finite group of order $pqr$ with $0<p < q < r$ prime numbers. Show that $G$ is not simple.

##### *Proof.*
Let $G$ be a finite group of order $pqr$ with $0<p < q < r$ prime numbers.
Suppose by way of contradiction that $G$ is simple. From Part (1) of Sylow's Theorem we have the following:
- $n_p|qr$ and $n_p\equiv 1\mod{p}$
- $n_q|pr$ and $n_q\equiv 1\mod{q}$
- $n_r|pq$ and $n_r\equiv 1\mod{r}$
As $G$ is simple, $n_r$ must be $pq$, as $p,q<r$. Each Sylow$-r$ subgroup has $r-1$ unique elements, so if $n_r=pq$ that would yield $(r-1)pq=pqr-pq$ elements of order $r$. 
As $G$ is still simple, $n_q$ must be either $pr$ or $r$. 
- Each Sylow$-q$ subgroup has $q-1$ unique elements, so if $n_q=pr$ that would yield $(q-1)pr=pqr-pr$ elements of order $q$. As $pqr-pq+pqr-pr=2pqr-p(q+r)$...idk if this is the right direction
***
#### Problem 
Let $G$ be a group of order $2^5\cdot 7^3$. Prove that $G$ is not simple.

##### *Proof.*
Let $G$ be a group of order $2^5\cdot 7^3$. 
Suppose by way of contradiction that $G$ is simple. From Part (1) of Sylow's Theorem we have $n_7|32$ and $n_7\equiv 1\mod{7}$, for which the options are $1$ and $8$. As $G$ is simple, $n_7=8$. Let $G$ act on $\Syl_7(G)$ by conjugation, yielding the permutation representation homomorphism $\rho:G\to S_8$. However, $|G|\not\big||S_8|$, so $\rho$ cannot be injective, making the $\ker(\rho)$ a non-trivial normal subgroup of $G$, a contradiction. Thus $G$ cannot be simple.
***
#### Problem 
Prove Cauchy's Theorem: If $G$ is a finite group and $p$ is a prime that divides $|G|$, then $G$ has an element of order $p$. Do this by completing the following steps. Let $S$ denote the set of ordered $p$-tuples of elements of $G$ whose product is $e$: $$ S = \{(x_1, \dots, x_p) \mid x_i \in G, x_1 x_2 \cdots x_p = e\}. $$
1. Show that $|S| = |G|^{p-1}$.
2. Let $C_p$ denote cyclic subgroup of $S_p$ of order $p$ generated by the $p$-cycle \\ $\sigma = (1 \, 2 \, \cdots \, p)$. The following rule gives an action of $C_p$ on $S$ (you need not check) $$ \sigma^i \cdot (x_1, \dots, x_p) := (x_{\sigma(1)}, \dots, x_{\sigma(p)}) = (x_{1+i}, x_{2+i}, \dots, x_{p+i}), $$ where the indices are taken modulo $p$. Show that an orbit of size one for this action is given by an element $(x, x, \dots, x)$ of $S$ with $x \in G$ satisfying $x^p = e$, and that there must be at least one orbit of size one besides the one given by $(e, e, \dots, e)$.

##### *Proof.*
***
#### Problem 
(**Optional -- Extra credit for complete solution**) Let $G$ be a finite group with $N \norm G$, let $p$ be a prime number and let $Q$ be a Sylow $p$-subgroup of G.
(a) Show that $Q \cap N \in \Syl_p(N)$.
(b) Show that $QN/N \in \Syl_p(G/N)$.
(c) Show that $|\Syl_p(G/N)| \leq |\Syl_p(G)|$.

##### *Proof.*
Let $G$ be a finite group with $N \norm G$, let $p$ be a prime number and let $Q$ be a Sylow $p$-subgroup of G.

###### Part (a)
Let $P\in\Syl_p(N)$. 
As $N\nsg G$, by the Second Isomorphism Theorem we have $Q\cap N\nsg Q$, and so $Q\cap N$is a $p$-group and $\frac{Q}{N\cap Q}\cong \frac{QN}{N}$. Thus $|\frac{Q}{Q\cap N}|=|\frac{QN}{N}|$ and $\frac{|Q|}{|Q\cap N|}=\frac{|QN|}{|N|}$. 
Note that $$[N:Q\cap N]=\frac{|N|}{|Q\cap N|}=\frac{|QN|}{|Q|}=[QN:Q]$$

Also, $[G:Q]=[G:QN]\cdot[QN:Q]$. 
As $Q$ is a Sylow $p$-subgroup of $G$ we know $\gcd(p,|[G:Q|])=1$, and thus that $p$ cannot divide $[QN:Q]$. As $[QN:Q]=[N:Q\cap N]$, we see that $Q\cap N$ is a $p$-subgroup of $N$ with $\gcd(p,[N:Q\cap N])=1$, we see that $Q\cap N$ is a Sylow $p$-subgroup of $N$.
***
###### Part (b)
As $N\nsg G$, by the Second Isomorphism Theorem we have $\frac{QN}{N}\cong\frac{Q}{Q\cap N}$

$[G/N:Q/N]=[G/N:QN/N]\cdot[QN/N:Q/N]$

***
###### Part (c)
***
### Homework 8
#### Problem – Prime Squared is Abelian
If $p$ is a prime integer and $G$ is a group of order $p^2$, prove that $G$ is abelian and in fact either $G\cong C_{p^2}$ or $G\cong C_{p}\times C_p$ (where $C_n$ denotes the cyclic group of order $n$). *Tip*: consider $Z(G)$.

##### *Proof.*
Let $G$ be a group of order $p^2$ for some prime $p$. In $p$-groups the center is non-trivial (See:) and thus $Z(G)$ has order $p$ or order $p^2$. 
- If $|Z(G)|=p$ then $G/Z(G)$ has order $p$, making it cyclic. This makes $G$ abelian. (See: ) 
- If $|Z(G)|=p^2$ then $Z(G)=G$, making $G$ abelian. 
By the FTFGAB there are two abelian groups of order $p^2: \Z_{p^2}$ and $\Z_p\times Z_p$. As $\Z_{p^2}\cong C_{p^2}$ and $\Z_p\times Z_p\cong C_p\times C_p$$, $G$ must be isomorphic to one of these groups.
***
#### Problem – Semidirect Product and GCD
Let $N$ be a normal subgroup of a finite group $G$, and assume that $|N|$ and $|G/N|$ are relatively prime (i.e., their greatest common divisor is 1). Assume there is a subgroup $H$ in $G$ such that $|H| = |G/N|$. Prove that $G$ is a semidirect product of $N$ and $H$.

##### *Proof.*
Let $N$ be a normal subgroup of a finite group $G$, and assume that $|N|$ and $|G/N|$ are relatively prime. Assume there is a subgroup $H$ in $G$ such that $|H| = |G/N|$.

As $|H|=|G/N|$ we see that $|H|$ and $|N|$ are relatively prime, making their intersection trivial. As $H$ is normal in $G$ we have $HN\leq G$ and $$|HN|=\frac{|H||N|}{H\cap N}=|H||N|=|G/N||N|=|G|,$$and so $HN=G$. Thus $G$ is a semidirect product of $N$ and $H$ by the recognition theorem.
***
#### Problem 
Prove that the [[Quaternions|quaternion]] group $Q_8$ is not isomorphic to a semi-direct product $H\sdp_\rho K$ for non-trivial groups $H$ and $K$.

##### *Proof.*
***
#### Problem 
Let $H = \langle x \mid x^m = e_H \rangle$ and $K = \langle y \mid y^n = e_K \rangle$ be cyclic groups of orders $m$ and $n$, respectively. Let $j>0$ be an integer satisfying $\gcd(j,m) = 1$ and $j^n \equiv 1 \pmod{m}$.
1. Show that there is a unique homomorphism $\phi: K \to \Aut(H)$ so that $\phi(y)(x) = x^j.$
2. If $\phi$ is the homomorphism from part (a), show that $$H \sdp_\phi K \cong \langle r,s \mid r^m = e, s^n = e, srs^{-1} = r^j \rangle.$$

##### *Proof.*
***
#### Problem 
Let $K$ be a finite cyclic group and let $H$ be an arbitrary group. Suppose that the images of $\phi: K \to \Aut(H)$ and $\theta: K \to \Aut(H)$ are conjugate subgroups of $\Aut(H)$, that is, there is $\sigma \in \Aut(H)$ such that $\sigma \phi(K) \sigma^{-1} = \theta(K)$. Show that $H \sdp_\phi K \cong H \sdp_\theta K$.
{\em Tip:} Show that there is an integer $m$ such that $\sigma \phi(x)\sigma^{-1} = \theta(x)^m$ for all $x \in K$, and that the map $\Psi: H \sdp_\phi K \to H \sdp_\theta K$ defined by $\Psi(n,x) = (\sigma(n),x^m)$ is an isomorphism.

##### *Proof.*
***
### Homework 9
#### Problem – Cyclic Automorphisms and Group of Units
Prove that the automorphism group of the cyclic group $C_n$ of order $n$ is isomorphic to the group of units of $\Z/n$ with multiplication as the binary operation, that is,
$$(\Z/n)^\times =\{[j]_n\mid \gcd(j,n)=1\}.$$

##### *Proof.*
Let $\phi\in\Aut(C_n)$, and let $x$ be a generator of $C_n$. $\phi(x)=x^i$ for some $i$. For $\phi$ to be an automorphism it must map $x$ to another generator of $G$. The generators of $C_n$ are precisely the elements of $(\Z/n)^\times$.
***
#### Problem – Groups of Order 105
Prove that there are precisely two groups of order $105$ up to isomorphism.
Here are some steps you will likely want to use:
1. If $|G| = 105$, then there is either a unique Sylow $5$-subgroup or a unique Sylow $7$-subgroup of $G$.
2. If $|G| = 105$, then $G$ has a cyclic subgroup of order $35$.
3. If $|G| = 105$ then $G \cong C_{35} \rtimes_\rho C_3$ for some $\rho:C_3 \to \Aut(C_{35})$.

##### *Proof.*
Let $G$ be a group of order 105. Then $G\cong C_{105}$ or it isn't. 
Suppose it's not. 
By Sylow's Theorem we know the following:
- $n_5|21$ and $n_5\equiv 1\mod{5}$, so $n_5=1$ or $21$.
- $n_7|15$ and $n_7\equiv 1\mod{7}$, so $n_7=1$ or $8$. 
If $n_5=21$ then there are $(5-1)21=84$ elements of order $5$ and if $n_7=8$ then there are $(7-1)\cdot 8=48$ elements of order $7$. As $84+58>105$ we see there will either be a unique Sylow $5$-subgroup or Sylow $7$-subgroup. 

Without loss of generality, suppose $n_5=1$, making $P$, the unique Sylow $5$-subgroup, normal in $G$. As $7$ is a prime dividing the order of $G$ there exists an element of order $7, x$ by Cauchy's Theorem. Let $Q=\langle x\rangle$. As $P$ has order $5$ it is cyclic. Since $P\nsg G$ we have $PQ\leq G$, and since $Q$ and $P$ are cyclic groups of relatively prime order, we see that $PQ\cong C_{35}$. Thus $G$ has a cyclic subgroup of order $35$. 

Let $PQ=H$ for simplicity. 
Notice that $[G:H]=3$, the smallest prime dividing the order of $G$, making $H$ normal in $G$. Let $k$ be an element of order $3$ in $G$ and let $K=\langle k\rangle$. As $H\nsg G$, we have $HK\leq G$, and as $H$ and $K$ are cyclic groups of relatively prime order, we see $HK=G$. Thus $G \cong C_{35} \rtimes_\rho C_3$ for some $\rho:C_3 \to \Aut(C_{35})$ by the recognition theorem.
***
#### Problem – Not Done
Classify all of the groups of order $28$ into isomorphism classes. (There will be $4$ classes.)

##### *Proof.*
Let $G$ be a group of order $28=2^2\cdot 7$. 
Suppose $G$ is abelian. Then by the FTFGAG and Sun Tzu's Theorem there are two possibilities for $G$:
1. $\Z_{28}$, 
2. $\Z_2\times Z_2\times \Z_7$
Suppose then that $G$ is not abelian. 
By Sylow's Theorem we know the following:
- $n_2|7$ and $n_5\equiv 1\mod{2}$, so $n_2=1$ or $7$.
- $n_7|4$ and $n_7\equiv 1\mod{7}$, so $n_7=1$. 
Lucky us! There is exactly one Sylow $7$-subgroup of $G$, which we denote $H$. As it is unique, $H\nsg G$.
Notice that any Sylow $2$-group of $G$ will have $2^2=4$ elements, and there are only two groups of order four: $\Z/4$ and $\Z/2\times\Z/2$. Let $K\in\Syl_2(G)$.

Suppose $K\cong\Z/4$. Then $K$ and $H$ are cyclic groups of relatively prime order, and since $H\nsg G$, we have $HK=G$, making $G \cong C_7 \rtimes_\rho C_4$ for some $\rho:C_4 \to \Aut(C_7)$ by the recognition theorem.

Suppose then that $K\cong \Z/2\times\Z/2$. We know $\Aut(H)\cong(\Z/7)^\times\cong\Z/6$. 


***
#### Problem 
Let $A,B,C$ be finitely generated abelian groups. Prove that the following cancellation property holds: if $A\times B\cong A\times C$, then $B\cong C$.

##### *Proof.*

***
#### Problem 
1. Let $G$ be a finite abelian group and let $e$ denote the smallest positive integer which satisfies $g^e=e_G$ for all $g\in G$. This number is called the {\em exponent} of $G$. Give, with justification, formulas for $e$ in terms of the elementary divisors of $G$ and, separately, in terms of the invariant factors of $G$.
2. Prove that if $p$ is prime then the abelian group $((\Z/p)^\times, \cdot)$ is cyclic. You may use the fact (which we will eventually prove) that for any integer $e>0$ the equation $[x]_p^e=[1]_p$ has at most $e$ solutions in $\Z/p$.

##### *Proof.*
***
### Homework 10
#### Problem 
Prove that any finite domain (i.e. an integral domain that has finitely many elements) is a field.

##### *Proof.*
Let $R$ be a finite integral domain, $x\in R$, and consider $S=\{x^i|i\in\N\}$. As $R$ is finite, there will come a time when $x^m=x^n$ for some $m<n\in\N$. Dividing on both sides by $x^m$ we find $1=x^{n-m}$. Thus $x\cdot x^{n-m-1}=1$, making $x$ a unit. As $x$ was arbitrary, every element of $R$ is a unit. Thus $R$ is a field.
***
#### Problem 
The center of a ring $R$ is the set $Z(R)=\{z \in R \mid zr = rz \text{ for all } r \in R\}$.
(a) Prove that the center of a ring with $1$ is a subring that contains the same $1$.
(b) Determine the center of the real quaternion ring $\mathbb{H}$.

##### *Proof.*
###### Part (a)
Let $x,y\in Z(R)$. Let $r\in R$. Notice $$(xy)r=x(yr)=x(ry)=(xr)y=rxy.$$As addition is always commutative in rings we see that the underlying subgroup is indeed a subgroup.
As $1$ commutes with everything it is in the center and remains the multiplicative identity. 
Thus $Z(R)$ is indeed a subring. 
***
###### Part (b)
***
#### Problem – Norm Function and Units of Gaussian Integers
Let $\Z[i] = \{a + bi \mid a,b \in \Z\}$ be the ring of Gaussian integers. Define a function $$N:\Z[i]\to\Z, N(a+bi)=a^2+b^2.$$
(a) Prove that $N(\a\b)=N(\a)N(\b)$ for any $\a,\b\in \Z[i]$.
(b) Use the function $N$ to determine the units of $\Z[i]$.

##### *Proof.*
###### Part (a)
Let $\alpha,\beta\in\Z[i]$ and behold $\begin{align}N(\alpha\beta)&=N((a+bi)(c+di))\\&=N(ac-bd+adi+bci)\\&=(ac-bd)^2+(ad+bc)^2\\&=((ac)^2-2acbd+(bd)^2)+((ad)^2+2abcd+(bc^2))\\&=a^2c^2+b^2d^2+a^2d^2+b^2c^2\\&=(a^2c^2+a^2d^2)+(b^2c^2+b^2d^2)\\&=a^2(c^2+d^2)+b^2(c^2+d^2)\\N(\alpha)N(\beta)&=(a^2+b^2)(c^2+d^2).\end{align}$
So there's that done.
***
###### Part (b)
Suppose $\alpha\beta=1$. Then by Part (a) we know $$N(\alpha)N(\beta)=N(\alpha\beta)=N(1)=1,$$ so $(a^2+b^2)(c^2+d^2)=1$, with $a,b,c,d\in\Z$. Thus we have $a^2+b^2=1=c^2+d^2$. So the units of $\Z[i]$ are $\{\pm 1,\pm i\}$.
***
#### Problem 
Let $S=\{a+bi+cj+dk \mid a,b,c,d \in \Z\}$ be the ring of integral Hamiltonian quaternions, where multiplication is defined using the same rules as in $\mathbb{H}$. Define a function $$N:S\to\Z, N(a+bi+cj+dk)=a^2+b^2+c^2+d^2.$$
1. For any $\a=a+bi+cj+dk\in S$, denote $\bar\a=a-bi-cj-dk$. Show that $\overline{\a\b}=\bar \b \bar\a$ for all $\a,\b\in \mathbb{H}$.
2. Prove that $N(\a)=\a\bar\a$ and $N(\a\b)=N(\a)N(\b)$ for any $\a,\b\in S$.
3. Prove that $\a\in S^\times$ if and only if $N(\a)=1$.
4. Show that there is a group isomorphism $(S^\times,\cdot)\cong Q_8$.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring with 1, and let $p(x) = a_0 + a_1x + \dots + a_nx^n$ be a nonzero element of $R[x]$.

(a) Prove that $p(x)$ is a zero divisor in $R[x]$ if and only if there is a nonzero $b \in R$ with $bp(x) = 0$.
(b) Conclude that, if $R$ is a domain, then $R[x]$ is a domain.

##### *Proof.*
Let $R$ be a commutative ring with 1, and let $p(x) = a_0 + a_1x + \dots + a_nx^n$ be a nonzero element of $R[x]$.

###### Part (a)
First suppose that $p(x)$ is a zero divisor in $R[x]$. Thus there exists some $q(x)\in R[x]$ such that $p(x)q(x)=0$. If $q(x)$ contains a nonzero term with an $x$ in it, then we cannot get to $0$, as $x$ has no multiplicative inverse in $R[x]$. In fact, the constant term of $q$ must knock every term in $p$ to $0$, and thus the constant term of $q$, we'll call it $b$, must annihilate $p$. 

Suppose there exists some nonzero $b\in R$ such that $bp(x)=0$. Well $b\in R[x]$, so $p(x)$ is a zero divisor.
***
###### Part (b)
If $R$ is a domain then there exist no zero divisors, so there can exist no polynomial zero divisors by Part (a), so $R[x]$ is a domain. 
***
### Homework 11
#### Problem 
(a) Let $a\neq 0, b\neq 0$ be integers and let $(a),(b)$ be the ideals they generate in $\Z$. Show that $(a)+(b)=(\gcd(a,b))$ and $(a)\cap (b)=(\rm{lcm}(a,b))$.
(b) Prove that the ideal $(2,x)$ of $\Z[x]$ is not principal, that is, it cannot be generated by a single element.

##### *Proof.*
###### Part (a)
***
###### Part (b)
***
#### Problem 
In each part, prove whether or not the ring $R$ is isomorphic to the ring $S$.
1. $R = \Z$ and $S = \Z[x]$.
2. $R = \Z/3$ and $S=\{t \in \Z/6 \mid 3t = 0\}$ \\(The set $S$ is a subring of $\Z/6$ -- a fact that you need not prove.)
3. $R = \Z/3 \times \Z/3$ and $S = (\Z/3)[x]/(x^2+[1]_3)$.
4. $R = \R[G]$, where $G = \Z/2 \times \Z/2$, and $S = \M_{4\times 4}(\R)$.

##### *Proof.*
***
#### Problem 
Let $R$ be a ring with $1\neq 0$.
(a) Prove that an ideal $I$ of $R$ is proper if and only if $I$ contains no unit.
(b) If $R$ is commutative, show that $R$ is a field if and only if the only ideals of $R$ are $(0)$ and $R$.

##### *Proof.*
Let $R$ be a ring with $1\neq 0$.
###### Part (a)
Suppose $I$ is a proper ideal. Suppose by way of contradiction that $I$ contains a unit, $u$. Then there exists some $v\in R$ such that $uv=1$. By absorption then $I$ contains $1$, and by absorption again we can multiply $1$ by all of $R$ to see $I=R$, contradicting the fact that $I$ was proper. 

Suppose $I$ contains no units. Then $I\neq R$, making it proper. 
***
###### Part (b)
Suppose $R$ is a field, and let $I$ be an ideal of $R$. As every element of $R$ is a unit, if $I$ has anything but $0$ then it is all of $R$. Thus the only ideals of $R$ are $(0)$ and $R$ itself.

Suppose the only ideals of $R$ are $(0)$ and $(R)$. Let $x\in R$. Then $(x)=R$ or $(x)=0$. If $(x)=0$ then $x=0$, which is boring. If $(x)=R$ then $xy=1$ for some $y\in R$, making $x$ a unit. Thus $R$ is a field.  
***
#### Problem – May 2022 (4)
Let $I$ and $J$ be ideals of a commutative ring $R$ with $1 \neq 0$. Show that if $I + J = R$, then we have
1. $IJ = I \cap J$
2. a ring isomorphism $R/(I\cap J) \cong R/I\times R/J$.
The latter isomorphism is called the Chinese Remainder Theorem.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring with $1 \neq 0$ and let $I$ be an ideal of $R$.
(a) The radical of $I$ is the set $$\sqrt I = \{r \in R \mid r^n \in I \text{ for some } n \geq 1\}.$$ Show that $\sqrt I$ is an ideal of $R$.
(b) The ideal $I$ is called a radical ideal if $\sqrt I = I$. Show that every prime ideal of $R$ is a radical ideal.
(c) Prove that the converse of part (b) is false.
*Tip*: In a commutative ring the Binomial Theorem holds: for any $r,s\in R, n\in\Z, n\geq 0$ $$(r+s)^n=\sum_{k=0}^n\binom{n}{k}r^ks^{n-k}.$$ You may use this fact without proof.

##### *Proof.*
***
### Homework 12
#### Problem 
Let $R$ be a commutative ring with $1 \neq 0$. Prove that the set of prime ideals of $R$ has a minimal element with respect to inclusion. *Remark*: Note that in general this minimal element will not be $(0)$ unless $R$ is a domain.

##### *Proof.*
Let $S$ be the set of all prime ideals
***
#### Problem 
Let $C_3 = \langle a | a^3 = e \rangle$ and let $R=(\Z/2)[C_3]$ be the group ring of $C_3$ with $\Z/2$ coefficients and let $S = (\Z/2)[y]/(y^3-[1]_2)$. Prove that $S$ and $R$ are isomorphic rings.

##### *Proof.*
***
#### Problem 
Denote $\sqrt{-2}=\sqrt{2}\cdot {i}\in \C$. Prove that $\Z[\sqrt{-2}]=\{a+b\sqrt{-2}\mid a,b\in\Z\}$ is a Euclidean domain with respect to the norm function given by $$N:\Z[\sqrt{-2}]\to\Z, N(a+b\sqrt{-2})=a^2+2b^2.$$

##### *Proof.*

***
#### Problem 
Let $R = \Z[\sqrt{-5}]$ where $\sqrt{-5}=\sqrt{5}\cdot {i}\in \C$ and $\Z[\sqrt{-5}]=\{a+b\sqrt{-5}\mid a,b\in\Z\}$.
(a) Prove that $R\cong \Z[x]/(x^2+5)$ and, for integers $p\geq 2$, $R/(p)\cong (\Z/p)[x]/(x^2+[5]_p)$.
(b) Let $p$ be a prime integer. Show that $p$ is a prime element in $R$ if and only if the polynomial $x^2+[5]_p \in (\Z/p)[x]$ does not have a root in $\Z/p$.
(c) For each of the integers 7 and 13, determine whether the number is prime in $R$.
*Tip*: A useful fact: long division applies in a polynomial ring with arbitrary coefficients as long as the leading coefficient of the divisor is a unit.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring with $1 \neq 0$. Recall that the ring $R$ is called noetherian if it satisfies the following ascending chain condition: for any ascending chain of ideals $I_1 \subseteq I_2 \subseteq I_3 \subseteq \dots$ there exists a positive integer $n$ such that $I_n=I_{n+k}$ for all positive integers $k$ (that is, the ascending chain stabilizes). Prove that a ring $R$ is noetherian if and only if every ideal of $R$ is finitely generated.

##### *Proof.*
Let $R$ be a commutative ring with $1 \neq 0$. 
First, suppose that $R$ is noetherian. Let $I$ be an ideal of $R$. 
***
### Midterm Review
#### Problem 
Let $G$ be a finite group and $m$ a positive integer which is relatively prime to $|G|$. If $b \in G$ and $a^mb=ba^m$ for all $a\in G$, show that $b$ is in the center of $G$.

##### *Proof.*
Let $G$ be a finite group, $m$ a positive integer which is relatively prime to $|G|$, $b \in G$, and $a^mb=ba^m$ for all $a\in G$.

Let $G$ act on itself by conjugation, and consider $C_G(b)$, the centralizer of $b$ in $G$. Under the conjugation action we have $C_G(b)=\Stab_G(b)$. Since $a^mb=ba^m$, we also have $a^mb(a^m)\inv=b$, placing $a^m\in C_G(b)$. 

Suppose $ab\neq ba$. 


***
#### Problem – January 2019 (1) 
Let $G$ be a [[Group|group]]. A [[Subgroup|subgroup]] $H$ of $G$ is called a *characteristic* subgroup of G if $\alpha(H) = H$ for every automorphism $\alpha$ of $G$. Show that if $H$ is a characteristic subgroup of $N$ and $N$ is a [[Normal Subgroup|normal]] subgroup of $G$, then $H$ is a normal subgroup of $G$.
*Tip*: Consider in particular for each $g\in G$ the automorphism $a_g:G\to G$ given by $a_g(g')=gg'g^{-1}$.

##### *Proof.*
Let $G$ be a group, $N$ is a normal subgroup of $G$, and $H$ a characteristic subgroup of $N$. 
Let $g\in G$ and consider the automorphism $a_g:G\to G$ given by $a_g(g')=gg'g^{-1}$. 

Let $n\in N$ and notice $a_g(n)=gng\inv\in N$, as $N\nsg G$. 
Thus $a_g:N\to N$ is well defined. Let $n\in N$. As $gNg\inv=N$, we can write $n=gn'g\inv$ for some $n'\in N$. Then $a_g(n')=gn'g\inv=n$, making $a_g$ surjective. As $|N|=|N|$ we see that $a_g$ is a bijection. The homomorphism piece we get for free from $G$, making $a_g\in\Aut(N)$. 

Let $h\in H$. As $H$ is a characteristic subgroup of $N$, we see that $a_g(h)=ghg\inv=h$ for all $h\in H$ and for all $g\in G$. Thus $H$ is normal in $G$. 
***
#### Problem – Jan 2014 (2)
Let $G$ be a finite group and let $H$ be a proper subgroup of $G$ with $[G:H]=h$.
(a) Prove that $H$ has at most $h$ distinct conjugate sets $gHg^{-1}$ for $g\in G$.
(b) Prove that $G\neq \bigcup_{g\in G} gHg^{-1}$.

##### *Proof.*
Let $G$ be a finite group and let $H$ be a proper subgroup of $G$ with $[G:H]=h$.

###### Part (a)
Since $[G:H]=h$ we know $\frac{|G|}{|H|}=h$. Let $G$ act on $H$ by conjugation. Thus the conjugacy classes are now the orbits. 
***
###### Part (b)
***
#### Problem 
Let $H$ be a subgroup of a group $G$.
1. Show that the centralizer $C_G(H)$ of $H$ in $G$ is a normal subgroup of the normalizer $N_G(H)$ of $H$ in $G$.
2. Show that the quotient $N_G(H)/C_G(H)$ is isomorphic to a subgroup of the automorphism group ${\rm Aut}(H)$ of $H$.

##### *Proof.*
***
#### Problem 
Let $G$ be a finite group such that $|G|=nm$.
1. Suppose $x \in G$ has order $n$ and let $\sigma_x \in \rm{Perm}(G)$ be the permutation such that $\sigma_x(g) = xg$ for every $g \in G$. Show that $\sigma_x$ is a product of $m$ disjoint $n$-cycles.
2. If $n = 2$ and $m$ is odd, show that there is a homomorphism $f : G \to S_{nm}$ such that $f(G)\not\subseteq A_{nm}$.
3. If $n = 2$ and $m$ is odd, conclude that $G$ has a subgroup of index 2.

##### *Proof.*
***
#### Problem – January 2019 (2)
Let $G$ be a group acting on a set $A$, and let $H$ be a subgroup of $G$ satisfying that the induced action of $H$ on $A$ is transitive (that is, for all $a,b \in A$ there is an $h \in H$ with $h \cdot a = b$). Let $t \in A$, and let ${\rm Stab}_G(t)$ be the stabilizer of $t$ in $G$. Show that $G = H {\rm Stab}_G(t)$.

##### *Proof.*
***
#### Problem – January 2019 (3)
(a) Let $G$ be a simple group of order 60. Determine the number of elements of $G$ of order 5.
(b) Show that there is no simple group of order 30.

##### *Proof.*
###### Part (a)
Let $G$ be a simple group of order $60=2^2\cdot3\cdot 5.$ 
By Sylow's Theorem we know that $n_5|12$ and that $n_5\equiv 1\mod{5}$. Thus the options for $n_5$ are $1$ and $6$. Since $G$ is simple we see that $n_5=6$. As each Sylow $5$-subgroup of $G$ has $4$ unique elements of order $5$ and the identity we see that the number of elements or order $5$ in $G$ is $(5-1)\cdot 6=24$. 
***
###### Part (b)
Suppose by way of contradiction that $G$ is a simple group of order $30$. Similarly to above, $n_5=6$, yielding $24$ elements of order $5$. Now, $n_3|10$ and $n_3\equiv 1\mod{3}$, so $n_3=10$, yielding far too many elements to fit in $G$. 
***
#### Problem 
(a) Let $G$ be a group of order 15 acting on a set $S$ with 7 elements. Prove that there exists at least one fixed point, i.e., there exists $s\in S$ such that $g\cdot s=s$ for all $g\in G$.
(b) Give an example of an action of $C_{15}$ on a set with 8 elements with no fixed points. Justify.

##### *Proof.*
###### Part (a)
Let $G$ be a group of order 15 acting on a set $S$ with 7 elements. 

Recall that the orbits of an action are pairwise disjoint and partition $S$. 
By Orbit-Stabilizer we have $|G|=15=|\Orb(s)|\cdot|\Stab(s)|$. 
So $\sum_{s\in S}|\Orb(s)|=7$ and $|\Orb(s)|=1,3,$ or $5$. We will need $1$ to get to $7$, so there needs to be a singleton orbit for some $s\in S$.. Luckily, this means that $\Stab(s)=15$ by Orbit-Stabilizer, making $s$ a fixed point after all.
***
###### Part (b) 

***
#### Problem 
Let $A$ be a set, let $F(A)$ be the free group on $A$ and let $R$ be a subset of $F(A)$. Let $H$ be a group, and let $f:A \to H$ be a function satisfying the property that for any $m \geq 0$ and any choices of $r_j \in R, g_j \in F(A), i_j \in \{1,-1\}$ for $1\leq j\leq m$ we have that $f(g_1)f(r_1)^{i_1}f(g_1)^{-1} \cdots f(g_m)f(r_m)^{i_m}f(g_m)^{-1} =e_H$.
Prove that there is a unique homomorphism $F: \langle A \mid R \rangle \to H$ satisfying $F(a\langle R\rangle ^N) = f(a)$ for all $a \in A$.

##### *Proof.*
***
### Final Review
#### Problem – May 2022 (2)
A non-abelian group of order $27$.
1. Prove there exists a non-abelian group of $27$. (*Hint*: Use a semi-direct product.)
2. Find, with justification, a presentation of the group you found in part (a).

##### *Proof.*
***
#### Problem – Done
Determine, with justification, all the isomorphism classes of groups of order $45$.

##### *Proof.*
Let $G$ be a group of order $45=3^2\cdot 5$. 
By Sylow's Theorem we see $n_5|9$ and $n_5\equiv 1\mod{5}$, so $n_5=1$, meaning that there is one Sylow $5$-subgroup, which is normal in $G$. 
Let $x$ be an element of order $3$, which exists by Cauchy's Theorem. As $Q=\langle x \rangle$ and $P$ are cyclic subgroups of relatively prime order, we see that $H=QP$ has order $15$. Additionally, as $P$ is normal, we have $H\leq G$. Notice that $[G:H]=3$, the smallest prime dividing the order of $G$, making $H$ normal in $G$ as well. 
Notice now that $n_3|5$ and $n_3\equiv 1\mod{3}$, and so $n_3=1$ as well. Thus there is only one Sylow $3$-subgroup of $G,$ $K$, which is either $\Z/9$ or $\Z_3/\times\Z/3$. However, $K$ and $H$ are relatively prime to each other regardless and so we have $G=HK$. So the only possibilities for $G$ are $H\times \Z/9$ or $H\times\Z/3\times\Z/3$. 
***
#### Problem 
Let $a, b$ be squarefree integers and set $R=\Z[\sqrt{a}]$ and $S=\Z[\sqrt{b}]$. Prove that
(a) There is a group isomorphism $(R,+) \cong (S,+)$.
(b) There is a ring isomorphism $R \cong S$ if and only if $a = b$.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring in which every element $x$ satisfies $x^n = x$ for some $n > 1$. Show that every prime ideal of $R$ is a maximal ideal.

##### *Proof.*
***
#### Problem 
Consider the subring $\Z[\sqrt{10}] = \{a + b\sqrt{10} \mid a,b \in \Z\}$ of $\R$. Show that $2$ is irreducible but not prime in $\Z[\sqrt{10}]$.

##### *Proof.*
***
#### Problem 
Let $R$ be an integral domain. Prove that if the polynomial ring $R[x]$ is a principal ideal domain, then $R$ must be a field.

##### *Proof.*
***
#### Problem 
Let $F$ be a field and let $f(x)\in F[x]$ be a non zero and non constant polynomial. An element $r\in F$ is called a root of $f(x)$ if $f(r)=0$. 
1. Prove that if $r$ is a root of $f(x)$ then there exists $g(x)\in F[x]$ so that $f(x)=(x-r)g(x)$.
2. Prove that if the degree of $f$ is at most 3, then $f(x)$ is irreducible in $F[x]$ if and only if $f(x)$ has no roots in $F[x]$.
3. Prove that the number of roots of $f(x)$ in $F$ is at most the degree of $f(x)$.

##### *Proof.*
***
#### Problem 
Prove that $f(x)=5x^4 + 7x^3 + 11x^2 + 6x + 1$ is irreducible in $\Q[x]$. *Hint*: Think about how the polynomial factors modulo $2$.

##### *Proof.*
***
## Spring 2022
### Homework 1
#### Problem 
Given a ring $R$, let $R^{op}$ denote the "opposite ring''. This is the same underlying set as $R$ equipped with the same rule for $+$ as $R$, but with multiplication rule (which I will write here as $\cdot_{op}$)redefined to be $a \cdot_{op} b := b a$ (where $ba$ refers to  the original multiplication rule for $R$). Then $R^{op}$ is also a ring --- you don't need to prove that.
Given a left $R$-module $M$, prove that $M$ is a right $R^{op}$-module via the same rule for addition but with the rule for scaling on the right defined to be $m r := rm$ for any $r \in R$ and $m \in M$.

##### *Proof.*
***
#### Problem 
Let $n$ be a positive integer and recall that $\Z/n$ denotes the ring of integers modulo $n$ (whose elements I will write as $\o{0}, \o1, \cdots, \o{n-1}$). 
1. Show that if $M$ is any abelian group (under the operation $+$) such that $nx = 0$ for all $x \in M$ (where $nx := \overbrace{x + x + \cdots + x}^{\text{n times}}$), then the pairing $\Z/n \times M \to M$ given $(\o{j}, m) \mapsto jm$ makes $M$ into a $\Z/n$-module. (Be sure to check this pairing is well-defined.)
2. Conversely, show that if $M$ is a $\Z/n$-module, then the underlying abelian group $(M, +)$ has the property that $nx = 0$ for all $x \in M$.

##### *Proof.*
***
#### Problem 
Let $F$ be any field and $R$ the set of infinte-by-infinite, column-finite matrices. That is, $R$ consists of arrays $A = (a_{i,j})_{i \in \N, j \in \N}$, where
$\N = \{1, 2, \dots \}$ and $a_{i,j} \in R$ for all $i,j$, such that for each $j$, there exists an $I$ (depending on $j$) 
such that $a_{i,j} = 0$ for all $i \geq I$. 
That is, $R$ consists of elements of the form
$$
A = \begin{bmatrix}
a_{1,1} & a_{1,2} & \cdots \\
a_{2,1} & a_{2,2} &  \cdots \\
\vdots & \vdots &  \\
\end{bmatrix}
$$
such that each column has only a finite number of non-zero entries (but, importantly, there is no uniform bound on the number of non-zero entries a
column may have). It is not difficult to see that $R$ is a ring under the usual rules for adding and multiplying matrices: Given $A$ as above and $B=(b_{i,j})_{i \in \N, j \in \N}$ we define
$$
\text{the $(i,j)$ entry of $A + B$ to be $a_{i,j} + b_{i,j}$}
$$
and 
$$
\text{the $(i,j)$ entry of $AB$ to be $\sum_l a_{i,l} b_{l , j}$}.
$$
Note that the latter is a finite sum since, given $j$,  
there is an $L$ such that $b_{l,j} = 0$ for all $l \geq L$. Moreover, $AB$ is column-finite
since, for each such $j$, each of the columns $1, \dots, L-1$ of $A$ has only a finite number of non-zero elements.
The multiplicative identity is the infinite identity matrix.
You need not prove any of this. 

Do prove that $R \cong R^2$ as left $R$-modules. {\em Tip:} Think about splitting up an element of $R$ into its even and odd columns. 

##### *Proof.*
***
#### Problem 
Bases of $R$.
1. Let $R$ be a non-zero, commutative ring. Prove that a subset $A$ of $R$ is a basis of $R$ as a module over itself if and only if $A =\{u\}$ for some unit $u$ of $R$.
2. Let $R$ be the ring of column-finite, infinite-by-infinite matrices with entries in a field $F$, as in  exercise \#3. Prove that for each positive integer $n$, there is a subset of $R$ of cardinality $n$ that forms as a basis for $R$ as a module over itself.

##### *Proof.*
***
#### Problem 
Bases of ideals in commutative rings
1. Assume $R$ is a non-zero, commutative ring and $I$ is a non-zero ideal. Prove $I$ is free as an $R$-module if and only if $I = R \cdot a$ for a non-zero-divisor $a$. (Recall that an  element $a$ is a non-zero-divisor in $R$ provided $a \ne 0$ and $xa = 0$ implies $x = 0$ for all $x \in R$. )
2. Let $F$ be a field and $R = F[x,y]$. Let $I = R \cdot \{x, y\}$, the ideal consisting of all polynomials with $0$ constant term. Prove $I$ is not free as an $R$-module. 

##### *Proof.*
***
#### Problem 
Let $V$ and $W$ be left $R$-modules for any ring $R$. The {\em direct sum} of $V$ and $W$, written $V \oplus W$, is the collection of ordered pairs $(v,w)$ with $v \in V$ and $w \in W$. The direct sum $V \oplus W$ is again an $R$-module under component-wise addition and scaling: $(v_1, w_1) + (v_2, w_2) := (v_1 + v_2, w_1 + w_2)$ and $r (v,w) = (rv , rw)$. You don't need to prove any of that. Do prove the following: 
1. If $V$ and $W$ are free $R$-modules with bases $X$ and $Y$, respectively, then $V \oplus W$ is also free and $Z := \{(x,0) \mid x \in X\} \cup \{(0,y) \mid y \in Y\}$ is a basis of it.
2. Let $\R$ be the real numbers and $\Q$ the rational numbers. Recall that we may view $\R$ as a $\Q$-module (aka $\Q$-vector space)  via restriction of scalars. Prove that $\R \oplus \R$ is isomorphic to $\R$ as a $\Q$-module. (Tip: You may use without proof the following fact, which we will soon prove: since $\Q$ is a field,  every $\Q$-module, including $\R$,  is free. Start by showing  that any basis of $\R$ must be infinite and use that if $X$ is any infinite set, then there exists a bijection from $X$ to $X \times \{0,1\}$. You may take this fact about infinite sets on faith too.) 

##### *Proof.*
***
### Homework 2
#### Problem 
Let $R$ be a ring, let  $M$ be a left $R$-module and let $N \subseteq M$ be a left $R$-submodule.
1. Prove that if $M$ is finitely generated (as an $R$-module), then so is $M/N$.
2. Prove that if $M/N$ and $N$ are both finitely generated, then so is $M$.
3. rove the converse to the previous part is false, as follows: Let $F$ be a field and $R = F[x_1, x_2, \dots]$, the ring of polynomials in the infinite list of variables $x_1, x_2, \dots$. (So, an element of $R$ is a {\em finite} $F$-linear combination of monomials of the form $x_1^{e_1} \cdots x_n^{e_n}$ for $n \geq 0$ and $e_i \geq 1$.\footnote{This is correct as written, but you could also change it to $e_i \geq 0$ if you prefer.} Note that each element of $R$ involves only a finite number of variables, but there is no uniform bound on how many such variables can be involved in the elements of $R$.) You may assume without proof that $R$ is a ring with the usual rules for adding and multiplying polynomials, which make sense since each element of $R$ involves only a finite number of variables. Finally let $I$ be the ideal of $R$ generated by the variables $x_1, x_2, \dots$. Prove $R$ is finitely generated as an $R$-module but the submodule $I$ is not.

##### *Proof.*
***
#### Problem 
Let $R$ be a ring. Recall that we proved in class that every cyclic $R$-module is isomorphic to $R/I$ for some left ideal $I$. Prove the left ideal $I$ occurring this statement is unique; that is, if a cyclic $R$-module is isomorphic to $R/I$ and $R/J$ for left ideals $I$ and $J$, then $I = J$.

##### *Proof.*
***
#### Problem 
Let $R$ be a ring, $M$ and $N$ left $R$-modules, and $p: M \to  N$ an $R$-module homomorphism. Assume that $p$ is surjective.
We say $p$ is a {\em split surjection} if  there exists an $R$-module homomorphism $j: N \to M$ such that $p \circ j = id_N$ (i.e., $p(j(n)) = n$ for all $n \in N$). 
1. Prove that if $N$ is free, then every surjective $R$-module homomorphism of the form $p: M \to N$ is a split surjection. 
2. By giving an explicit example with justification, show the statement in part (a) would become false if $N$ were not assumed to be free.

##### *Proof.*
***
#### Problem 
1. Assume $R$ is a ring, $W$ an $R$-module, and $i: V \to W$ an injective $R$-module homomorphism. We say $i$ is a {\em split injection} if there exists an $R$-module homomorphism $q: W \to V$ such that $q \circ i = id_V$ (i.e., $q(i(v)) = v$ for all $v \in V$). 
2. Prove that if $R$ is a field, $V$ is a subspace (i.e., submodule) of $W$, and $i$ is the inclusion map, then $i$ is a split injection. Note that since $i$ is the inclusion map, what you need to prove is that there exists an $R$-module homomorphism $q: W \to V$ such that $q(v) = v$. {\em Tip}: Start by picking a basis $B$ of $V$ and use a theorem proven in class to show that $B$ can be extended to a basis $C$ of $W$. Use $C$ to construct $q$. (I am assuming that $V$ is a subspace of $W$ and that $i$ is the inclusion map just for simplicity --- more generally, it is true that every injective $R$-module homomorphism is a split injection whenever $R$ is a field.) 
3. Assume $R$ is a non-zero integral domain,  but that it is not a field. Prove there exists an $R$-module homomorphism that is an injection but {\em not} a split injection. {\em Tip}: Pick $a \in R$ such that $a \neq 0$ and $a$ is not a unit, let  $I$ be the proper ideal $I = R \cdot a$ generated by $a$ and show the inclusion map $i: I \to R$ is not a split injection. 

##### *Proof.*
***
#### Problem 
Let $F$ be a field and let $V$ and $W$ be finite dimensional $F$-vector spaces.
1. Let $\a: V \to W$ be an $F$-linear transformation. Prove $\dim(\coker(\a)) - \dim(\ker(\a)) = \dim(W) - \dim(V)$, where by definition $\coker(\a) := W/\im(\a)$. 
2. Let $\phi: V \to V$ be an $F$-linear transformation from $V$ to itself. Prove that if $\phi \circ \phi  = 0$, then $\rank(\phi) \leq \frac12 \dim_F(V)$. (Note: Racall that, by definition, $\rank(\phi) := \dim_F(\im(\phi))$.)
3. For extra credit:  Let $\phi: V \to V$ be an $F$-linear transformation from $V$ to itself. Prove that if $\overbrace{\phi \circ \cdots \circ \phi}^{\text{n times}}  = 0$ for some $n \geq 1$ then $\rank(\phi) \leq \frac{n-1}{n} \dim_F(V)$. 

##### *Proof.*
***
### Homework 3
### Homework 4
#### Problem 
Let $R$ be a non-zero commutative ring and   $A \in \Mat_{n    \times n}(R)$. Let $A^{adj}$ denote the classical adjugate of $A$ --- the $(i,j)$ entry of $A^{adj}$ is defined to be $(-1)^{i+j} \det(A_{j,i})$ where $A_{j,i}$ is $(n-1) \times (n-1)$ matrix obtained by deleting the $j$-th row and $i$-th column of $A$. You may assume without proof that when $R$ is a field, we have $A A^{adj} = \det(A) I_n = A^{adj} A$. Prove $A A^{adj} = \det(A) I_n = A^{adj} A$ holds for any non-zero commutative ring $R$.

##### *Proof.*
***
#### Problem 
Let $V$ be the $\R$-vector space consisting of polynomials in the variable $x$ of degree at most $3$ and let $g: V \to V$ be the $\R$-linear operator given by $$g(p(x)) = p''(x) + (x+1) p'(x) + 7 p(x),$$where $p''(x)$ and $p'(x)$ denote the first and second derivatives of $p(x)$. (You may take it on faith that $g$ is $\R$-linear.) Find the determinant, the trace, and the characteristic polynomial of $g$.

##### *Proof.*
***
#### Problem 
Let $F$ be a field and $V = F[x]/I$ with $I = F[x] \cdot f(x)$  for some monic polynomial $f(x) = x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$. Regard $V$ as an $F$-vector space (via restriction of scalars along $F \into F[x]$), and recall that the function $g: V \to V$ given by $g(v) = x \cdot v$ is an $F$-linear operator on $V$.

Prove that the characteristic polynomial of $g$ is $f(x)$.

##### *Proof.*
***
#### Problem 
Let $A = \begin{bmatrix} 6 & 4 & 2 \\ 2 & 7 & 4 \end{bmatrix} \in \Mat_{2 \times 3}(\Z)$. 
1. Find invertible matrices $P$ and $Q$ such that $B := PAQ$ is diagonal (i.e., $b_{i,j} = 0$ for all $i \ne j$). 
2. Find all integer solutions of $A \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}$.

##### *Proof.*
***
#### Problem 
Let $A = \begin{bmatrix} 3 & 1 & -4 \\ 2 & -3 & 1 \\ -4 & 6 & -2 \end{bmatrix} \in \Mat_{3 \times 3}(\Z)$. Express the $\Z$-module presented by $A$ as the direct sum of cyclic groups. Justify your answer. 

##### *Proof.*
***
### Homework 5
#### Problem 
({\em Note}: This problem was on your mid-term exam.)  Let $R$ be a Euclidean domain, $A$ an $m \times n$ matrix with elements from $R$, and $A^T$ the transpose matrix of $A$. Let $\coker(A)$ denote the quotient of $R^m$ by the submodule generated by the columns of $A$. The {\em torsion} submodule of an $R$-module $M$ is the submodule $\{m \in M \mid rm = 0 \text{ for some $r \ne 0$}\}$. (It is indeed a submodule and you need not prove this.) 
1. Prove that the torsion submodules of $\coker(A)$ and $\coker(A^T)$ are isomorphic.
2. Prove that the modules $\coker(A)$ and $\coker(A^T)$ are isomorphic if and only if $m = n$.

##### *Proof.*
***
#### Problem 
Let $A$ and $B$ be $n \times n$ matrices with entries in $\Q$. Prove $A$ and $B$
are similar in $\Mat_{n \times n}(\Q)$ if and only if $A$ and $B$ are similar in $\Mat_{n \times n}(\R)$. (That is, show there is a $P \in GL_n(\Q)$ such that $A = PBP^{-1}$ if and only if there is a $R \in GL_n(\R)$ such that $A = RBR^{-1}$.) {\em Tip}: Use the Theorem on Rational Canonical Forms.

##### *Proof.*
***
#### Problem 
Find the Rational Canonical Form of 
$$
A = \begin{bmatrix}
0 & -1 & - 1\\
0 & 0 & 0 \\
-1 & 0 & 0 \\
\end{bmatrix} \in \Mat_{3 \times 3}(F),
$$
where $F$ is any field. 

##### *Proof.*
***
#### Problem 
Similarity of two-by-two matrices:
1. Let $F$ be any field and $A, B \in \Mat_{2 \times 2}(F)$, and  assume that neither $A$ nor $B$ is a scalar matrix. (Recall that a scalar matrix is one of the form $c I_n$ for some $c \in F$.) Prove $A$ and $B$ are similar if and only if they have the same determinant and the same trace.
2. Let $F$ be a finite field with $q$ elements. Find, with justification,  the number of similarity classes of $2 \times 2$ matrices with entries in $F$.
3. Let $F$ be a finite field with $q$ elements. Find, with justification, the number of conjugacy classes of the group $GL_2(F)$. 

##### *Proof.*
***
#### Problem 
Let $F$ be any field. Up to similarity, how many matrices in $\Mat_{5 \times 5}(F)$ of the form
$$A = \begin{bmatrix}
1 & * & * & * & * \\
0 & 1 & * & * & * \\
0 & 0 & 1 & * & * \\
0 & 0 & 0 & 1 & * \\
0 & 0 & 0 & 0 & 1 \\
\end{bmatrix}
$$
are there? Justify. 

##### *Proof.*
***
#### Problem 
Let $F$ be a field, $V$ a finite dimensional $F$-vector space,  and $g: V \to V$ an $F$-linear operator. Prove that the following are equivalent for an element $\lambda \in F$:
1. $\lambda$ is an eigenvalue of $g$.
2. $\lambda$ is a root of the minimum polynomial $\mp_g(x)$ of $g$. 
3. $\lambda$ is a root of the characteristic polynomial $\cp_g(x)$ of $g$.
(Recall that $\lambda \in F$ is a {\em eigenvalue} of $F$ provided $g(v) = \lambda \cdot v$ for some non-zero vector $v \in V$.)

##### *Proof.*
***
### Homework 6
#### Problem – May 2021 (6)
For any integer $n \geq 1$, consider the $\C$-[[Vector Space|vector space]] $V = \{p \in \C[x] : \deg(p) \leq n - 1\}$.

(a) Let $T:V \to V$ be the [[Linear Operator|linear operator]] given by $T(p) = xp'$ (where $p'$ denotes the derivative of $p$). Find with justification the Jordan Canonical Form of $T$. 
(b) Let  $D:V \to V$ be the linear operator given by $D(p) = p'$. Find with justification the Jordan Canonical Form of $D$. 

##### *Proof.*
For any integer $n \geq 1$, consider the $\C$-vector space $V = \{p \in \C[x] : \deg(p) \leq n - 1\}$.

###### Part (a)
Let $T:V \to V$ be the linear operator given by $T(p) = xp'$ (where $p'$ denotes the derivative of $p$). Note that the change of basis matrix for this operator is given by $$
\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix},$$with the basis $\{1,x,\dots,x^{n-1}\}$. Thus $\cp_A(x)$ will be given by the determinant of the matrix
$$\begin{bmatrix}
  x & 0 & \cdots & 0 & 0 \\
  0 & x-1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & x-(n-1) \\   
\end{bmatrix},$$
which is diagonal. Hence $\cp_AT(x)=\displaystyle\prod_{i=0}^{n-1}(x-i)$. Thus $\cp_AT(x)$ factors into distinct linear polynomials, each of which is in the form $(x-i)^1$ for $0\leq i\leq n-1$. Thus each linear term is an elementary divisor, making each Jordan block a $1\times1$ matrix with $i$ as the only entry. Thus the Jordan Canonical form is $$\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix}.$$
***
###### Part (b)
This time around the change of basis matrix (denoted $B$ and using the same basis as above) for this matrix has 0s along the diagonal, and increasing natural numbers (starting at 0, sorry) along the upper diagonal. Thus $\cp_B(x)=x^n$.

Recall that the minimal polynomial corresponding to $B$ will be the the smallest monic polynomial such that $B$ is sent to 0. Note that as $D$ is the operator sending $p$ to its derivative, and that $D^{(2)}=D(D(p))=p''=p^{(2)}$. Thus $B^2$ can be viewed as a change of basis matrix for taking the second derivative of the basis, and so on.

As the basis extends to $x^{n-1}$, it requires $n$ derivatives to make this polynomial become 0. Thus the minimal polynomial of $B$ must be $x^n$, as it it monic and $B^n=0$. As the degree of the invariant factors must sum to $n$ and $\mp_B(x)=x^n$, which is itself an invariant factor, we see that it must in fact be the only one.

As $x^n$ is already a power of a prime, it is the only elementary divisor as well. Thus the Jordan Canonical Form for $B$ is an $n\times n$ Jordan Block with 0s along the diagonal and 1s along the sub-diagonal. 
***
#### Problem – June 2016 (7)
Let $g: V \to V$ be an $F$-[[Linear Operator|linear operator]] on a finite dimensional [[Vector Space|vector space]] $V$, where  $F$ is a field. Recall than $g$  is *diagonalizable* provided there is some basis $B$ of $V$ such that $[g]_B^B$ is a diagonal matrix. Prove $g$ is diagonalizable if and only if its minimum polynomial factors completely into *distinct* linear factors.

##### *Proof.*
$(\Rightarrow)$ Suppose that $g$ is diagonalizable. Thus there exists a change of basis matrix $A$ such that $A$ is diagonal. As it is diagonal, its diagonal entries are the eigenvalues of $g$, and thus the roots of the minimal polynomial of $g$ by Problem 6 on the previous homework. Using row and column operations we can rearrange $A$ so that all repeated linear factors are next to each other in the diagonal, for convenience. 

We know that $\mp_A(x)$ is the smallest monic polynomial that sends $A$ to 0. Take all the distinct eigenvalues $\lambda_i$ and consider $q(x)=\prod(x-\lambda_i)$. 

We examine $q(A)$. It will be a product of matrices, one for each $\lambda_i$. First, take the first matrix in this product, $(A-\lambda_1I)$, and note that it sends all $\lambda_1$ in $A$ to 0. Thus all of the rows and columns that contained a $\lambda_1$ are now 0, and thus all these rows and columns will be 0 in the final product $q(A)$. As this is we set $q(x)=\prod(x-\lambda_i)$ for all $l\lambda_i\in A$, we see that for each row and column in $A$ there will exist a matrix $A-\lambda_iI$ in the product $q(A)$ such that the row and column will be 0. Thus the entire matrix will be 0, and $q(A)=0$.

Note that if any $\lambda_i$ were excluded from $q(x)$ there would exist a non-zero row and column for every matrix in the product, and thus $q$ would not send $A$ to 0. Thus $q(x)$ is indeed the minimal polynomial of $A$. As $q(x)=\prod(x-\lambda_i)$, we see it does indeed factor into distinct linear terms. 

$(\Leftarrow)$ Suppose the minimum polynomial of $g$ factors completely into distinct linear factors, each of which has the form $x-\lambda_i$ for some $\lambda_i\in F$. As each $\lambda_i$ is distinct, each elementary divisor is of the form $(x-\lambda_i)^1$.

Using Theorem 1.222 we construct the Jordan Canonical Form of $g$. As the elementary divisors are linear the Jordan blocks are $1\times1$ matrices, making the $JCF$ a diagonal matrix. As the JCF is itself a change of basis matrix, we see that $g$ is diagonalizable.
***
#### Problem 
Let  $\Q(i) = \{a + bi \mid a, b \in \Q\}$ and $\Z[i] = \{a + ib \mid a, b \in \Z\}$ and recall (from 817) that $\Z[i]$ is a PID and $\Q(i)$ is its field of fractions.
(a) Prove $x^6 + 7$ is irreducible in $\Q(i)[x]$.
(b) Prove $x^4 - 6x^2 + 10$ is irreducible in $\Q[x]$ but is reducible in $\Q(i)[x]$. 

##### *Proof.*
Let  $\Q(i) = \{a + bi \mid a, b \in \Q\}$ and $\Z[i] = \{a + ib \mid a, b \in \Z\}$.

###### Part (a)
Suppose by way of contradiction that $7$ is not prime in $\Z[i]$. Thus $7=\alpha\beta$, with $\alpha,\beta$ non-units and where $\alpha=a+bi$ and $\beta=c+di$, for $a,b,c,d\in Z$. Thus $\overline{7}=\overline{\alpha\beta}=\overline{\alpha}\overline{\beta}$. As $\overline{7+0i}=49$, we see that $\overline{\alpha}=(a^2+b^2)|49$. Note that the possible factorizations of 49 in $\Z$ are $(1)(49)$ and $(7)(7)$.

However, if $\overline{\alpha}=49$ then $\overline{\beta}=1$, making it a unit. So $\overline{\alpha}=7$ and thus $a^2+b^2=7$. As $a^2, b^2\leq0$, either $a=0$ or $b=0$. But then either $a^2=7$ or $b^2=7$, and as $\sqrt{7}\not\in\Z$, we have a contradiction. Thus $7$ is prime in $\Z[i]$. Using Eisenstein's Criterion with $p=7$, we see that $x^6 + 7$ is irreducible in $\Q(i)[x]$.
***
###### Part (b)
Using Eisenstein's Criterion with $p=2$, we see that $x^4 - 6x^2 + 10$ is irreducible in $\Q[x]$. However, in $\Q(i)[x]$ observe that $$x^4-6x^2+10=(x^2-(3+i))(x^2-(3-i)).$$ As neither $(x^2-(3+i))$ nor $(x^2-(3-i))$ are units in $\Q(i)[x]$ (as $x$ has no inverse), we see that $x^4-6x^2+10$ is reducible in $\Q(i)[x]$.
***
#### Problem 
Consider the two field extensions $\Q \subseteq \Q(i, \sqrt{3})$ and $\Q \subseteq \Q(i, \sqrt[3]{2})$.
(a) Prove they have degrees $4$ and  $6$, respectively. {\em  Tip}: For the second one,  show $x^3 - 2$ is irreducible in $\Q(i)[x]$.
(b) Find a primitive element $\gamma$ for the extension $\Q \subseteq \Q(i, \sqrt{3})$ and find $m_{\gamma, \Q}(x)$.
(c) (For extra credit.) Find a primitive element $\delta$ for the extension $\Q \subseteq \Q(i, \sqrt[3]{2})$  and find $m_{\delta, \Q}(x)$.

##### *Proof.*
Consider the two field extensions $\Q \subseteq \Q(i, \sqrt{3})$ and $\Q \subseteq \Q(i, \sqrt[3]{2})$.

###### Part (a)
Consider the polynomial $x^2-3$. This has a root $\sqrt{3}$, which is not in $\Q$. Thus, as $x^2-3$ has degree 2, it is irreducible by Theorem 2.2, making it the minimal polynomial of $\Q(\sqrt{3})$. Thus by Theorem 2.31 we see that $[\Q(\sqrt{3}):\Q]=2$.

Next, consider the polynomial $x^2+1$. This has a root $i$, which is not in $\Q(\sqrt[3]{2})$ as $\Q(\sqrt[3]{2})\subseteq\R$ and $i\not\in\R$. Let $K=\Q(\sqrt[3]{2})$ for convenience. As $x^2+1$, has degree 2, it is irreducible by Theorem 2.2, making it the minimal polynomial of $K(i)$. Thus by Theorem 2.31 we see that $[K(i):K]=2$. Thus by the degree formula we have $[K(i):\Q]=[K(i):K][K:\Q]=2(2)=4$.

By Example 2.22 we see that $[\Q[\sqrt[3]{2}]:\Q]=3$. However, as $\sqrt[3]{2}$ is the root of $x^3-2$ it is algebraic over we see that $\Q[\sqrt[3]{2}]=\Q(\sqrt[3]{2})$ and thus that $[\Q(\sqrt[3]{2}):\Q]=3$. 

Next, consider the polynomial $x^2+1$. This has a root $i$, which is not in $\Q(\sqrt[3]{2})$ as $\Q(\sqrt[3]{2})\subseteq\R$ and $i\not\in\R$. Let $L=\Q(\sqrt[3]{2})$ for convenience. As $x^2+1$, has degree 2, it is irreducible by Theorem 2.2, making it the minimal polynomial of $L(i)$. Thus by Theorem 2.31 we see that $[L(i):L]=2$. Thus by the degree formula we have $[L(i):\Q]=[L(i):L][L:\Q]=2(3)=6$.
***
###### Part (b)
Consider $\gamma=\sqrt{3}+2i$, and note that $\gamma^2=-1+4\sqrt{3}i$ and $\gamma^3=-9\sqrt{3}+10i$. Thus $\frac{1}{28}(\gamma^3+9\gamma)=i$ and $\frac{-1}{14}(\gamma^3+9\gamma)=\sqrt{3}$. Thus $\gamma$ is a primitive element of this extension field.

Next, consider the monic polynomial $x^4+2x^2+49$, and observe $$\begin{align}
    0&=x^4+2x^2+49\\
    -48&=x^4+2x^2+1\\
    (16)(3)(-1)&=(x^2+1)^2\\
    4\sqrt{3}i&=(x^2+1)\\
    -1+4\sqrt{3}i&=x^2.
\end{align}$$However, as $\gamma^2=-1+4\sqrt{3}i$, we see that $\gamma$ is the root of this polynomial. Since this is a monic polynomial of degree $4=[K(i):\Q]$, it must be the minimal polynomial as well. Thus the minimal polynomial of $[K(i):\Q]=x^4+2x^2+49$.
***
###### Part (c)
Consider $\gamma=\sqrt[3]{2}i$, and note that $\frac{-1}{2}\gamma^{-2}=\frac{-1}{2}\frac{1}{-\sqrt[3]{2}^2}=\frac{-1}{2}\frac{\sqrt[3]{2}}{-2}=\sqrt[3]{2}$, and $2\gamma^{-3}=2\frac{-1}{2i}=2\frac{i}{2}=i$. 

Consider $x^6-4$, and note that $\gamma^2=2^{2/3}$, and thus $\gamma^6=2^2=4$. Thus $\gamma^6-4=0$, so $\gamma$ is a root of this polynomial. Since this is a monic polynomial of degree $6=[L(i):\Q]$, it must be the minimal polynomial as well. Thus the minimal polynomial of $[L(i):\Q]=x^6-4$.
***
#### Problem – May 2021 (7)
Assume that $F \subseteq K$ is a finite extension of fields of degree $n = [K : F ]$.

(a) Prove that if $f \in F[x]$ is irreducible of degree $d$ and $\gcd(d, n) = 1$ then $f$ remains irreducible when regarded as an element of the ring $K[x]$.
(b) Show, by means of an explicit example with justification, that the statement in part (a) would become false if the assumption that $\gcd(n, d) = 1$ were omitted.

##### *Proof.*
Let $F \subseteq K$ be a finite extension of fields of degree $n = [K : F ]$.

##### Part (a)
Suppose that $f \in F[x]$ is irreducible of degree $d$ and $\gcd(d, n) = 1$. 

First, note that if $d=1$ then $f(x)$ will remain irreducible in $K[x]$ by Theorem 2.2.
Suppose then that $d>1$. By Theorem 2.51 there exists an algebraically closed extension $\widetilde F$ such that $f$ has a root $r$. Consider $K(r)$. As $r$ is algebraic in $K(r)$ we know there exists some unique irreducible minimal polynomial $g$ of degree $q$, and thus that $[K(r):K]=q$ by Theorem 2.31. Using the Degree Formula we see that $$[K(r):F]=[K(r):K][K:F]=qn.$$However, $[K(r):F]=[K(r):F(r)][F(r):F]$ and so $qn=md$ for some $m\in\Z$, so $d|qn$. As $\gcd(n,d)=1$ we must have $d|q$. But $q$ was defined to be the degree of $g$, which divides $f$. As $d|q$ and $q\leq d$, we see that $d=q$, so $f=kg$ for some $k\in F$. As irreducible polynomials multiplied by a constant are still irreducible, we see that $f$ is indeed irreducible in $K[x]$.
***
##### Part (b)
Let $p(x)$ be a non-constant irreducible polynomial of degree $d$ in $F[x]$. Let $K=F[x]/p(x)$. Because $p(x)$ is irreducible and $F[x]$ is a PID, $(p(x))$ is a maximal ideal. Thus $K = F[x]/(p(x))$ is a field, $[K:F]=d$, and $x+p(x)$ is a root of $p(x)$ in $K$ By Proposition 2.23. Hence $p(x)$ is no longer irreducible by Theorem 2.2.
***
#### Problem 
Let $E$ be the field extension of $\Q$ obtained by adjoining to $\Q$ all four complex roots of the polynomial $x^4 + 5$. ($E$ is what's known as the "splitting field'' of $x^4 + 5$  over $\Q$.) That is, $E = \Q(\a_1, \a_2, \a_3, \a_4)$ where
$\a_1 = e^{\pi i/4}\sqrt[4]{5}$,
$\a_2 = e^{3\pi i/4}\sqrt[4]{5}$,
$\a_3 = e^{5\pi i/4}\sqrt[4]{5}$, and
$\a_4 = e^{7\pi i/4}\sqrt[4]{5}$.
(a) Prove that there exist a field extension $\Q \subseteq F$ such that $F \subseteq E$, $F \subseteq \R$ and $[F :\Q]=4$. *Tip*: Note that  $\a_1 + \a_4$ is  real number; find it explicitly. 
(b) Determine, with justification, $[E : \Q]$.

##### *Proof.*
Let $E$ be the field extension of $\Q$ obtained by adjoining to $\Q$ all four complex roots of the polynomial $x^4 + 5$.

##### Part (a)
Let $F=\Q(\sqrt[4]{20})$. Note that by Eisenstein's Criterion using $p=5$ we see that $\sqrt[4]{20}$ is the root of an irreducible polynomial $x^4-20$ in $\Q$. Thus by Theorem 2.31 we see that $[F:\Q]$ is the degree of the minimum polynomial of this extension. However, as $x^4-20$ is monic and of degree 4, we see that it is the minimal polynomial and thus that $[F:\Q]=4$. As $\sqrt[4]{20}\in\R-\Q$, this extension will be contained in the real numbers, and thus that $F\subseteq\R$.

Next, observe
$$\begin{align}
    \alpha_1+\alpha_4&=e^{\pi i/4}\sqrt[4]{5}+e^{7\pi i/4}\sqrt[4]{5}\\
    &=(\cos(\frac{\pi}{4})+i\sin(\frac{\pi}{4}))\sqrt[4]{5}+(\cos(\frac{7\pi}{4})+i\sin(\frac{7\pi}{4}))\sqrt[4]{5}\\
    &=(\frac{\sqrt{2}}{2}+i\frac{\sqrt{2}}{2})\sqrt[4]{5}+(\frac{\sqrt{2}}{2}-i\frac{\sqrt{2}}{2})\sqrt[4]{5}\\
    &=\sqrt{2}\sqrt[4]{5}\\
    &=\sqrt[4]{20},
\end{align}$$
and thus that $F\subseteq E$.
***
##### Part (b)
Note that $i$ is the root of $x^2+1$, and since $F\subseteq\R$ and $i\not\in\R$, we see that $x^2+1$ is irreducible in $F$ due to it having degree 2. As $x^2+1$ is monic and degree 2 we see its the minimal polynomial of $[F(i):F]=2$. By the Degree Formula, we see that $[F(i):\Q]=[F(i):F][F:\Q]=(2)(4)=8$.

Note that 

$\a_1 = e^{\pi i/4}\sqrt[4]{5} = \cos(\frac{\pi}{4})+i\sin(\frac{\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}+i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{20}(1+i)$,

$\a_2 = e^{3\pi i/4}\sqrt[4]{5} = \cos(\frac{3\pi}{4})+i\sin(\frac{3\pi}{4})\sqrt[4]{5} = \frac{-\sqrt{2}}{2}\sqrt[4]{5}-i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{20}(-1+i)$,

$\a_3 = e^{5\pi i/4}\sqrt[4]{5} = \cos(\frac{5\pi}{4})+i\sin(\frac{5\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}+i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{20}(-1-i)$, and

$\a_4 = e^{7\pi i/4}\sqrt[4]{5} = \cos(\frac{7\pi}{4})+i\sin(\frac{7\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}-i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{20}(1-i)$, all of which can be written with $i$ and $\sqrt[4]{20}$. Thus $E\subseteq F(i)$. 

We already know that $\alpha_1+\alpha_4=\sqrt[4]{20}$, and thus all that remains is to show that $i$ can be expressed in terms of the $\alpha$. Observe
$$\begin{align}
    \alpha_1+\alpha_2&=e^{\pi i/4}\sqrt[4]{5}+e^{3\pi i/4}\sqrt[4]{5}\\
    &=(\cos(\frac{\pi}{4})+i\sin(\frac{\pi}{4}))\sqrt[4]{5}+(\cos(\frac{3\pi}{4})+i\sin(\frac{3\pi}{4}))\sqrt[4]{5}\\
    &=(\frac{\sqrt{2}}{2}+i\frac{\sqrt{2}}{2})\sqrt[4]{5}+(\frac{\sqrt{2}}{2}+i\frac{\sqrt{2}}{2})\sqrt[4]{5}\\
    &=\sqrt{2}\sqrt[4]{5}\\
    &=\sqrt[4]{20}i,
\end{align}$$
and thus that $(\alpha_1+\alpha_2)(\alpha_1+\alpha_4)\inv=i$. Thus $F(i)\subseteq E$, and $F(i)=E$. Hence $[E:\Q]=8$.
***
### Homework 7
#### Problem – $[L: \Q]$ and $(x^p -2)$
Let $L$ be the splitting field of $x^p -2 \in \Q[x]$ over $\Q$ where $p$ is an odd prime integer. Find $[L: \Q]$. *Tip*: Consider both chains $\Q \subseteq \Q(\sqrt[p]{2}) \subseteq L$ and $\Q \subseteq \Q(e^{2 \pi i/p}) \subseteq L$.

##### *Proof.*
As seen in Example 2.60, $e^{2\pi i/p}$ is a root of the $(n-1)$th cyclotomic polynomial, which is monic and irreducible in $\Q$. Hence $e^{2\pi i/p}$ is the minimal polynomial of the $(n-1)$th cyclotomic polynomial in $\Q[x]$, and thus the field extension $\Q(e^{2\pi i/p})$ has degree $p-1$ over $\Q$ by Theorem 2.31. It follows that $[\Q(e^{2\pi i/p}):\Q]=p-1$. 

Next, note that $\sqrt[p]{2}$ is a root of the polynomial $x^p-2$, making it algebraic over $\Q$. Using Eisenstein's Criterion in conjunction with the prime $q=2$ we see that $x^p-2$ is irreducible in $\Q[x]$. As $\gcd(p,p-1)=1$, by Problem 5 on the previous homework we see that $x^p-2$ is irreducible in $\Q(\sqrt[p]{2})$ as well. As $x^p-2$ is irreducible and monic, we see that it is the minimal polynomial of $\sqrt[p]{2}$ in $\Q(e^{2\pi i/p})[x]$, and thus $$[\Q(e^{2\pi i/p},\sqrt[p]{2}):\Q(e^{2\pi i/p})]=p.$$
Using the degree formula, we see that $$[\Q(\sqrt[p]{2},e^{2\pi i/p}):\Q]=[\Q(e^{2\pi i/p},\sqrt[p]{2}):\Q(e^{2\pi i/p})][\Q(\sqrt[p]{2}):\Q]=p(p-1).$$
Notice that $\sqrt[p]{2}\cdot (e^{{2\pi i/p}^n})$, where $1\leq n\leq p$, which are all roots of $x^p-2$. By the Factor Theorem, there can be no other roots of this polynomial. Thus $L\subseteq\Q(\sqrt[p]{2},e^{2\pi i/p})$.

Additionally, notice that $e^{2\pi i/p}$ and $\sqrt[p]{2}$ are both roots of $x^p-2$. Thus they are both contained in $L$. Observe $\frac{e^{2\pi i/p}\sqrt[p]{2}}{\sqrt[p]{2}}=e^{2\pi i/p}$. Hence $\Q(\sqrt[p]{2},e^{2\pi i/p})\subseteq L$, and thus we see that $L=\Q(\sqrt[p]{2},e^{2\pi i/p})$. Therefore, $[L:\Q]=p(p-1)$. 
***
#### Problem – June 2020 (9)
Assume $F$ is field and let $f(x) \in F[x]$.
(a) Assume $\chr(F) = 0$. Prove that $f(x)$ is not separable if and only if the prime factorization of $f(x)$ in $F[x]$ admits a repeated factor. (We will define "separable'' in class shortly, but here is the definition: $f$ is separable if and only if $f$ has no repeated roots in an algebraic closure $\overline{F}$ of $F$.)
(b) Give a counter example to the previous part when the assumption $\chr(F ) = 0$ is omitted.

##### *Proof.*
###### Part (a)
Assume $\chr(F) = 0$.
$(\Rightarrow)$ Suppose that $f$ is not separable, so $f$ has a repeated root in $\overline{F}$, which we denote $\alpha$. So $x-\alpha$ is a factor of $f(x)$. By Corollary 2.96, $F(\alpha)$ is separable, so the minimal polynomial of $\alpha$ in $F[x]$ has no repeated root in $\overline{F}$. As $f$ does have a repeated root (by supposition) it cannot be the minimum polynomial of $\alpha$. Thus $f(x)=\mp_{\alpha,F[x]}(x)g(x)$ for some $g(x)\in F[x]$ such that $g(x)$ has $\alpha$ as a root, otherwise $f$ would not obtain its repeated root. However, this means that $\mp_{\alpha,F[x]}(x)\big|g(x)$, meaning that $g(x)$ has $x-\alpha$ as a factor as well. Thus we see that $x-\alpha$ is a repeated factor of $f(x)$, one from the minimum polynomial, one from $g(x)$.

$(\Leftarrow)$ Suppose that the prime factorization of $f(x)$ in $F[x]$ admits a repeated factor. Thus there exists some prime (and thus irreducible, as we are in a UFD) $g(x)$ such that $g(x)g(x)|f(x)$. However, $g$ has a root $\alpha$ in $\overline{F}$, so in $F(\alpha)$ we see that $f(x)$ has $\alpha$ as a root as well, as $g(a)=0$. But since $g(x)$ has factor $x-\alpha$, it shows up twice in the factorization of $f$ because $g(x)g(x)|f(x)$. So $\alpha$ has multiplicity at least 2, so $f$ is not separable. 
***
###### Part (b)
Let $y,z$ be indeterminants, $F=\Z/3(y)$, and $L=\Z/3(z)$ such that $z^3=y$ (as seen in Example 2.78). Note then that $z^3$ is a root of the polynomial $x^3-y\in F[x]$.

Moreover, since $F$ is the field of fractions of the PID $R=(\Z/3)[y]$ and $y$ is a prime element of R, we may apply Eisenstein's Criterion (using $p=y$) to conclude that $x^3-y$ is irreducible in $F[x]$. Thus $x^3-y$ is the minimum polynomial of $z$ in $F[x]$.

However, as the derivative of this polynomial is 0, we see that the $\mp_{z,F[x]}(x)$ is not separable by Proposition 2.72. However, by the Freshman's Dream, we see that $x^3-y=x^3-z^3=(x-z)^3\in L$. But as $z\not\in F$, we see that the prime factorization of $x^3-y$ admits no repeated factor.
***
#### Problem – May 2017 (9)
Let $f(x) \in \Q[x]$ be an irreducible cubic (degree $3$) polynomial having exactly one real root. Let $L$ be the splitting field of $f(x)$ over $\Q$. Show that $\Aut(L/\Q) \cong S_3$.

##### *Proof.*
Let $f(x) \in \Q[x]$ be an irreducible cubic (degree $3$) polynomial having exactly one real root, and let $L$ be the splitting field of $f(x)$ over $\Q$.

As $L$ is the splitting field of $f$, it is a normal extension. As $\Q$ has characteristic 0, $L$ is separable (because $L$ is algebraic extension, as its the extension caused by adjoining each root of $f$, and algebraic extensions of algebraic extensions are algebraic). Thus by Theorem 2.90 we see that $|\Aut(L/\Q)|=[L:F]$.

By Proposition 2.83 we see that $\Aut(L/F)$ is isomorphic to some subgroup of $S_m$, where $m$ is the number of distinct roots of $f$. As $f$ cubic and irreducible we know that the real root must be irrational, which we will denote $\alpha$. Consider the extension $\Q(\alpha)$. As $\alpha\not\in\Q$, we see that $[\Q(\alpha):\Q]\geq 2$. However, neither of our complex roots are in this extension, and so another extension is needed to reach $L$. But this extension would also have a degree larger than $1$, so $[L:\Q]\geq4$. As $|S_2|=2$, there exists no subgroup of it that $\Aut(L/F)$ can be isomorphic to, given that $|\Aut(L/\Q)|=[L:F]$. Thus we see that $m=3$, meaning that our complex roots are distinct.

Then $|\Aut(L/F)|=1,2,3,$ or $6$, the only possible sizes of subgroups of $S_3$. However, by the previous argument we see that as $[L:\Q]\geq4$, the only viable subgroup of $S_3$ is $S_3$ itself. Thus $\Aut(L/\Q) \cong S_3$.
***
#### Problem – Radical Element and $\Aut$
Assume $F \subseteq L$ is a finite extension of fields and that the characteristic of $F$ is $p$, where $p$ is a prime. Suppose there exists an element $a \in L$ such that $a \notin F$ but $a^p \in F$.
(a) Prove $\sigma(a) = a$ for all $\sigma \in \Aut(L/F)$.
(b) Prove $|\Aut(L/F)| < [L : F]$. 

##### *Proof.*
Let $F \subseteq L$ be a finite extension of fields and that the characteristic of $F$ is $p$, where $p$ is a prime. Suppose there exists an element $a \in L$ such that $a \notin F$ but $a^p \in F$.

###### Part (a)
Let $\sigma\in\Aut(L/F)$. Thus $\sigma(x)=x$ for all $x\in F$. Let $b=\sigma(a)$. Thus $b^p=\sigma(a)^p=\sigma(a^p)=a^p$. Thus $a^p-b^p=0$. We proceed via cases:

First, suppose that $p$ is an odd prime. Then by the Freshman's Dream we see that $0=a^p-b^p=(a-b)^p$. As we are in a domain, it must be the case that one of the $(a-b)=0$, and thus they all must be. Thus $a=b$, and $\sigma(a)=a$ for all $\sigma\in\Aut(L/F)$.

Next, suppose that $p$ is an even prime (not naming names, you know who you are). Then we have $a^2-b^2=0$, and thus by the Freshman's Dream we see that $(a-b)^2=0$, and so $(a+b)(a-b)=0$, so either $a=b$ or $a=-b$. However, if $a=-b$ then we can substitute back in to see that $0=(a-b)^2=a^2$, so $a=0$, contradicting the fact that $a\not\in F$. Thus $a=b$, and $\sigma(a)=a$ for all $\sigma\in\Aut(L/F)$.
***
###### Part (b) 
By Proposition 2.85, we know that $|\Aut(L/F)|<[L:F]$. Consider the polynomial $f(x)=x^p-a^p$. Suppose by way of contradiction that $f$ is reducible. Thus there exists polynomials (with coefficients in $F$) such that $g(x)h(x)=f(x)$. When viewed in $L$, we see by the Freshman's Dream that $f(x)=x^p-a^p=(x-a)^p$. As $L$ is a field it is a UFD, and since $x-a$ is irreducible it is also prime. Thus this is the only prime factorization of $f(x)$. Since $g(x)h(x)=(x-a)^p$, we see that $g(x)=(x-a)^n$ and $h(x)=(x-a)^m$, where $n+m=p$. However, when viewed back in $F$, we see that when foiled out $g(x)$ will contain the term $x^{n-1}a$. (See: Binomial Theorem). However, $a\not\in F$, which is bad. There would be a binomial coefficient attached, but as $F$ is a field and thus closed, it could still be removed by multiplying by its inverse. Thus $x^p-a^p$ is irreducible in $F$. As $f$ is irreducible, monic, and has $a$ as a root, we see that $f$ is the minimal polynomial of $a$ in $F$. However, as $f'(x)=px^{p-1}=0$, we see that it is not separable. Thus $|\Aut(L/F)|\neq[L : F]$ by Theorem 2.90, and so $|\Aut(L/F)|<[L : F]$, as desired.
***
#### Problem – $\Aut(E/\Q)$, $(x^4 + 5)$, and $D_8$. 
Let $E$ be the splitting field of $x^4 + 5$ over $\Q$. (Recall  that this extension occurred on the last problem set, and that $E = \Q(\a_1, \a_2, \a_3, \a_4)$ where
- $\a_1 = e^{\pi i/4}\sqrt[4]{5}$,
- $\a_2 = e^{3\pi i/4}\sqrt[4]{5}$,
- $\a_3 = e^{5\pi i/4}\sqrt[4]{5}$, and
- $\a_4 = e^{7\pi i/4}\sqrt[4]{5}$.)
Prove $\Aut(E/\Q) \cong D_8$. 

##### *Proof.*
Note that from the previous homework, we know that $[E:\Q]=8$, and that $E=\Q(\sqrt[4]{20},i)$. Additionally, we know the following:
- $\a_1 = e^{\pi i/4}\sqrt[4]{5} = \cos(\frac{\pi}{4})+i\sin(\frac{\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}+i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{5/4}(1+i)$,
- $\a_2 = e^{3\pi i/4}\sqrt[4]{5} = \cos(\frac{3\pi}{4})+i\sin(\frac{3\pi}{4})\sqrt[4]{5} = \frac{-\sqrt{2}}{2}\sqrt[4]{5}-i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{5/4}(-1+i)$,
- $\a_3 = e^{5\pi i/4}\sqrt[4]{5} = \cos(\frac{5\pi}{4})+i\sin(\frac{5\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}+i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{5/4}(-1-i)$, and
- $\a_4 = e^{7\pi i/4}\sqrt[4]{5} = \cos(\frac{7\pi}{4})+i\sin(\frac{7\pi}{4})\sqrt[4]{5} = \frac{\sqrt{2}}{2}\sqrt[4]{5}-i\frac{\sqrt{2}}{2}\sqrt[4]{5}=\sqrt[4]{5/4}(1-i)$.
Note that by Eisenstein's Criterion using $p=5$ we see that $x^4+5$ is irreducible in $\Q$. As $\Q$ has characteristic 0, we see that $x^4+5$ is separable as well. 

As $E$ is the splitting field of an irreducible polynomial in $F[x]$, by Theorem 2.90 we see that $|\Aut(E/\Q)|=[E:\Q]=8$. In the Gaussian integers, it is known that if both $a$ and $b$ are nonzero then, $a+bi$ is a Gaussian prime if and only if $a^2+b^2$ is an ordinary prime. Note that $5=(2-i)(2+i)$, and that $2^2+i^2=3$, which is prime. Thus $2+i$ is prime in $\Z[i]$. Thus we may invoke Eisenstein's Criterion using $p=2+i$ to see that $x^4+5$ is irreducible in $\Q(i)$, as $(2+i)^2=3-2i$ does not divide 5, but we'll prove it just to be sure.

Suppose $(3+2i)|5$. Then $(3+2i)(a+bi)=5$, so $3a+3bi+2ai-2b=5$, and thus $3a-2b+(2a+3b)i=5$. As 5 has no imaginary component, it must be the case that $2a+3b=0$, and thus that $a=-\frac{3}{2}b$. Substituting in, we see that $-\frac{9}{2}b-3b=5$, and thus that $b=-\frac{10}{3}$, which has historically not been an integer.

Anyway, we may thus apply Porism 2.61 to see that there exists some $\tau\in\Aut(E/\Q(i))$ such that $\tau(\alpha_1)=\alpha_2$. We may regard $\tau$ as an element of $\Aut(E/\Q)$ since, by definition, $\Aut(E/\Q(i))$ is a subgroup of $\Aut(E/\Q)$.

As $\tau(\alpha_1)=\alpha_2$, observe the following glory:
$$\begin{align}
    \tau(\alpha_1)&=\alpha_2\\
    \tau(\sqrt[4]{5/4}(1+i))&=\sqrt[4]{5/4}(-1+i)\\
    \tau(\sqrt[4]{5/4})\tau(1+i)&=\sqrt[4]{5/4}(-1+i)\\
    \tau(\sqrt[4]{5/4})(1+i)&=\sqrt[4]{5/4}(-1+i)\\
    \tau(\sqrt[4]{5/4})&=\frac{\sqrt[4]{5/4}(-1+i)}{(1+i)}\\
    \tau(\sqrt[4]{5/4})&=\frac{\sqrt[4]{5/4}(-1+i)}{(1+i)}\frac{(1-i)}{(1-i)}\\
    \tau(\sqrt[4]{5/4})&=\frac{\sqrt[4]{5/4}(2i)}{2}\\
    \tau(\sqrt[4]{5/4})&=\sqrt[4]{5/4}i
\end{align}$$
With that in mind, we examine 
$$\begin{align}
    \tau(\alpha_2)&=\tau(\sqrt[4]{5/4}(-1+i))\\
    &=\tau(\sqrt[4]{5/4})\tau(-1+i)\\
    &=\tau(\sqrt[4]{5/4})(-1+i)\\
    &=\sqrt[4]{5/4}i(-1+i)\\
    &=\sqrt[4]{5/4}(-1-i)\\
    &=\alpha_3,
\end{align}$$
and
$$\begin{align}
    \tau(\alpha_3)&=\tau(\sqrt[4]{5/4}(-1-i))\\
    &=\tau(\sqrt[4]{5/4})\tau(-1-i)\\
    &=\tau(\sqrt[4]{5/4})(-1-i)\\
    &=\sqrt[4]{5/4}i(-1-i)\\
    &=\sqrt[4]{5/4}(1-i)\\
    &=\alpha_4,
\end{align}$$
and don't forget
$$\begin{align}
    \tau(\alpha_4)&=\tau(\sqrt[4]{5/4}(1-i))\\
    &=\tau(\sqrt[4]{5/4})\tau(1-i)\\
    &=\tau(\sqrt[4]{5/4})(1-i)\\
    &=\sqrt[4]{5/4}i(1-i)\\
    &=\sqrt[4]{5/4}(1+i)\\
    &=\alpha_1,
\end{align}$$
So $\tau$ corresponds to the permutation (1 2 3 4). We have proven that $\Aut(E/\Q(i))$ is isomorphic to a subgroup of $S_4$ having order at most 8 and that it contains an element or order 2 and (1 2 3 4), an element of order 4. Since the subgroup generated by these two elements has order 8, we see that $\Aut(E/\Q) \cong D_8$. (Also by Sylow's Theorem, $S_4$ only has one subgroup of order 8, and it is $D_8$).
***
### Midterm Problems
#### Problem – May 2018 (5)
Let $R$ be a commutative ring and let $M$ be an $R$-module. Show that if $M \ne 0$ and the only submodules of  $M$ are $0$ and $M$, then there is a maximal ideal $I$ of $R$ such that $M$ is isomorphic to $R/I$ as an $R$-module.

#### Problem 
Let $R$ be a commutative integral domain and $M$ an $R$-module. A subset $S$ of $M$ is called a *maximal linearly independent* subset of $M$ if $S$ is linearly independent and any subset of $M$ properly containing $S$ is linearly dependent.
1. Let $T$ be a linearly independent subset of $M$. Prove that $T$ is contained in some maximal linearly independent subset of $M$.
2. Let $T$ be a linearly independent subset of $M$ and let $N$ be the $R$-submodule of $M$ generated by $T$. Prove that $T$ is a maximal linearly independent subset if and only if $M/N$ is torsion. (Recall that an $R$-module $P$ is called "torsion'' if for each $p \in P$, there is a $r \in R$ such that $r \ne 0$ and $rp = 0$.)
#### Problem 
Let $R$ be a non-zero commutative ring and suppose $p: R^m \to R^n$ is a surjective homomorphism of $R$-modules for some non-negative integers $m$ and $n$. 
1. Prove that if $R$ is a field, then $m \geq n$.
2. Prove that if $R$ is any non-zero commutative ring, then $m \geq n$. 
#### Problem – June 2010 (5)

#### Problem 
Suppose $A \in \Mat_{n \times n}(F)$ where $F$ is a field and $A^k = 0$ for some integer $k \geq 1$.
Prove $A^n = 0$. {\em Tip}: Note that for any $m \geq 1$, $\im(T_A^{m+1}) \subseteq \im(T_A^{m})$. Show that if equality holds then $A^m = 0$. 
#### Problem 
Let $A = \begin{bmatrix} 2 & 0 & 0 & 0 \\ 0 & 6 & 0 & 0 \\ 0 & 0 & 20 & 0 \end{bmatrix}$
and $B = \begin{bmatrix} 2 & 0 & 0  \\ 0 & 6 & 0  \\ 0 & 0 & 20 \\ 0 & 0 & 0  \end{bmatrix}$, regarded as matrices
with entries in $\Z$. 
1. Express the cokernel of $A$ (i.e., $\Z^3/\im(t_A)$) in elementary divisor form (that is, as a direct sum of cyclic groups each of which is either infinite or of prime power order).
2. Express the cokernel of $B$ in elementary divisor form.

#### Problem 
Recall that a $\Z$-module $M$ is called torsion-free if the only element $m \in M$ such that $r \cdot m = 0$for some non-zero integer $r$ is the element $m = 0$. Let $M = coker(T_A)$ where $T_A: \Z \to \Z^2$ is the homomorphism $T_A(v) = Av$ for the matrix $A  = \begin{bmatrix} 7 \\ 11 \\ \end{bmatrix}$. Prove $M$ is torsion-free.
#### Problem – January 2016 (9)
Let $I$ be an ideal in a commutative ring $R$, let $M$ and $N$ be $R$-modules and let $f : M \to N$ be an $R$-module homomorphism.
1. Prove there is a unique $R$-module homomorphism $\overline{f} : M/IM\to N/IN$ such that $\overline{f} \circ p = q \circ f$, where $p : M \to M/IM$ and $q : N \to N/IN$ are the canonical quotient maps. (Recall $IM$ is the submodule of $M$ generated by elements of the form $am$ for $a \in I$ and $m \in M$.)
2. Prove that if $I^2 = 0$ and $\overline{f}$ is surjective, then so is $f$. (Recall that $I^2$ is the ideal generated by all elements of the form $ab$, where $a, b\in I$ .)

#### Problem 
Let $V$ be a finite dimensional vector space over a field $F$ and $f: V \to V$ an $F$-linear transformation. Prove the following assertions.
1. There exists an integer $s \geq 0$ such that for $n \geq s$ there are equalities $\ker(f^n) = \ker(f^s)$ and $\im(f^n) = \im(f^s)$. (Here $f^m$ denotes $f$ composed with itself $m$ times.) 
2. $\ker(f^s) \cap \im(f^s) = \{0\}$ for any $s$ as above.
3. $V = \ker(f^s) \oplus \im(f^s)$ for any s as above. (Recall $V = U \oplus W$ for subspaces $U$ and $W$ if $U + W = V$ and $U\cap W = \{0\}$. )

#### Problem 
Let $F$ be a field, $V$ an $F$-vector space, and $W$ a subspace of $V$. A subspace $U$ of $V$ is called a {\em complement} of $W$  in $V$ if $U \cap W = \{0\}$ and $U + W = V$. 
1. Prove that for every $V$ and $W$ as above, $W$ has at least one complement in $V$.
2. Prove that if $U$ is a complement of $W$ in $V$ and $V$ is finite dimensional, then $\dim_F(V)=\dim_F(W)+\dim_F(U)$.
3. Prove that if $T$ is a subspace of $V$ with $V$ finite dimensional and $\dim_F(T) + \dim_F(W)  > \dim_F(V)$, then $T \cap W$ is non-zero.

#### Problem 
Let $V$ be the set of all $r \times s$ matrices over a field $F$, let $G$ denote the group $GL_r(F) \times GL_s(F)$ (where, recall, $GL_m(F)$ is the group of $m \times m$ invertible matrices with entries in $F$) and set $(A,B)\cdot M=AMB^{-1}$ for all $M \in V$ and $(A,B) \in G$.
1. Prove that the formula above defines a group action.
2. Prove that each orbit contains a matrix $M = (m_{i,j})$ such that $m_{i,j}  = 0$ for all $i \ne j$ and $m_{i,i} \in \{0,1\}$ for all $i$
3. How many orbits are there?

#### Problem 
Let $R$ be a Euclidean domain, $A$ an $m \times n$ matrix with elements from $R$, and $A^T$ the transpose matrix of $A$. Let $\coker(A)$ denote the quotient of $R^m$ by the submodule generated by the columns of $A$. The {\em torsion} submodule of an $R$-module $M$ is the submodule $$\{m \in M \mid rm = 0 \text{ for some $r \ne 0$}\}.$$ (It is indeed a submodule and you need not prove this.) 
1. Prove that the torsion submodules of $\coker(A)$ and $\coker(A^T)$ are isomorphic.
2. Prove that the modules $\coker(A)$ and $\coker(A^T)$ are isomorphic if and only if $m = n$.

### Final Problems
#### Problem – June 2010 (9)
![[June 2010#Problem 9]]
***
#### Problem – June 2010 (4)
![[June 2010#Problem 4]]

***
#### Problem 
Let $L$ be the splitting field over $\Q$ of the polynomial $x^3 - 7$.
(a) Find all intermediate fields $E$ with $\Q \subseteq E \subseteq L$ (including possibly $L$ and $\Q$) such that $E$ is Galois over $\Q$.
(b) For each field $E$ you found in (a), find with justification a primitive generator (i.e., find $\alpha \in E$ so that $E = \Q(\alpha)$).

##### *Proof.*
###### Part (a) 
Invoking Eisenstein's Criterion and setting $p=7$ we see that $x^3 - 7$ is an irreducible cubic with exactly one real root. Thus $\Gal(L/\Q)\cong S_3$. Thus the subgroups of $\Gal(L/\Q)$ are as follows: $H_1\cong\langle(12)\rangle, H_2\cong\langle(13)\rangle, H_3\cong\langle(23)\rangle,$ and $H_4\cong\langle(123)\rangle.$ By the Fundamental Theorem of Galois Theory there exist four intermediate field extensions: $E_1=L^{H_1}, E_2=L^{H_2}, E_3=L^{H_3}$, and $E_4=L^{H_4}$. Note that as $H_1,H_2,$ and $H_3$ are all Sylow-2 subgroups of $S_3$, by [[Results#Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]] none are normal in $S_3$. However, as $[G:H_4]=2$, the smallest prime dividing 6, we see that $E_4$ is the only strictly intermediate field that is Galois over $\Q$. 

As the identity map is the only automorphism from $\Q\to\Q$ that fixes $\Q$ and $[\Q:\Q]=1$, we see that $\Q$ is Galois over itself. As all finite extensions of fields with characteristic 0 are separable, we see that $L$ is also Galois over $\Q$. Thus $\Q, L,$ and $E_4$ are the only intermediate fields $\Q \subseteq E \subseteq L$ that are Galois over $\Q$. 
***
###### Part (b)
Observe that $\Q(1)=\Q$, and as $\Q=\Q$ we see that 1 is a primitive element of $\Q$.

Next, note that As $i$ is a root of $x^2+1$, by the Degree Formula we have $[L:\Q(i)]=3$. As $E_4$ is the only extension with degree 3, we see that $E_4=\Q(i)$. Thus $i$ is a primitive element of $E_4$. 

Finally, let $\alpha=\sqrt[3]{7}i\in L$. Consider $$-7\alpha^{-2}=-7\left(\frac{1}{\sqrt[3]{7}}^2\right)=-7\left(\frac{\sqrt[3]{7}}{-7}\right)=\sqrt[3]{7}$$ and $$7\sqrt[3]{7}^{-3}=7\left(\frac{1}{-7i}\right)=7\left(\frac{i}{7}\right)=i.$$ Thus $L=\Q(\sqrt[3]{7}i)$. 
***
#### Problem – May 2019 (9)
Consider $f(x) = x^5 - 20x - 2 \in \Q[x]$. This polynomial has exactly three real roots, a fact that you may use without proof.
1. Show that $f$ is irreducible in $\Q[x]$.
2. Let $L$ be a splitting field of $f$ over $\Q$. Find the isomorphism class of the Galois group $\Gal(L/\Q)$.

##### *Proof.*
###### Part (a) 
Notice that $p=2$ is prime in $\Q[x]$, and thus $f(x)$ is irreducible in $\Q[x]$ by Eisenstein's Criterion.
***
###### Part (b) 
Because there are exactly two complex roots, the element of the Galois group given by complex conjugation corresponds to a transposition. Let $\alpha$ be a real root of $f(x)$. As $f$ is irreducible this root is not in $\Q$. As $\alpha$ is the root of a monic irreducible polynomial, we see that $[\Q(\alpha):\Q]=5$. As $\Gal(L/\Q)$ is isomorphic to a subgroup of $S_5$ and because there exists an extension of order 5, there must exist an element of $\Gal(L/\Q)$ of order 5. Thus we have a 5-cycle and a 2-cycle, from which we can generate all of $S_5.$. Thus $\Gal(L/\Q)\cong S_5$. 
***
#### Problem 
Suppose $F \subseteq K$ is a finite extension of fields such that $[K: F]$ is odd. Show that for any $b \in K$ we have $F(b) = F(b^2)$.

##### *Proof.*
Let $F \subseteq K$ be a finite extension of fields such that $[K: F]$ is odd, and let $b\in K$. 

Notice that $F(b^2)\subseteq F(b)$ , as $b^2$ can be expressed in terms of $b$ (exercise left to the reader). Suppose by way of contradiction that $b\not\in F(b^2)$. Then the polynomial $x^2-b^2$ has no roots in $F(b^2)$, making it irreducible in $F(b^2)$. As it is monic and irreducible, $x^2-b^2$ is the minimum polynomial of $b$ in $F(b^2)$, and thus $[F(b):F(b^2)]=2$. But then by the Degree Formula we have $$[K:F]=[K:F(b)][F(b):F(b^2)][F(b^2):F]=2[K:F(b)][F(b^2):F],$$ contradicting the fact that $[K: F]$ is odd. Thus $b\in F(b^2)$, and hence $F(b) = F(b^2)$.
***
#### Problem 
Find, with justification, a complete and non-redundant list of conjugacy class representatives for the group $\GL_3(\bF_2)$, where $\bF_2$ is the field with two elements.

##### *Proof.*
Let $\bF_2$ denote the field with two elements, and consider the group $\GL_3(\bF_2)$. 

Recall that matrices are in the same conjugacy class if and only if they are similar, and that two matrices are similar if and only if they share the same invariant factors. 

Let $A\in\GL_3(\bF_2)$. All characteristic polynomials are monic, and as $A$ is invertible we see the $a_0$  term in the $\cp_A(x)\neq0$, and thus $a_0=1$, the only other element in $\bF_2$. There are only so many monic polynomials with coefficients in $\bF_2$; hence there are only four possible characteristic polynomials of $A$:
1. $f(x)=x^3+x^2+x+1$, 
2. $g(x)=x^3+x^2+1$, 
3. $h(x)=x^3+x+1,$ and 
4. $j(x)=x^3+1$.
Note that since $a_0=1$, 0 cannot be a root of any of these polynomials. Thus all that remains is to check $1$. Luckily, $1$ is not a root of $g(x)$ or $h(x)$, so the only invariant factor of each is themselves. While 1 is a root of $j(x)$, we see that $j(x)=(x+1)(x^2+x+1)$. As $(x+1)\not|(x^2+x+1)$, neither of these polynomials can be invariant factors by the [[Results#Theorem – Rational Canonical Form|RCF Theorem]]; thus the only invariant factor of $j(x)$ is itself. However $f(x)=(x+1)^3$, and so its possible invariant factors are 
- $(x+1)^3$;
- $(x+1),(x+1)^2;$ and 
- $(x+1),(x+1),(x+1)$.
Let $k(x)=(x+1)^2$ and $\ell(x)=x+1$. Thus the conjugacy class representatives for $\GL_3(\bF_2)$ are 
1. $C(f)$, 
2. $C(\ell)\oplus C(k)$, 
3. $C(\ell)\oplus C(\ell)\oplus C(\ell)$,
4. $C(g)$, 
5. $C(h)$, and 
6. $C(j)$. 
***
#### Problem – January 2019 (6)
Determine, with justification, all similarity classes of matrices with entries in $\Q$ with characteristic polynomial $(x^4- 1)(x^2 -1)$. Provide an explicit representative for each of these similarity classes.

##### *Proof.*
Let $A$ be a matrix with entries in $\Q$ with characteristic polynomial $(x^4- 1)(x^2 -1)$.

By this [[Results#Corollary – Every Matrix Similar to Unique RCF Matrix|Corollary]] we know that every matrix is similar to a unique matrix in RCF. Note that RCF is based on the invariant factors if a matrix, and thus if two matrices have the same invariant factors they will have the same RCF, making them both similar to the same (unique) matrix, making them similar to each other. By part (1) of this [[Results#Theorem – Cayley-Hamilton Theorem|Theorem]], the characteristic polynomial of a matrix is equal to the product of the invariant factors of that same matrix. 

Recall that the invariant factors must divide all preceding invariant factors in RCF (See: [[Results#Theorem – Rational Canonical Form|Theorem]]), and observe that $(x^4-1)$ factors as $(x^2-1)(x^2+1)$ and $(x^2-1)$ factors as $(x-1)(x+1)$. Given this information, after some fiddling with the factors, we find four possible options for invariant factors of $A$:
1. $x^6-x^4-x^2+1=(x^2 -1)(x^4- 1)$,
2. $(x^2-1),(x^4-1)$,
3. $(x+1), (x-1)(x^4-1)$, and 
4. $(x-1),(x+1)(x^4-1)$.
Let $f(x)=x^6-x^4-x^2+1, g(x)=(x^4-1),$ $h(x)=x^2-1$, $j(x)=(x-1),$ and $k(x)=(x+1)$.
Observe the companion matrices of each of these polynomials:
$$C(f)=\begin{bmatrix}
0 & 0 & 0 & 0 & 0 & -1\\
1 & 0 & 0 & 0 & 0 & 0\\
0 & 1 & 0 & 0 & 0 & 1\\
0 & 0 & 1 & 0 & 0 & 0\\
0 & 0 & 0 & 1 & 0 & 1\\
0 & 0 & 0 & 0 & 1 & 0\\
\end{bmatrix},
C(g)=\begin{bmatrix}
0 & 0 & 0 & 1\\
1 & 0 & 0 & 0\\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix},
C(h)=\begin{bmatrix}
0 & 1\\
1 & 0\\
\end{bmatrix},
C(j)=\begin{bmatrix}
1\\ 
\end{bmatrix}\textrm{ and } 
C(k)=\begin{bmatrix}
-1\\ 
\end{bmatrix}
$$
Behold: explicit representatives of each similarity class:
1. $C(f)$,
2. $C(g)\oplus C(h)$,
3. $C(k)\oplus C(gj)$, and
4. $C(j)\oplus C(gk)$.
***
#### Problem 
Let $F$ be a field and recall that a square matrix $A$ with entries in $F$ is called nilpotent if $A^m = 0$ for some positive integer $m$.

(a) Assume $n \leq 3$ and prove that two $n \times n$ nilpotent matrices are similar if and only if they have the same rank. (Recall the rank of a matrix is the dimension of the vector space spanned by its columns.)
(b) Give an example, with justification, of two $4 \times 4$ nilpotent matrices that have the same rank but are not similar.

##### *Proof.*
Let $F$ be a field and recall that a square matrix $A$ with entries in $F$ is called nilpotent if $A^m = 0$ for some positive integer $m$.

###### Part (a) 
Assume $n \leq 3$ and let $A,B$ be nilpotent matrices with entries in $F$.
$(\Rightarrow)$ Suppose $A\sim B$. Thus there exists some invertible matrix $P$ such that $PAP\inv=B$ by the definition of [[Definitions#Similar Matrices|similar matrices]]. Let $U\in\ker(PA)$. Thus $PA(U)=0$ and $P(AU)=0$. We multiply both sides by $P\inv$ to see that $AU=0$. Therefore the $\ker(PA)=\ker(A)$, and hence the ranks of $PA$ and $A$ are equal by the [[Results#Corollary – Rank Nullity Theorem|Rank-Nullity Theorem]]. 

Next, observe 
$$\begin{align}
    \rank(AP\inv)&=\rank((AP\inv)^T)\\
    &=\rank(P^{-1^T}A^T)\\
    &=\rank(A^T)\\
    &=\rank(A),
\end{align}$$
as $(P^{-1})^T$ is an invertible matrix. Thus $\rank(B)=\rank(PAP\inv)=\rank(A)$.

$(\Leftarrow)$ Suppose that $\rank(A)=\rank(B)$. Let $\lambda$ be some eigenvalue of $A$. Thus there exists some matrix $U$ such that $A\lambda=\lambda U$ by Problem 6 on Homework 5. Let's consider this the base-case of some rather banal induction. Now assume that for $n$ we have $A^nU=\lambda^nU$. Consider $A^{n+1}U=A(A^nU)=A(\lambda^n U)=\lambda^n(AU)=\lambda^{n+1}U$. 

Recall that as $A$ is nilpotent, there exists some $m\in\N$ such that $A^m=0$. As $\lambda$ is an eigenvalue of $A$, by the above induction we see that $\lambda^m$ is an eigenvalue for $A^m=0$. As $F$ is a field and thus an integral domain, we see that $\lambda^n=0$ implies that $\lambda=0$ as well. 

A similar argument shows that all eigenvalues of $B$ as well as $A$ are in fact 0. As this holds in the algebraic closure of $F$ as well, we see that when factored into linear terms all the $\lambda=0$. Thus $\cp_A(x)=\cp_B(x)=x^n$. 

As $\cp_A(x)=\cp_B(x)$ and scalar matrices are not nilpotent, if $n=1$ or $2$ we see that $A\sim B$ by Problem 4 on Homework 5. Thus we only need to consider the case where $\cp_A(x)=\cp_B(x)=x^3$.

The only possible invariant factors involving $x^3$ are 
1. $x,x,x$;
2. $x,x^2$; and 
3. $x^3$ itself.
However, if $x,x,x$ are the invariant factors then the rank of $A$ would be 3, making it invertible, contradicting the fact that 0 is an eigenvalue of $A$. Thus we need only consider the latter two cases.

Note that $$C(x)=[0], C(x^2)=
\begin{bmatrix}
0 & 0\\
1 & 0\\
\end{bmatrix}, 
C(x)\oplus C(x^2)\begin{bmatrix}
0 & 0 & 0\\
0 & 0 & 0\\
0 & 1 & 0\\
\end{bmatrix}, \textrm{ and } C(x^3)=
\begin{bmatrix}
0 & 0 & 0\\
1 & 0 & 0\\
0 & 1 & 0\\
\end{bmatrix}.$$
As $C(x)\oplus C(x^2)$ has rank 1 and $C(x^3)$ has rank 2, since $\rank(A)=\rank(B)$ we see that they must have the same invariant factors, making them similar. 
***
###### Part (b) 
Consider $A=C(x^2)\oplus C(x^2)$ and $B=C(x)\oplus C(x^3)$.

Thus 
$$A=\begin{bmatrix}
0 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix} \textrm{ and } 
B=\begin{bmatrix}
0 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix},$$

both of which have rank 2 and are in RCF. Thus they are not similar. 
***
#### Problem January 2012 (4)
Let $F$ be a field of characteristic $p > 0$, $a \in F$ , and  consider the polynomial $f(x)=x^p -x-a \in F[x]$.

(a) Prove that $f(x)$ is either irreducible over $F$ or it splits into distinct linear factors over $F$. (*Hint*: If $\alpha$ is a root of $f(x)$,  consider $\alpha + j$ for $j \in \Z/p$.)
(b) Suppose $f(x)$ is irreducible over $F$ and let $L$ be a splitting field of $f$ over $F$. Prove that the Galois group of $L$ over $F$ is cyclic.

##### *Proof.*
Let $F$ be a field of characteristic $p > 0$, $a \in F$ , and  consider the polynomial $f(x)=x^p -x-a \in F[x]$.
###### Part (a) 
Suppose $f$ has a root, $\alpha$, in $F$. Then $\alpha^p-\alpha-a=0$. Consider $\alpha+j$ for some $j\in\Z/p$, and observe $(\alpha+j)^p-(\alpha+j)-a$. By The Freshman's Dream, we have $\alpha^p+j^p-\alpha-j-a$, but as $\alpha^p-\alpha-a=0$, we really have $j^p-j$. By Fermat's Little Theorem, $p|j^p-j$, and thus $f(\alpha+j)=0$. Thus we have found $p$ roots of $f$, and thus $f$ splits into linear factors. 

Suppose then that no root of $f$ exists in $F$. Let $L$ be a splitting field of $f$ over $F$, and note that from the above paragraph we have $L=F(\alpha)$. As $f'(x)=1$, we see $\gcd(f,f')=1$, and thus $f$ is separable. Hence $F(\alpha)$ is a Galois extension. Thus there exists a $\sigma\in\Gal(L/F)$ such that $\sigma(\alpha)\neq\alpha$. So $\sigma(\alpha)=\alpha+j$ for some $j\in\Z/p$. Notice $\sigma(\alpha+j)=\sigma(\alpha)+j=\alpha+2j$. As $p$ is prime, we see that $|j|=p$, and thus we need to apply $\sigma$ to $\alpha$ $p$ times in order to get back to $\alpha$. Thus $\sigma(\alpha)^p=\alpha$, so $|\sigma|=p$. Thus $|\Gal(L/F)|=p$. Thus the minimum polynomial of $\alpha$ must have degree $p$. As $\alpha$ is a root of $f$ and $f$ is monic, it must be the minimal polynomial and is thus irreducible.
***
###### Part (b) 
Suppose $f(x)$ is irreducible over $F$ and let $L$ be a splitting field of $f$ over $F$. Let $\alpha$ be a root of $f.$ Consider $F(\alpha)$. By part (a), $F(\alpha)$ contains all the roots of $f$, hence $L=F(\alpha)$. As $f$ is monic and irreducible, it is the minimum polynomial of $f$, and thus $[L:F]=p$. Hence $|\Gal(L/F)|=p$. All groups of prime order are cyclic, completing the proof.
***
#### Problem 
Let $p$ be any positive prime integer.
(a) Prove that if $p = k^2 + 1$ for some integer $k$, then $p$ is not an irreducible element of $\Z[i]$.
(b) Prove $x^4 - p$ is irreducible in $\Q(i)[x]$. {\em Tip:} Find the degree of the splitting field of $x^4 - p$ over $\Q(i)$.  

##### *Proof.*
Let $p$ be any positive prime integer.
###### Part (a) 
Suppose $p = k^2 + 1$ for some integer $k$.  As $(k-i)(k+i)=p$, $p$ is not an irreducible element of $\Z[i]$.
***
###### Part (b) 
As $x^4-p$ is irreducible in $Q$ (Eisenstein, $p=p$) and $x^4-p$ is monic, we see that $[\Q(\sqrt[4]{p}):\Q]=4$. As $x^2+1$ is irreducible and monic, we see that $[\Q(\sqrt[4]{p},i):\Q(\sqrt[4]{p})]=2$. By the Degree Formula we have $[\Q(\sqrt[4]{p},i):\Q]=8$. Note that the four roots of $(x^4 - p)$ are -
- $\sqrt[4]{p}$, 
- $-\sqrt[4]{p}$,
- $\sqrt[4]{p}i,$ and 
- $-\sqrt[4]{p}i$.
As $\sqrt[4]{p}i/\sqrt[4]{p}=i$, we see that $\Q(\sqrt[4]{p}$ is the splitting field of $F$. Note then that as $[\Q(i):\Q]=2$ and the degree of the splitting field is 8, by the Degree Formula we see that the degree of the splitting field of $x^4-p$ over $\Q(i)=4$. As $x^4-p$ is monic and degree $4$, it must be the minimal polynomial of the second extension and thus irreducible in $\Q(i)[x]$. 
***
#### Problem – January 2017 (4)
Let $F \subseteq L$ be a finite Galois field extension of degree $45$. Prove there exists a unique intermediate field $E$ (i.e., $F \subseteq E \subseteq  L$) such that $[E : F] = 5$.

##### *Proof.*
Let $F \subseteq L$ be a finite Galois field extension of degree $45$. 

Note that as $45=5\cdot 9$, we see that the number of Sylow-$5$ subgroups of $G$ divides $9$ and is congruent to $1\mod{5}$. Thus there is exactly one Sylow-$5$ subgroup of $G$, which we denote $H$. By the Fundamental Theorem of Galois Theory, $H$ corresponds to an intermediate field extension $E$. Note that as $H$ has order 5, we see that $[G:H]=9$, and thus $[L:E]=9$ as well. By the Degree Formula we see that $[L:F]=[L:E][E:F]$. As $[L:F]=45$ and $[L:E]=9$, we see that $[E:F]=5$, as desired. As $E$ corresponds to the unique subgroup of $G$ or order 5, we see that this extension must be unique as well.
***
#### Problem 
For the matrix
$$A  = \begin{bmatrix} 0 & -1 & 2 \\ 1 & 0 & 0 \\ 0 & 1 & -2 \\ \end{bmatrix}$$
(a) Find the rational canonical form of $A$.
(b) Determine whether or not $A$ has a Jordan canonical form, and if so, find this form.

###### *Proof.*
###### Part (a) 
Note that by taking the determinant of $xI-A$ we see that $\cp_A(x)=x^3+2x^2+x$. This factors as $x(x+1)^2$, so this is the only invariant factor. Thus RCF is the companion matrix of $\cp_A(x)$, 
$$C(\cp_A(x))=\begin{bmatrix} 0 & 0 & 0 \\ 1 & 0 & -1 \\ 0 & 1 & -2 \\ \end{bmatrix}$$
***
###### Part (b) 
The elementary divisors of $A$ are $(x)$ and $(x+1)^2$. As $J_1(0)=[0]$ and $J_2(-1)=\begin{bmatrix} -1 & 0\\ 1 & -1\\ \end{bmatrix}$,  the JCF of $A$ is $J_1(0)\oplus J_2(-1)$. 
***
## Fall 2021
### Homework 1
#### Problem – Groups of Order $4$ Abelian
Prove that every group of order $4$ is abelian. Your proof should only use the definition of a group. 

##### *Proof.*
Let $G$ be a group with $4$ elements, and suppose there are elements $a,b\in G$  
such that $ab\neq ba$ for some elements $a, b\in G$. Since $ab \neq ba$, we must have $a \neq b$,  
$a \neq e$, and $b\neq e$. Since $G$ has only $4$ elements and $ab \neq ba$, either $ab \in \{e, a, b\}$ or $ba \in\{e, a, b\}$. Without loss, say the former occurs. But $ab = e$ implies $b=a\inv$ and we know $a\inv$ commutes with $a$, and hence this is not possible. If $ab = a$, then $b = e$ and if $ab = b$ then $a = 1$, both of which are impossible. Since a, b were arbitrary, G must be abelian.
***
#### Problem 
Let $G$ be a group and $x \in G$ any element. 
Recall that $|x|$ denotes the {\em order} of $x$, defined to be the least integer $n \geq 1$ such that $x^n = 1$; if no such integer exists, we say $|x| =\infty$. Also, let $\#G$ denote the cardinality of $G$, which is an element of $\{1, 2, 3, \cdots \} \cup \{\infty\}$.
1. Prove that if $|x| = n$, then $e, x, \dots, x^{n-1}$ are all distinct elements of $G$. 
2. Prove that if $|x| = \infty$, then $x^i \ne x^j$ for all integers (positive or negative) $,j$ with $i \ne j$. 
3. Conclude $|x| \leq |G|$ in all cases.

#### Problem 
A subset $S$ of a group $G$ is said to {\em generate $G$} if every element of $G$ is equal to a product of elements of $S$ and their inverses (with repetitions allowed).
(a) Prove that $D_{2n}$ is generated by $r$ and any reflection.
(b) Prove that if $p\ge 3$ is prime then $D_{2p}$ is generated by any two distinct reflections.

##### *Proof.*
***
#### Problem – Cyclic Groups are Abelian
Prove that any cyclic group is abelian. Give an example of an abelian group which is not cyclic, with justification.

##### *Proof.*
Let $G$ be a cyclic group and let $x,y\in G$. As $G$ is cyclic we see $x=g^n$ and $y=g^m$ for some $n,m\in\N$ and $g\in G$. Notice then $$xy=g^ng^m=g^{nm}=g^{mn}=g^mg^n=yx,$$ making $G$ abelian.

The group $\Z/2\times\Z/2$ is a group of order $4$, making it abelian (See:). However, every element has order $2$, and thus it cannot be cyclic. 
***
#### Problem
Prove that $(\mathbb Q, +)$ is not a cyclic group.

##### *Proof.*

***
#### Problem 
Prove that $\operatorname{GL}_2(\mathbb Z_2)$ is not cyclic.

##### *Proof.*
***
### Homework 2
#### Problem – Generating $S_n$
For $n\ge 2$ prove that $S_n$ is generated by $(12)$ and the $n$-cycle $(12\cdots n)$.

##### *Proof.*
Let $H = 〈(12),(12 ···n)〉$. Since every permutation can be written as a product of transpositions (See:[[Proposition – Disjoint Cycles & Transpositions|Proposition]]), it suffices to show that every transposition is in $H$. Note that $(ij) = (1i)(1j)(1i)$ for any $i\neq j$. Thus, it suffices to prove that every transposition of the form $(1i)$ is in $H$. Next note that for any $1 ≤i ≤n −2$,  
$$(12 ···n)(ii + 1)(12 ···n)−1 = (i + 1 i + 2).  $$
Since $(12) ∈ H$ we get by repeated application of this equation that $(ii + 1) ∈ H$ for  
all $1 ≤ i ≤ n −1$. As $(ii + 1)(1i)(ii + 1) = (1 i + 1)$ and $(12) ∈ H$, we obtain that $(1i) ∈H$ for $i ≤n$. This finishes the proof.
***
#### Problem 
For $n\ge 1$ let $\operatorname{SL}_n(\mathbb R)$ denote the set $\{A\in \operatorname{GL}_n(\mathbb R) \mid \det(A)=1\}$.  Prove that $\operatorname{SL}_n(\mathbb R)$, called the {\it special linear group} of degree $n$,  is a subgroup of $\operatorname{GL}_n(\mathbb R)$. 

##### *Proof.*
***
#### Problem – Unions of Subgroups
Let $G$ be a group and $H$, $H'$ subgroups.  Prove that $H\cup H'$ is a subgroup if and only if $H\subseteq H'$ or $H'\subseteq H$.

##### *Proof.*
First, note that if $H\subseteq H'$ or $H'\subseteq H$ then their union is just the larger set, which is a subgroup of $G$ by supposition. This completes the forward direction.

Suppose by way of contradiction that $H ∪H′$ is a subgroup but $H\not\subseteq H'$  
and $H'\not\subseteq H$. Choose $a \in H \setminus H'$ and $b \in H'\setminus H$. Then $a,b \in H \cup H'$, so by closure  
$ab \in H \cup H'$. But if $ab \in H$, then multiplying on the left by $a-1$ gives $b ∈ H$, a  
contradiction. A similar contradiction holds if $ab\in H'$.
***
#### Problem – Centralizer is a Subgroup
Let $G$ be a group and $a\in G$.  Let $C_G(a):=\{x\in G\mid xa=ax\}$.  Prove that $C_G(a)$, called the {\it centralizer} of $a$ in $G$, is a subgroup of $G$.

##### *Proof.*
As $1 ∈C_G(a)$, $C_G(a)$ is nonempty. Let $x,y ∈C_G(a)$. Then $$(xy)a = x(ya) =  
x(ay) = (xa)y = (ax)y = a(xy).$$This shows that $xy ∈C_G(a).$ As $x ∈C_G(a)$, we have $xa = ax$. Multiplying on the left and right by $x−1$, we obtain $ax−1 = x−1a$. Thus, $x−1 ∈C_G(a)$, and $C_G(a)$ is a subgroup of $G$.
***
#### Problem – Automorphism Group is a Group
Let $G$ be a group. An isomorphism $\phi:G\to G$ is called an {\it automorphism} of $G$.   Prove that the set of automorphisms of $G$, denoted $\operatorname{Aut}(G)$, is a group under composition.

##### *Proof.*
***
#### Problem – Abelian Groups and Inverse Automorphism
Let $G$ be a group.  Prove that the map $f:G\to G$ given by $f(a)=a^{-1}$ for all $a\in G$ is an automorphism if and only if $G$ is abelian.  

##### *Proof.*
Suppose G is abelian. Then $$f(ab) = (ab)\inv = b\inv a\inv = a\inv b\inv = f(a)f(b)$$  
for all $a,b ∈ G$. Hence, $f$ is a homomorphism. Note that $$(f\circ f)(a) = f(f(a)) =  
f(a\inv) = (a\inv)\inv = a$$for all $a \in G$. Hence, $f\circ f = \id_G$, which means $f = f\inv$.  Hence, $f$ is bijective. Thus, $f$ is an automorphism of $G$. Conversely, suppose $f$ is an automorphism. Then for any $a,b \in G$ we have $$ab = (a−1)−1(b−1)−1 = f(a\inv)f(b\inv)=f(a\inv b\inv)=(a\inv b\inv)\inv=(b\inv)\inv(a\inv)\inv=ba.$$ Thus, G is abelian.
***
#### Problem – Conjugation Yields Automorphism
Let $G$ be a group and $x\in G$.  Define a map $\psi_x:G\to G$ by $\psi_x(a)=xax^{-1}$ for all $a\in G$.
(a) Prove that $\psi_x\in \operatorname{Aut}(G)$ for all $x\in G$. 
(b) Prove that $\{\psi_x\mid x\in G\}$ is a subgroup of $\operatorname{Aut}(G)$.
##### *Proof.*
Let $G$ be a group and $x\in G$.  Define a map $\psi_x:G\to G$ by $\psi_x(a)=xax^{-1}$ for all $a\in G$.

###### Part (a)
We first prove $ψx$ is a homomorphism: Let $a,b ∈ G$. Then $$ψ_x(ab) =  
x(ab)x\inv = (xax\inv)(xbx\inv) = ψ_x(a)ψ_x(b).$$To show $ψ_x$ is bijective, I will exhibit an inverse map for $ψ_x$ (which will be needed for the second part anyway). Below, we show $ψ_x ◦ψ_y = ψ_{xy}$ for all $x,y ∈ G$. From this, it follows that $ψ_x ◦ψ_{x\inv} = ψ_1 = \id_G$, and also $ψ_{x\inv} ◦ψ_x = \id_G$. Hence, $ψ_x$ has an inverse, namely $ψ_{x\inv}$, and is thus necessarily bijective. Thus, $ψ_x$ is an automorphism for every $x ∈G$.
***
###### Part (b)
Let $H = \{ψ_x | x \in G\}$. To show $H$ is a subgroup, note first that  
$H$ is nonempty since $ψ_1 ∈ H$. Now let $ψ_x,ψ_y ∈ H$. For any $a ∈ G$, note that  
$$(ψ_x ◦ψ_y)(a) = ψ_x(ψ_y(a)) = ψ_x(yay\inv) = x(yay\inv)x\inv = (xy)a(xy)\inv = ψ_{xy}(a). $$
Hence, $ψ_xψ_y = ψ_x ◦ψ_y = ψ_{xy} ∈H$. By the argument in part (1), we have for any  
$x ∈G, (ψx)\inv = ψ_{x\inv} ∈H$, so $H$ is closed under inverses. Thus, $H$ is a subgroup  
of $\Aut(G)$.
***
### Homework 3
#### Problem – Bijection of Left and Right Cosets
Let $G$ be a group and $H$ a subgroup of $G$.  Prove there is a bijection between the set of (distinct) left cosets of $H$ and the set of (distinct) right cosets of $H$.

##### *Proof.*
Let $X$ be the set of left cosets of $H$ and $Y$ the set of right cosets. Define  
$f : X → Y$ by $f(xH) = Hx\inv.$ We first need to show that this map is well-defined.  
Suppose $xH = yH$. Then $y\inv x ∈ H$, which implies $Hx\inv = Hy\inv$, so that $f(xH) = f(yH)$. Now $f$ is certainly surjective, as $f(x\inv H) = Hx$ for any $x ∈G$. Finally, to see that $f$ is injective, suppose $f(xH) = f(yH)$. Then $Hx\inv = Hy\inv$, which implies that $y\inv x ∈H$. As before, this implies that $xH = yH$. Hence, $f$ is a bijection.
***
#### Problem – Subgroups of Relatively Prime Order
Suppose $H$ and $K$ are subgroups of $G$ of relatively prime (hence, finite) order. Prove that $H\cap K=\{e\}$.

##### *Proof.*
Let $H$ and $K$ be subgroups of $G$ of relatively prime order. Let $x\in H\cap K$. By Lagrange's Theorem we see that $|x|\big||H|$ and $|x|\big||K|$, but as these orders are relatively prime, we have $|x|=1$, making $x=e$. Thus $H\cap K=\{e\}$.
***
#### Problem – Only Subgroup of Order Always Normal
Let $H$ be a [[Subgroup|subgroup]] and $x\in G$.  
(a) Prove that $xHx^{-1}$ is a subgroup of $G$.
(b) Prove that $H\cong xHx^{-1}$ (See: [[Isomorphism|Isomorphic]]).
(b) Suppose $|H|=n$ and $H$ is the only subgroup of $G$ of [[Order|order]] $n$. Prove that $H$ is [[Normal Subgroup|normal]].

##### *Proof.*
Let $H$ be a subgroup and $x\in G$.  

###### Part (a)
Let $ψ_x : G →G$ be the automorphism defined by $ψ_x(g) = xgx\inv$. (See: [[Mathematics/Modern Algebra/Results/Problems#Problem – Conjugation Yields Automorphism|Result]]) Then $ψ_x(H) = xHx\inv$. As the image of a subgroup under a homomorphism is a subgroup (See: Result), we can conclude that $xHx\inv$ is a subgroup of $G$.
***
###### Part (b) 
The map $ψ_x$ restricted to $H$ is the desired isomorphism.
***
###### Part (c)
Let $x ∈ G$. As $H\cong xHx\inv$, $|xHx\inv| = |H|$. Since $H$ is the unique subgroup of $G$ of order $n$, this implies $xHx\inv = H$. Hence, $H$ is normal.
***
#### Problem 
Let $H$ and $K$ be [[Normal Subgroup|normal]] [[Subgroup|subgroups]] of a [[Group|group]] $G$ such that $H\cap K=\{1\}$.  Prove that $xy=yx$ for all $x\in H, y\in K$.

##### *Proof.*
Let $x ∈H$ and $y ∈K$. As $H$ is normal, $k\inv hk ∈H$. Hence, $h\inv k\inv hk ∈H$.  Similarly, as $K$ is normal, $h\inv k\inv h ∈K$, so $h\inv k\inv hk ∈K$. Thus, $h\inv k\inv hk ∈H∩K = {1}$, so $hk = kh$.
***
#### Problem – Generated and Normal Subgroups
Let $G$ be a group and $S$ a subset of $G$.  Let $H=\langle S \rangle$.  Prove that $H\triangleleft G$ if and only if $gsg^{-1}\in H$ for every $s\in S$ and $g\in G$.

##### *Proof.*
As $H=\langle S \rangle$ we have $s\in H$ for every $s\in S$. Thus $gsg\inv\in H$, as $gHg\inv=H$ for all $g\in G$.

Suppose $gsg\inv ∈ H$ for all $s ∈ S$. Let $h ∈ H$ and $g ∈ G$. Then $h=s^{e_1}_1 s^{e_2}_2\dots s^{e_n}_n$ for some $s_1,...,s_n ∈S$ and $e_1,\dots,e_n\in\{\pm1\}$. Let $g ∈G$. Then  
$$ghg\inv = (gs^{e_1}_1g\inv)(gs^{e_2}_2g\inv) ···(gs^{e_n}_ng\inv).$$

Note that if $e_i = −1$ then $gs\inv_i g\inv = (gs_ig\inv)\inv ∈H$. Thus, $gs^{e_i}_i g\inv ∈H$ for all $i$, and hence $ghg\inv ∈H$. Therefore, $H\nsg G.$ 
***
#### Problem 
Let $G$ be a group, $S=\{aba^{-1}b^{-1}\mid a,b\in G\}$, and $H=\langle S \rangle$.  Prove that $H\triangleleft G$.

##### *Proof.*
Let $g ∈G$ and $s = aba\inv b\inv$. Note that $gsg\inv = xyx\inv y\inv ∈S ⊆H$, where $x = gag\inv$ and $y = gbg\inv$. Hence, $H \nsg G$ (See: [[Mathematics/Modern Algebra/Results/Problems#Problem – Generated and Normal Subgroups|Result]])
***
#### Problem – $G/Z(G)$ Cyclic
Let $G$ be a group and $Z=\operatorname{Z}(G)$.  Suppose $G/Z$ is cyclic.  Prove that $G$ is abelian.

##### *Proof.*
Let $G/Z = 〈xZ〉$ for some $x ∈ G$. Let $a,b ∈ G$. Then $aZ = x^iZ$ and $bZ = x^j Z$ for some $i,j$. Hence, $a = x^iz_1$ and $b = x^j z_2$ for some $z_1,z_2 ∈ G$. Then $$ba = (x^j z_2)(x^iz_1) = x^{j+i}z_1z_2 = (x^iz_1)(x^j z_2) = ab.$$Hence, G is abelian.
***
### Homework 4
#### Problem – Inner Automorphisms are Normal
Let $G$ be a group and $\operatorname{Aut}(G)$ be its automorphism group. In Problem 7 on HW \# 2, you proved that for each $g\in G$, the function $\psi_g:G\to G$ defined by $\psi_g(x)=gxg^{-1}$ for all $x\in G$ is an automorphism of $G$.  Further, you proved the set $\operatorname{Inn}(G):=\{\psi_g \mid g\in G\}$, called the set of *inner automorphisms* of $G$, is a subgroup of $\operatorname{Aut}(G)$. Prove that $\operatorname{Inn}(G)\triangleleft \operatorname{Aut}(G)$.

##### *Proof.*
Let $ψ_g ∈\Inn(G)$ and $φ ∈\Aut(G)$. We claim that $φψ_gφ\inv = ψ_{φ(g)} ∈\Inn(G)$.  
Let $x ∈ G$. Then $$φψ_gφ\inv(x) = φ(gφ\inv(x)g\inv) = φ(g)xφ(g)\inv = ψ_{φ(g)}(x).$$ This proves the claim. Hence, $\Inn(G)\nsg \Aut(G)$.
***
#### Problem 
Let $G$ be a group.  Prove that $\operatorname{Inn}(G)\cong G/\operatorname{Z}(G)$.

##### *Proof.*
Define $f : G → \Inn(G)$ by $f(g) = ψ_g$. Recall on HW #2 that when you  
proved $\Inn(G)$ is a subgroup, you proved that $ψ_gψ_h = ψ_{gh}$ for all $g,h ∈ G$. Hence,  $$f(gh) = ψ_{gh} = ψ_gψ_h = f(g)f(h),$$so f is a homomorphism. Each $ψ_g=f(g)$, making $f$ is surjective.  

Note that $g ∈ \Ker(f)$ if and only if $ψ_g = \id_G$, which is if and only if $gxg\inv = x$ for all $x ∈G$. This last condition is equivalent to saying $g\in Z(G)$. Thus, $\Ker(f) = Z(G)$. The result now follows from the First Isomorphism Theorem.
***
#### Problem – Element of Order 2 Sans Cauchy
Let $G$ be a finite group.  Prove that the number of elements in the set $S=\{g\in G\mid g\neq g^{-1}\}$ is even. Conclude that a group of even order must have an element of order $2$. (Do not use Cauchy's Theorem here, in case we have proved it before this homework is due.)

##### *Proof.*
Define an equivalence relation on $G$ by $a ∼b$ if and only if $a = b$ or $a = b\inv$. It is easily checked that this relation is an equivalence relation. Thus, the equivalence classes partition $G$. Note for $a ∈G$, the equivalence class of a has $1$ or $2$ elements, and has $2$ elements if and only if $a ∈ S$. Thus, each equivalence class of an element in $S$ has size $2$ (and the class is contained in $S$), so $|S|$ is even. We have $|G|= |S|+ n$ where $n$ is the number of elements a having equivalence class size $1$, i.e.. $a = a\inv.$ Since $|G|$ is even and $|S|$ is even, we must have $n$ is even also. Since $e = e\inv$, there must exist at least one other element a such that $a = a\inv$. This element has order $2$.
***
#### Problem – Groups of Order Six
Let $G$ be a group of order $6$.  Prove that either $G$ is cyclic or $G\cong S_3$.  (Hint:  By the previous problem, $G$ has a subgroup $H$ of order 2.  Consider the action of G on the left cosets of $H$.)

##### *Proof.*
Let $G$ act on the set of left cosets of $H$, where $H = 〈a〉$ is a subgroup of order $2$. As $[G : H] = 3$, there exists a homomorphism $φ : G →S_3$ whose kernel is the largest normal subgroup of $G$ contained in $H$. Thus, either $\Ker(φ) = {e}$  (i.e., φ is injective) or $\Ker(φ) = H$. If $φ$ is injective, then $φ$ must be an isomorphism since $|G|= |S_3|= 6$. If $\Ker(φ) = H$, then $H\nsg G$. As $|H|= 2$ and normal, $H ⊆Z(G)$. Hence, $G/Z(G)$ has order at most $3$, and is thus cyclic. By a previous exercise, this implies that $G$ is abelian. 

As $G/H$ has order $3$ (and is thus cyclic), there exists $b ∈G$ such that $bH$ has order $3$ in $G/H$. Let $n = |b|$. Since $bn = 1$, we also have $(bH)n = bnH = H$.  Hence, $3$ divides $n$. Since $|G| = 6$, $n$ divides $6$, so $n = 3$ or $n = 6$. 

If $n = 6$ then $G = 〈b〉$. Suppose $n = 3$. We claim $|ab|= 6$. Let $m = |ab|$. Certainly, $m ≤|G|= 6$. As $G$ is abelian, $ambm = (ab)m = e$, so $am = b−m ∈〈a〉∩〈b〉= {1}$, with the last equality following by Lagrange’s theorem, since $〈a〉$ and $〈b〉$ have relatively prime orders. Hence, $am = bm = e$. Thus, $|a|$ and $|b|$ both divide $m$, so $m≥6$. Thus, $G = 〈ab〉$ is cyclic.
***
#### Problem 
Let $H$ be a subgroup of a finite group $G$ and consider the set $X=\{xHx^{-1} \mid x\in G\}$.  Prove that $|X|=[G:N_G(H)]$ where $N_G(H)=\{g\in G\mid gHg^{-1}=H\}$.  $N_G(H)$ is called the {\it normalizer} of $H$ in $G$.

##### *Proof.*
Note that $G$ acts on $X$ by conjugation and that $X = \Orb(H)$. Note also  
that the stabilizer of $H$ under this action is precisely $N_G(H)$. The result now follows directly from the Orbit-Stabilizer theorem.
***
#### Problem 
Let $G$ be a finite group and $H$ a proper subgroup (i.e., $H\neq G$).  Prove that $$\bigcup_{x\in G} xHx^{-1}\neq G.$$
##### *Proof.*
Note that $|xHx\inv| = |H|$ for all $x ∈ G$. Also, by the previous problem,  
the number of distinct subgroups $xHx\inv$ is $[G : NG(H)]$. Let $n = [G : N_G(H)]$ and  
$x_iHx\inv_i$ for $i = 1,...,n$ the distinct conjugates of $H$. Note first that if $n = 1$ then  
$H \nsg G$ and result holds since $H \neq G$. So assume $n ≥2$. Since each conjugate contains $|H|−1$ non-identity elements, we have $$⋃_{x∈G}  xHx\inv|= |  n⋃_{i=1}  x_iHx\inv_i |≤1 +  n∑_{i=1}  (|H|\inv) = 1 + n|H|−n.$$ As $n = [G : NG(H)] ≤ [G : H]$ (as $H ⊆ N_G(H)$), we have $n|H|≤|[G : H]|H| = |G|$.  
Thus, as $n ≥2, 1 + n|H|−n ≤1 + |G|−n < |G|.$
***
#### Problem 
Suppose $G$ acts on a set $X$ and let $u,v\in X$.  Suppose $u$ and $v$ lie in the same orbit.  Prove that $G_u=gG_vg^{-1}$ for some $g\in G$. Conclude that if the action is transitive (i.e., there is precisely one orbit) then for any $u\in X$ the kernel of the action is $$\bigcap_{g\in G} gG_ug^{-1}.$$
##### *Proof.*
Suppose $u,v ∈X$ lie in the same orbit. Then $u = gv$ for some $g ∈G$. Then  
$a ∈ G_u$ if and only $au = u$, which is if and only if $agv = gv$, which is if and only if  
$(g\inv ag)v = v$, which is if and only $if g\inv ag ∈ Gv$, which is if and only if $a ∈ gGvg−1.$  

Thus, $G_u = gG_vg\inv$. Now, if $G$ acts transitively on $X$, then $X = \{gv |g ∈G\}$ for any  
$v ∈ X$. Hence, by the argument above, for any $u ∈ X, G_u = gG_vg\inv$ for some $g ∈ G$.  

Since the kernel of the action is the intersection of all the stabilizers, we obtain the  
desired conclusion.
***
#### Problem 
Suppose that $G$ is an abelian group acting transitively and faithfully on a set $X$.  Prove that $|G|=|X|$.

##### *Proof.*
Let $u ∈ X$. As the action is transitive, by the exercise above we have that the kernel of the action is the intersection of $gG_ug\inv$ over all $g ∈ G$. However, as $G$ is abelian, $gG_ug\inv = G_u$ for all $g ∈ G$. Hence, the kernel of the action is $G_u$ for any $u ∈ X$. On the other hand, the action is faithful, which means the kernel of the action is the identity. It follows that $G_u = \{e\}$ for every $u ∈ X$. Finally, as the action is transitive, $X = \Orb(u)$ for some (any) $u ∈X$. By the Orbit-Stabilizer theorem, $|X|= |\Orb(u)|= [G : G_u] = |G|$.
***
### Homework 5
#### Problem – Free Group Map Injective
Let $i:S\to F$ be a free group on $S$.  Prove that the map $i$ is injective. 

##### *Proof.*
Let $s,t ∈ S (s \neq t)$ and define $j : S → \Z_2$ by $j(s) = 0$ and $j(a) = 1$ for all $a ∈ S$, $a\neq s.$ (In particular, $j(t) = 1$.) Then there exists a homomorphism $f : F → \Z_2$ such that $f(i(a)) = j(a)$ for all $a ∈ S$. Hence, $f(i(s)) = j(s) = 0$ and $f(i(t)) = j(t) = 1$. As f is a well-defined function, we must have $i(s)\neq i(t)$. Hence, $i$  is injective.
***
#### Problem 
Let $i:S\to F$ be a free group on $S$, $H=\langle i(S) \rangle$, and $j:S\to H$ be the map $i$ restricted to the co-domain $H$. The universal property gives a group homomorphism $f:F\to H$ such that $fi=j.$ Let $\ell:H\to F$ be the inclusion map, which is obviously a group homomorphism, and that $\ell j=i$. As $fi=j$, we see that $\ell j=\ell fi=i$. Thus we can use the universal property again to obtain a homomorphism from $i$ to $i$ (which is the identity function $1_F$) such that $\ell f=1_F$. As $1_F$ is an isomorphism, we see that it is also surjective, meaning that $\ell$ is surjective and $f$ is injective. Thus $\ell$ is surjective, completing the proof. 

##### *Proof.*
Let $j, H, f$ and $\ell$ be given as in the Hint. Now, for $s ∈ S$, $\ell(f(i(s))) = \ell(j(s)) = i(s),$ as $fi = j$ and $\ell j = i.$ Hence, $\ell fi = i$. Thus, $\ell f : F → F$ is a group  
homomorphism such that $(\ell f)i = i.$ But the identity map $1_F$ also satisfies $1_F i = i$.  
By the uniqueness of the homomorphisms in the definition of free group, this means  
$\ell f = 1_F$. In particular, $\ell$ is surjective. Hence, the inclusion map $H →F$ is surjective, which implies $H = F$. Thus, $S$ generates $F$
***
#### Problem – Infinite Order in Free Groups
Let $i:S\to F$ be a free group. Prove that for every $s\in S$, the order of $i(s)$ is infinite.

##### *Proof.*
Suppose, by way of contradiction, that $|i(s)| = n$, where $n$ is a positive  
integer. Define $j : S →\Z$ by $j(a) = 1$ for every $a ∈S$. Then there exists a homomorphism $f : F →\Z$ such that $f(i(a)) = j(a) = 1$ for every $a ∈S$. As $|i(s)|= n$, we have $i(s)n = 1$. Then $$0 = f(i(s)n) = n ·f(i(s)) = n ·1 = n,$$ a contradiction.
***
#### Problem – Quaternion Presentation
Find with proof a presentation of $Q_8$.

##### *Proof.*
We claim that $〈x,y | x^4 = 1,x^2y^2 = 1,yxy^3x = 1〉$ is a presentation for  
$Q_8$. Let $F$ be the free group on $\{x,y\}$ and $N$ the normal subgroup of $F$ generated  
by $\{x^4,x^2y^2,yxy^3x\}$. Then, by the definition of free group, there exists a (unique) group homomorphism $f : F → Q_8$ by $f(x) = i$ and $f(y) = j$. As $Q_8 = 〈i,j〉,$ we see that $f$ must be surjective. It is easily seen that $f(x^4) = i^4 = 1$, $f(x^2y^2) = i^2j^2 =1$ and $f(yxy^3x) = jij^3i = 1$. Hence, $N ⊆ \Ker(f)$. Thus, there exists an induced homomorphism $f : F/N → Q_8$. Note that in $F/N$, $x^4 = 1, x^2 = y^{-2}$ (and so $y^4 = 1$ and $y^2 = x^2$) and $yx = x^3y$. Thus, every element in $F/N$ can be expressed in the form  
$x^iy^j$ for $0 ≤i ≤3$ and $0 ≤j ≤1$. Thus, $|F/N|≤8$. Since $f$ is surjective and $|Q_8|= 8$, we must have $f$ is bijective and thus an isomorphism.
***
#### Problem – Non-Abelian Group of Order 55 Presentation
Find with proof a presentation of a non-abelian group of order $55$.

##### *Proof.*
First, let’s construct a nonabelian group of order $55$. Let $H = 〈x〉$ be a cyclic  
group of order $11$ and $K = 〈y〉$ be a cyclic group of order $5$. Note that $\Aut(H) \cong\Z^\times_{11}$,  
which is cyclic of order $10$. Note that $4 ∈ \Z^\times_{11}$ has order $5$, so $φ_4 : H → H$ defined by  
$φ_4(x^i) = x^{4i}$ is an automorphism of order $5$. Thus, we can define $ψ : K →\Aut(H)$ by  $ψ(y^j) = φ^j_4$, which is a nontrivial homomorphism. Hence, $G = H \sdp_ψ K$ is a nonabelian group of order $55$. Let $a = (x,1)$ and $b = (1,y)$. Then $a^ib^j = (x,1)^i(1,y)^j = (x^i,y^j)$, so $G = 〈a,b〉$. Note that $a^{11} = 1$ and $b^5 = 1$. Also, $$ba= (1,y)(x,1) = (ψ_{(y)}(x),y) = (φ_4(x),y) = (x^4,y) = a^4b.$$One can now show that $〈s,t |s^{11} = 1,t^5 = 1,tst\inv s^{-4} = 1〉$ is a presentation for G using an argument very similar to the one given in Problem #4.
***
### Homework 6
#### Problem 
Let $G$ be a finite group and $K$ a normal subgroup of $G$.  Let $P$ be a Sylow $p$-subgroup of $K$ (for some prime $p$ dividing the order of $K$). Prove that $G=KN_G(P)$.  (Hint:  Let $g\in G$.  Then $gPg^{-1}$ is a Sylow $p$-subgroup of $K$ and hence conjugate in $K$ to $P$.)

##### *Proof.*
As in the hint, for $g ∈G$, we have $gPg\inv = kPk\inv$ for some $k ∈K$. Thus,  $(k\inv g)P(k\inv g)\inv = P$, which means $k\inv g ∈N_G(P)$. Hence, $g ∈KN_G(P)$.
***
#### Problem – Subgroups of $S_4$
Prove that $S_4$ has precisely three distinct subgroups of order $8$, all of which are isomorphic to $D_8.$

##### *Proof.*
Any subgroup of $S_4$ of order $8$ is a Sylow $2$-subgroup. By Sylow’s theorems,  
the number of Sylow $2$-subgroups is either $1$ or $3$. As any $2$-cycle or $4$-cycle must be  contained in a Sylow $2$-subgroup (since such elements generate subgroups of order $2i$, for some i) and there are six $2$-cycles and six $4$-cycles, there has to be more than one Sylow $2$-subgroup. Hence, there are precisely $3$ distinct subgroups of order $8$. 

As all of them are conjugate, and conjugation induces an isomorphism on the group, we see that all three subgroups are isomorphic. Hence, we just need to show that $S_4$ contains a subgroup isomorphic to $D_8$. Let $X$ be the set of left cosets of the subgroup $\{e,s\}$ of $D_8$. Note that $|X| = 4$. Let $G$ act on $X$ by left multiplication. This action induces a homomorphism $\varphi : G \to P(X)$ where $P(X)\cong S_4$ is the permutation group on $X$. As shown in class, the kernel of this homomorphism is the largest normal subgroup contained in $\{e,s\}$, which is $\{e\}$. Thus, $\varphi$ is injective and the image of $\varphi$ is a subgroup of $S_4$ isomorphic to $D_8$.
***
#### Problem 
Prove that a group of order 30 has a normal Sylow $3$-subgroup and a normal Sylow $5$-subgroup.

##### *Proof.*
Let $G$ be a group of order $30=2\cdot3\cdot5$, and note that by Sylow's Theorem we have the following:
- $n_3|10$ and $n_3\equiv 1\mod{3}$, and thus $n_3=1$ or $10$.
- $n_5|6$ and $n_3\equiv 1\mod{5}$, and thus $n_5=1$ or $6$.
If $n_3=10$ then we have $20$ elements of order $3$ and if $n_5=6$ then we have $24$ elements of order $5$, which is too many. Thus $n_3=1$ or $n_5=1$. 

Assume without loss of generality and $n_3=1$, so there exists one Sylow $3$-subgroup, $P$. Let $Q$ be a Sylow $5$-subgroup. As $P\nsg G$, we see $PQ\leq G$. As $|PQ=15|$, we see that $[G:PQ]=2$, the smallest prime dividing the order of $G$, making $PQ$ normal in $G$. 

Not Done, Tom uses a Lemma Alexandra doesn't have on file
***
#### Problem 
Prove that a group of order $pqr$, where $p<q<r$ are primes, has a normal Sylow subgroup.

##### *Proof.*
***
#### Problem – Order 75 with Element of Order 25
Let $G$ be a group of order $75$ which contains an element of order $25$.  Prove that $G$ is cyclic.

##### *Proof.*
Let $P$ be a Sylow $3$-subgroup and $Q$ a Sylow $5$-subgroup. By Sylow’s theorems, $n_5 = 1$ so $Q$ is normal in $G$. As $G = PQ$ and $P\cap Q = \{e\}$, we have that $G = Q\sdp_\phi P$, where $\phi : P \to\Aut(Q)$. Note that $\Aut(Q)\cong\Z^\times_{25}$, which is cyclic of order $20$. Since $|P| = 3$ and $\gcd(3,20) = 1$, we conclude that $\phi$ must be the trivial map. Hence, $G = P\times Q$, which is a direct product of cyclic groups of relatively prime order. Hence, $G$ is cyclic.
***
#### Problem – Order 231
Let $G$ be a group of order $231$.  Prove that the Sylow $11$-subgroup is contained in $\operatorname{Z}(G).$

##### *Proof.*
We have $|G|= 3 ·7 ·11$. Let $P,Q,R$ be Sylow subgroups of orders $3, 7,$ and  
$11$, respectively. By Sylow’s theorems, we easily see that $Q$ and $R$ are normal. Thus,  
$PQ$ is a subgroup of $G$ of order $21$, $G = PQR$ and $PQ∩R = \{e\}$. Thus, $G = R\sdp_φ PQ$ where $φ : PQ → \Aut(R)$. Since $|\Aut(R)| = 10$ and $\gcd(10,21) = 1$, we see that $φ$ must be the trivial map. Hence, $G = R\times PQ$. Thus every element of $R$ commutes with every element of $PQ$. Since $R$ is cyclic, we see that every element of $R$ commutes with every element of $PQR = G$; i.e., $R$ is contained in $Z(G)$.
***
### Homework 7
#### Problem 
Find the cardinality of the conjugacy class of $(123)(456)$ in $S_6$.  How many elements in $S_6$ commute with this element?  What is the cardinality of the conjugacy class of this element in $A_6?$  (Hint:  Note $(142536)$ commutes with $(123)(456)=(142536)^2$.)

##### *Proof.*
***
#### Problem 
Prove that any group of order $pq^2$, where $p$ and $q$ are primes, is solvable.  (Note:  Do not assume $p<q$.)

##### *Proof.*
***
#### Problem 
Prove that every group of order $48$ is solvable.

##### *Proof.*
***
#### Problem 
Prove that every group of order $72$ is solvable.

##### *Proof.*
***
#### Problem 
Suppose $m,n$ are positive integers such that $m$ divides $n$.  Assume that every group of order $n$ is solvable. Prove that every group of order $m$ is solvable.

##### *Proof.*
***
### Homework 8
#### Problem 
Let $R$ be a ring with identity. 
1. Prove that $a\cdot 0=0=0\cdot a$ for all $a\in R$.
2. Prove that $(-1)a=-a$ for all $a\in R$.

##### *Proof.*
***
#### Problem 
Let $R$ be a ring with identity. 
1. Let $a\in R$. Observe that $0a=(0+0)a=0a+0a$ by the distributive law. Subtracting $0a$ from both sides we have $0=0a$. A similar argument shows that $0=a0$. 
2. Let $a\in R$. Note that $-a+a=0$. Consider $(-1)a+a$. Using the distributive law we see that $(-1)a+a=a(-1+1)=a(0)=0$. Thus $-a$ and $(-1)a$ are both additive inverses of $a,$ making them unique. 

##### *Proof.*
***
#### Problem 
Let $R$ be a ring with identity. An element $a\in R$ is called {\it nilpotent} if  $a^n=0$ for some $n\ge 1$.
1. Give an example of a ring with a nonzero nilpotent.
2. Suppose $R$ is a commutative ring.  Prove that the set of all nilpotents in $R$ form an ideal of $R$.  (Note: You may assume the binomial theorem holds for commutative rings.)
3. Suppose $a\in R$ is nilpotent. Prove that $1-a$ is a unit in $R$.

##### *Proof.*
***
#### Problem 
Let $R$ be a ring with identity.   An element $e\in R$ is called {\it idempotent} if $e^2=e$.
1. Give an example of a ring which has an idempotent other than $0$ or $1$.
2. Prove that if $e$ is idempotent, so is $1-e$.
3. Suppose $R$ is commutative and $e$ an idempotent.  Let $Re:=\{re\mid r\in R\}$.  Observe that $Re$ is a commutative ring  (with identity $e$). Prove that the map $\phi:R\to Re \times R(1-e)$ given by $\phi(r)=(re, r(1-e))$ is a ring isomorphism.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring with identity and $\{I_{\alpha}\mid \alpha\in \Lambda\}$ a set of ideals of $R$ (indexed by some set $\Lambda$).
Prove that $$\displaystyle\sum_{\alpha} I_{\alpha}:=\left\{\sum_{\alpha} i_{\alpha}\mid i_{\alpha}\in I_{\alpha} \text{ for all } \alpha, \text{ and } i_{\alpha}=0 \text{ for all but finitely many }\alpha\right\}$$ is an ideal.

##### *Proof.*
***
#### Problem 
Prove that a commutative ring is a field if and only if the ring has exactly two distinct ideals.

##### *Proof.*
***
#### Problem 
Prove that the ideal $(2,x)$ of the ring $\mathbb Z[x]$ is not a principal ideal.

##### *Proof.*
***
#### Problem 
Let $R$ be a commutative ring with identity, $x$ an indeterminate,  and $f(x)\in R[x]$.  Suppose $f(x)$ is a zero-divisor in $R[x]$.  Prove that there exists $b\in R, b\neq 0$ such that $bf(x)=0$.  (Hint:  Write $f(x)=a_nx^n+\cdots+a_0$ where $a_n\neq 0$.  Choose a nonzero polynomial $g(x)=b_mx^m+\cdots +b_0$ (with $b_m\neq 0$) of least possible degree such that $fg=0$.  Note that $a_nb_m=0$.  Hence, $\deg a_ng<\deg g$.  Since $f(a_ng)=a_n(fg)=0$ and $a_ng$ has degree less than $g$, we must (by choice of $g$) have $a_ng=0$.  
Now looking at the coefficient of $x^{n+m-1}$ in $fg$, we have $a_{n-1}b_m+a_nb_{m-1}=0$.  But $a_nb_{m-1}=0$ as $a_ng=0$.  Hence, $a_{n-1}b_m=0$.  Thus, $\deg a_{n-1}g<m$ and $f(a_{n-1}g)=0$.  Again, by minimality of $g$, we have $a_{n-1}g=0$.   Continue this argument using induction to get that $a_ig=0$ for all $i$.  Hence, $a_ib_m=0$ for all $i$, and we may choose our $b=b_m$.)

##### *Proof.*
***
### Midterm 1
#### Problem
Let G be a group and $a, b ∈ G$ two elements of finite order. Suppose $ab = ba$ and  
$〈a〉∩〈b〉= {1}$.

(a) Prove that $|ab|= \lcm(|a|, |b|)$.
(b) Use (a) to prove that if $H$ and $K$ are finite cyclic groups of relatively prime orders  
then $H\times K$ is cyclic.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $G$ be a group acting on a set $X$. For $a\in X$, let $\Orb(a)$ denote the orbit of a and $G_a$ the stabilizer of a.
(a) Prove the Orbit-Stabilizer theorem: $|\Orb(a)|= [G : Ga]$.
(b) Suppose $G$ is a group of prime order and there are at least two distinct orbits. Prove that the action is trivial, i.e., that the kernel of the action is all of $G$.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $G$ be a group and $N\leq H$ subgroups of $G$.
(a) Give an example such that $N\nsg H$ and $H\nsg G$ but $N$ is not normal in $G$.
(b) Suppose $N\nsg G$ and $G/N$ is abelian. Prove that $H\nsg G$ and $G/H$ is abelian.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $G$ be a group (possibly infinite) and $H \leq K$ subgroups of $G$. Suppose $[G : H]$ is finite. Prove that $[G : H] = [G : K][K : H].$ (Hint: First prove this in the case $G$ is a  
finite group. Then prove you can reduce to the finite case.)

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $G$ be a finite group and $K$ a subgroup of $G$ such that: $[G : K] = 2$, $K$ is simple, and $Z(G) = \{e\}$. Prove that the only normal subgroups of $G$ are $\{e\}, K$, and $G$. (Hint: Let H be a normal subgroup of G. Then H ∩K is a normal subgroup of K.)

##### *Proof.*
***
### Midterm 2
#### Problem
Prove that a group of order $30$ has a normal Sylow $3$-subgroup and a normal Sylow $5$-subgroup.

##### *Proof.*
***
#### Problem
Let $G$ be a group, and $K\leq H$ subgroups of $G$ such that $K$ is a characteristic subgroup of $H$ and $H\nsg G$. Prove that $K\nsg G$. 

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Prove that any group of order $3^2\cdot 11\cdot17$ is abelian.
##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Find a presentation (with justification) for a nonabelian group which is a semidirect product of a cyclic group of order $4$ and a cyclic group of order $3$.
##### *Proof.*

***
#### Problem
Let $G$ be a group and $H,K$ solvable subgroups of $G$ such that $G=HK$. 
(a) Prove that if either $H$ or $K$ is normal then $G$ is solvable. (Note: There is not assumption on the order of $H\cap K$.)
(b) Show that Part (a) is false if neither $H$ nor $K$ is assumed to be normal. (Hint: The obvious choice for $G$ works.)
##### *Proof.*

###### Part (a)
***
###### Part (b)
***
### Final Exam
#### Problem
Let $R$ be an integral domain.
(a) Prove that every prime element is irreducible.
(b) Prove that if $R$ is a PID then every irreducible element is prime.
##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Prove that a ring $R$ has a non-trivial idempotent if and only if $R\cong S\times T$, where $S$ and $T$ are rings.

##### *Proof.*
***
#### Problem
Let $R$ be a ring.
(a) Prove that an element cannot be both a unit and a zero-divisor.
(b) Give an example of a ring $R$ and an element $a\in R$ which is neither a unit nor a zero-divisor.
(c) Prove that if $R$ is finite then every element is either a unit of a zero-divisor.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
###### Part (c)
***
#### Problem
Let $I$ be a finitely generated ideal of $R$. Suppose every element of $I$ is nilpotent. Prove that there exists an integer $n\geq 1$ such that $b^n=0$ for all $b\in I$. 

##### *Proof.*

***
#### Problem
Let $R$ be a ring. An ideal $I$ of $R$ is *irreducible* if $I\neq R$ and whenever $I=J\cap K$, where $J$ and $K$ are ideals of $R$, then either $I=J$ or $I=K$.
(a) Prove that every prime ideal of $R$ is irreducible.
(b) Suppose $R$ is noetherian. Prove that every ideal $I\neq R$ is an intersection of a finite number of irreducible ideals. (Note: We consider an irreducible ideal as the intersection of one irreducible ideal)

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $R$ be a domain.
(a) Define what it means for $R$ do be a UFD
(b) Give an example, with justification, of a domain which is not a UFD.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem
Let $I=\{f\in C[0,1]|f(x)=0\text{ on } [0,b]\text{ for some } b>0\}$
(a) Prove that $I$ is an ideal of $C[0,1]$.
(b) Prove that $I$ is not finitely generated.

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
#### Problem

##### *Proof.*

###### Part (a)
***
###### Part (b)
***
