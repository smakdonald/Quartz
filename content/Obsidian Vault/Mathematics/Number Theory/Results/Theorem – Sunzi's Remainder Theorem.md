#### $\thm$ – Sunzi's Remainder Theorem (Integers)
Suppose $m, n \in\N$[^1] are relatively prime. Then the [[Function|function]] $\psi: \Z/(mn)\to \Z/(m) \times \Z/(n)$[^2] defined by $\psi ([x]) = ([x \mod m], [x \mod n])$[^3] is a well-defined [[Bijective|bijection]] that preserves the ring operations: for $[x], [y] \in\Z/(mn)$, we have $\psi ([x] + [y]) = \psi ([x]) + \psi ([y])$  and  $\psi ([x] \cdot  [y]) = \psi ([x]) \cdot  \psi ([y])$.

##### *Proof.*
Since both m and n divide mn, \psi  is well defined by Lemma 4.7.1. We then  
verify  
\psi ([x] + [y]) = ([x + y \mod m], [x + y \mod n])  
= ([x \mod m] + [y \mod m], [x \mod n] + [y \mod n])  
= ([x \mod m], [x \mod n]) + ([y \mod m], [y \mod n])  
= \psi ([x]) + \psi ([y])  
by the definition of the ring operations in Cartesian products (Theorem 4.7.2) and  
using Lemma 4.2.4. Verifying the result for multiplication follows similarly.  
Next, to establish that \psi  is a bijection, it’s clear that \Z/(mn) and \Z/(m) \times \Z/(n)  
have the same number of elements (namely, mn), and so to show that our function  
is a bijection it suffices to show it is surjective. To this end, suppose ([a], [b]) \in  
\Z/(m) \times \Z/(n). Since \gcd(m, n) = 1, we can write  
sm + tn = 1  
for some s, t \in\Z. Let x = bsm + atn. Then x \equiv 0 + atn \equiv a(1) \equiv a (\mod m) and  
x \equiv bsm + 0 \equiv b(1) + 0 \equiv b (\mod n). Thus, by definition \psi ([x]) = ([a], [b]), as  
desired. Since ([a], [b]) was arbitrary, we conclude \psi  is surjective.

[^1]: Notation: [[Mathematics/Number Theory/Definitions/Natural Numbers]]
[^2]: Notation: [[Z(n)]], [[Direct Product, Sum]]
[^3]: Notation: [[Congruent]]

#### $\thm$ – Sunzi's Remainder Theorem (Groups)
Suppose $m = p_1^{e_1} \cdots p_l^{e_l}$ for distinct primes $p_1, \dots, p_l$. Then there is an [[Isomorphism|isomorphism]]
$$\phi: \Z/m \xra{\cong} \Z/(p_1^{e_1}) \times \cdots \times \Z/(p_l^{e_l})$$
given by
$$\phi([j]_m) = ([j]_{{p_1}^{e_1}}, \cdots, [j]_{{p_l}^{e_l}})$$
where $[j]_b$ denotes the class of an integer $j$ in $\Z/b$.
##### *Proof.*
Using the UMP for infinite cyclic groups, 
we let $\psi: \Z \to \Z/(p_1^{e_1}) \times \cdots \times \Z/(p_l^{e_l})$ be the unique homomorhism that sends $1$ to 
$([1]_{{p_1}^{e_1}}, \cdots, [1]_{{p_l}^{e_l}})$. Then 
$$
\psi(j) = ([j]_{{p_1}^{e_1}}, \cdots, [j]_{{p_l}^{e_l}}).
$$
Clearly $m \in \ker(\psi)$ and so $\langle m \rangle \subseteq \ker(\psi)$. Conversely, if $\psi(n) = 0$, then $p_i^{e_i} \mid n$ for all $i$ and since 
$p_1^{e_1}, \dots, p_l^{e_l}$ are pairwise relatively prime, it follows that $m \mid n$. This proves $\ker(\psi) = \langle m \rangle$. The claim follows by the first isomorphism theorem.
***

#### $\thm$ – Sunzi's Remainder Theorem (Rings)
Suppose $I$ and $J$ are [[Ideal|ideals]] in a [[Commutative Ring|commutative]] [[Ring|ring]] $R$ such that $I + J = R$. Then $I \cap J = I \cdot J$ (where $I \cdot J$ is defined as the set of all sums of products of  the form $ab$ with $a \in I$ and $b \in J$) and there is an [[Isomorphism|isomorphism]] of $R$-[[Module|modules]] $$R/(I J) \cong R/I \oplus R/J.$$
In particular, if $R$ is a [[Unique Factorization Domain|UFD]] and $x$ and $y$ are relatively prime elements of $R$, then $$R/(xy) \cong R/x \oplus R/y$$

###### *Proof.* 
Note that $I \cdot J \subseteq I \cap J$ holds in general for any pair of ideals. If $I + J = R$ then $a + b = 1$ for some $a \in I$ and $b \in J$. Given $x \in I \cap J$ we have $xa + xb = x$ with $xa \in I \cdot J$ and $xb \in I \cdot J$, which proves $x \in I \cdot J$.

For the second assertion define $g: R \to R/I \oplus R/J$ to be the $R$-module homomorphism $g(r) = (r +I, r + J)$. Note that the kernel of $g$ is $I \cap J$ which equals $I\cdot J$ by the first assertion. I claim $g$ is onto: Pick $(x + I, y +J) \in R/I \oplus R/J$. With $a,b$ chosen as above, we have $$ g(xb + ya) = (xb + ya + I, xb + ya + J) = (xb + I, ya + J) = (x + I, y +J).$$The last equation holds since $xa + xb = x$ and thus $xb + I = xb + xa + I = x + I$ and similarly $ya + J = y + J$.

For the final assertion, recall that when $R$ is a UFD, two principle ideals $Rx$ and $Ry$ satisfy $Rx + Ry = R$ if and only if $x$ and $y$ are relatively prime. Also, for $I = Rx$ and $J = Ry$, we have $I\cdot J = R(xy)$. 
***