# What is a Number?
## Algebraic Number Systems
#### $\defn$ – Natural Numbers
![[Mathematics/Number Theory/Definitions/Natural Numbers]]
#### $\defn$ – Integers
![[Integers]]
#### $\defn$ – Rational Numbers
![[Rational Numbers]]
#### $\defn$ – Real Numbers
![[Real Numbers]]
#### $\defn$ – Complex Numbers
![[Complex Numbers]]
## New Numbers, New Worlds
#### $\defn$ – Gaussian Integers
![[Gaussian Integers]]
#### $\thm$ – Complex Operations
![[Theorem – Complex Operations]]
#### $\defn$ – Complex Conjugate
![[Complex Conjugate]]
# The Last Two Millennia
## Quadratic Equations
#### Question – 
What are the solutions to the equation $x^{2} + y^{2} = 3$? What about $x^{2} + y^{2} = 5$?
#### $\ex$
Find all rational solutions to $x^{2} + y^{2} = 1$.
#### $\defn$ – Pythagorean Triple
![[Pythagorean Triple]]
#### $\thm$ – Classifying Pythagorean Triples
![[Theorem – Classifying Pythagorean Triples]]
#### $\rem$
In Chapter 3, once we have established some basic properties of divisibility, primes, and common factors, we will be able to refine the parameterization: every Pythagorean triple is a multiple of one coming from a pair $(u, v)$ with one of $u$, $v$ even, one odd, and $u$ and $v$ having no factors in common.
#### $\thm$ – One Rational Solution Gives Infinite
![[Theorem – One Rational Solution Gives Infinite]]
## Diophantine Equations
#### $\defn$ – Diophantine Equation
![[Diophantine Equation]]
#### $\ex$ – 
Vineas and Herb have a truly marvelous collection of rubber balls. 
When Vineas takes possession of the balls, he arranges them in a perfect square 
pyramid. When Herb takes possession of the balls, he arranges them in a perfect 
flat square. How many balls are there?
#### $\defn$ – Elliptic Curve
![[Elliptic Curve]]
# In $\Z$ Beginning
## Algebraic Structures
#### $\defn$ – Ring
![[Ring]]
#### $\defn$ – Commutative Ring
![[Commutative Ring]]
#### $\defn$ – Unital Ring
![[Unital Ring]]
#### $\defn$ – Field
![[Field]]
#### $\ex$ – 
The sets $\Z$, $\Z[i]$, and $\R[x]$ are commutative rings with unity but are not fields.
#### $\ex$ – 
The set $\N$ is not even a ring, as elements of $\N$ lack additive inverses (not to mention an additive identity).
#### $\ex$ – 
The set of $n\times n$ matrices with real entries forms a non-commutative ring with unity. Many elements of this ring do not have multiplicative inverses.
#### $\defn$ – Subring
![[Subring]]
#### $\ex$ – 
The rings $\Q$ and $\R$ are both subfields of the field $\C$, while $\Z$ and $\Z[i]$ are merely subrings of $\C$
#### $\ex$ – 
The set of odd integers has additive inverses $1$ but is not closed under addition. The set $2\Z = \{2n : n \in \Z\}$ of even integers is a commutative ring without unity and a subring of $\Z$.
#### $\rem$ – 
The linguistically curious will wonder about the seemingly out-of-place words “rings” and “fields” peppering the landscape of mathematical jargon. There is no universal consensus as to the etymology, though it seems likely to have come in part from unfaithful translations from French or German. For example, the French word corps used for fields translates most literally as “body,” as in “body of water” or one’s “body of knowledge” (much like, say, one’s “field of vision”), and so it may have been a cultural difference in the use of those words that provoked the change in metaphors
#### $\defn$ – Integral Domain
An integral domain is a commutative ring with unity in which the product of non-zero elements is always non-zero; that is, for all $a$ and $b$ in the ring $R$, $ab = 0$ if and only if $a = 0$ or $b = 0.$
#### $\lem$ – Fields are Integral Domains
![[Lemma – Fields are Integral Domains]]
#### $\lem$ – Integral Domain and Polynomial Degree
![[Lemma – Integral Domain and Polynomial Degree]]
#### $\lem$ – Factor Theorem
![[Lemma – Factor Theorem]]
#### $\defn$ – Divides
Given elements $a$ and $b$ in a commutative ring $R$, we say that $a$ divides $b$ if there exists an element $c \in R$ such that $ac = b$. We write $a | b$ to denote that a divides $b$, and say that $a$ is a divisor of $b$, or equivalently that $b$ is a multiple of $a$. If $a$ does not divide $b$, we write $a\not\mid b$.
## Linear Diophantine Equations & the Euclidean Algorithm
#### $\ex$ – 
Suppose one can purchase boxes of O’Nuggets in boxes of either a or b nuggets so that by buying x boxes with a nuggets and y boxes with b nuggets, the possible numbers of Chicken O’Nuggets we can purchase are the numbers of 
the form ax + by. 

What are the possible numbers of nuggets we can buy? That is, for which values of $c$ can we solve the linear equation $ax + by = c$?
#### $\defn$ – GCD
Let $a$ and $b$ be integers, not both equal to $0$. A common divisor of $a$ and $b$ is an integer $d$ such that $d | a$ and $d | b$. The largest integer that divides both $a$ and $b$ is called the greatest common divisor of $a$ and $b$, denoted $\\gcd(a, b)$. Similarly, a common multiple of $a$ and $b$ is an integer $n$ such that $a | n$ and $b | n$. The smallest positive integer $n$ satisfying $a | n$ and $b | n$ is called the least common multiple of $a$ and $b$, denoted $\lcm(a, b)$. We say that $a$ and $b$ are relatively prime (or coprime) if $\gcd(a, b) = 1$.
#### $\ex$ – 
Be sure to convince yourself these results are what the definition 
above mandates: 
\gcd(15, 10) = 5 \gcd(3, -7) = 1 \gcd(-15, -15) = 15 
\gcd(0, 12) = 12 \gcd(0, 0) = undefined.
#### $\lem$ – Linear Combination Lemma
![[Lemma – Linear Combination Lemma]]
#### $\cor$ – Sums and Divisibility
![[Corollary – Sums and Divisibility]]
#### $\cor$ – Properties of GCD
![[Corollary – Properties of GCD]]
#### $\ex$ – 
We systematically apply the identities in Corollary 3.2.6 to compute the \gcd of 52 and 91: 
\gcd(91, 52) = \gcd(52, 91) = \gcd(52, 91 - 52) = \gcd(52, 39) 
= \gcd(39, 52) = \gcd(39, 52 - 39) = \gcd(39, 13) = 13.
#### $\ex$ – 
#### $\thm$ – The Division Algorithm
![[Theorem – The Division Algorithm]]
#### $\defn$ – Mod
![[Mod]]
#### $\ex$ – 
Verify each of the following using mental arithmetic: 
37 \mod 5 = 2 77 \mod 7 = 0 12 \mod 15 = 12 
4 \mod 1 = 0 - 3 \mod 7 = 4 97 \mod 23 = 5 
What are the quotients q in each case?
#### $\lem$ – Reduction Lemma
![[Lemma – Reduction Lemma]]
#### $\ex$ – 
Compute \gcd(1914, 899). 
Solution Noting that 1914 = 899 \cdot 2 + 116, we begin with \gcd(1914, 899) = 
\gcd(899, 116). Then continuing, we find 
\gcd(1914, 899) = \gcd(899, 116) = \gcd(116, 87) = \gcd(87, 29) = 29 
by repeated application of the Reduction Lemma.
#### $\thm$ – The Euclidean Algorithm
![[Theorem – The Euclidean Algorithm]]
#### $\cor$ – GCD and Coefficients
![[Corollary – GCD and Coefficients]]
#### $\cor$ – GCD and Fractions
![[Corollary – GCD and Fractions]]
#### $\rem$ – 
The previously mentioned efficiency of the Euclidean Algorithm can be quantified explicitly. In what might be retroactively classified as one of the first theorems in the branch of mathematics known as computational complexity 
theory, Gabriel Lamé proved in 1844 that the Euclidean Algorithm never takes more steps than five times the number of digits in the smaller of the two inputs (Exercise 3.41)
#### $\thm$ – Bézout’s Identity
![[Theorem – Bézout’s Identity]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
Find \gcd(429, 273). Let a = 429 and b = 273. 
Solution We first apply the Division Algorithm to reduce the \gcds. 
429 = 273 \cdot 1 + 156 \gcd(429, 273) = \gcd(273, 156) 
273 = 156 \cdot 1 + 117 \gcd(273, 156) = \gcd(156, 117) 
156 = 117 \cdot 1 + 39 \gcd(156, 117) = \gcd(117, 39) 
117 = 39 \cdot 3 + 0 \gcd(117, 39) = \gcd(39, 0) = 39 
Retracing the steps of the algorithm we can solve for the \gcd(429, 273): 
\gcd(429, 273) = 39 = 156 - 117 
= 156 - (273 - 156) 
= (429 - 273) - (273 - (429 - 273)) 
= 2 \cdot 429 - 3 \cdot 273. 
Thus, we can represent \gcd(429, 273) as a linear combination of 429 and 273. Note 
that we don’t simplify along the way (other than combining like remainders), as that 
would simply unravel all our hard work!
#### $\thm$ – Solutions to $ax+by=c$
![[Theorem – Solutions to $ax+by=c$]]
#### $\lem$ – Euclid's Lemma
![[Lemma – Euclid's Lemma]]
#### $\thm$ – Solutions to Diophantine Equations
![[Theorem – Solutions to Diophantine Equations]]
#### $\thm$ – Fundamental Theorem of GCDs
![[Theorem – Fundamental Theorem of GCDs]]
## The Fundamental Theorem of Arithmetic
#### $\defn$ – Unit
![[Unit]]
#### $\defn$ – Associates
![[Associates]]
#### $\ex$ – 
As you may have discovered in Exploration C, 
• the units of Z are precisely \pm1, 
• the units of \Z[i] are {\pm1, \pmi}, 
• the units of R and Q (and any field) are everything except 0, and 
• the units of R[x] are all non-zero constant polynomials
#### $\defn$ – Prime
![[Prime]]
#### $\thm$ – Fundamental Theorem of Arithmetic
![[Mathematics/Number Theory/Results/Theorem – Fundamental Theorem of Arithmetic]]
#### $\ex$ – 
Consider again the ring of even integers, 2Z. We can still talk about 
divisibility since, e.g., 10 | 20 (because 20 = 2 \cdot 10). On the other hand, we now 
have 2  6 since there is no k \in 2Z such that 2k = 6. In fact, 6 has no divisors in 
this ring (not even itself!), making it vacuously prime, and likewise, for any even 
number that is not a multiple of 4. But now consider the identity 
2 \cdot 30 = 60 = 6 \cdot 10. 
This provides two distinct factorizations of 60 as the product of two prime elements 
of this ring!
#### $\cor$ – The Prime Divisor Property
![[Corollary – The Prime Divisor Property]]
#### $\rem$
In fact, the Prime Divisor Property provides a property of primes that could have been used as the definition of a prime number. As it turns out, this is precisely the definition we will take of a prime element in a more general ring when we come to that stage.
#### $\cor$ – Arbitrary Prime Divisor Property
![[Corollary – Arbitrary Prime Divisor Property]]
#### $\cor$ – Prime Divisor and Exponents
![[Corollary – Prime Divisor and Exponents]]
#### $\cor$ – Roots of Primes Irrational
![[Corollary – Roots of Primes Irrational]]
## Factors and Factorials
#### $\defn$ – Valuation
![[Valuation]]
#### $\lem$ – Valuation of Products
![[Lemma – Valuation of Products]]
#### $\lem$ – Valuation and Divisibility
![[Lemma – Valuation and Divisibility]]
#### $\lem$ – Valuations, GCD, LCM
![[Lemma – Valuations, GCD, LCM]]
#### $\lem$ – GCD $\times$ LCM
![[Lemma – GCD $times$ LCM]]
#### $\lem$ – Valuation and Square Numbers
![[Lemma – Valuation and Square Numbers]]
#### $\cor$ – Roots of Non Squares Irrational
![[Corollary – Roots of Non Squares Irrational]]
#### $\thm$ – Rational Root Test
![[Theorem – Rational Root Test]]
#### $\cor$ – Roots of Monic Polynomials
![[Corollary – Roots of Monic Polynomials]]
#### $\lem$ – Power Lemma
![[Lemma – Power Lemma]]
#### $\cor$ – All Primitive Pythagorean Triples
![[Corollary – All Primitive Pythagorean Triples]]
## The Prime Archipelago
#### $\lem$ – Composite Numbers and Prime Divisors
![[Lemma – Composite Numbers and Prime Divisors]]
#### Sieve – Sieve of Eratosthenes
Fix $n > 2$. To find all primes $p \leq n$: 
• Begin with a list of the integers $2 \leq k \leq n$. Initially, all numbers are neither circled nor crossed out. 
• Circle the smallest remaining number (that is, not circled and not crossed out) and cross off all of its multiples in the list. 
• Repeat the previous step until all numbers less than or equal to $\sqrt{n}$ have been circled or crossed out. 
• Circle every remaining number on the list not yet crossed out. Now the circled numbers are all prime, and all crossed-out numbers are composite
#### $\thm$ – Infinite Primes
![[Mathematics/Number Theory/Results/Theorem – Infinite Primes]]
#### $\defn$ – Prime Counting Function
![[Prime Counting Function]]
#### $\thm$ – The Prime Number Theorem
![[Theorem – The Prime Number Theorem]]
# In the Mod-$n$ Era
## Equivalence Relations and the Binary World
#### $\defn$ – $\Z_{2}$
#### $\defn$ – $\Z_{3}$ 
#### $\defn$ – Equivalence Relation
![[Equivalence Relation]]
#### $\defn$ – Equivalence Class
![[Equivalence Relation]]
#### $\lem$ – Equivalence Classes Partition
![[Theorem – Equivalence Classes Partition]]

##### *Proof.*
If [a] \cap [b] = ∅, choose any c \in [a] \cap [b]. Then (a, c), (b, c) \in R and thus 
(c, b) \in\R by symmetry, and finally (a, b) \in\R by transitivity. Transitivity further 
implies that anything equivalent to a is equivalent to anything equivalent to b, and 
vice versa, so [a] = [b]. For the second claim, we note that each element a \in S is 
an element of its own equivalence class [a] (by reflexivity), so the union of all the 
equivalence classes contains all elements of S.
#### $\rem$ – 
It is also true that any partition of S can be used to define an equivalence relation, namely, the equivalence relation which declares two elements to be equivalent if and only if they are in the same part of the partition. Thus, the two notions are roughly synonymous concepts, and we speak freely of taking a set and “partitioning it into equivalence classes.”
## The Ring of Integers Modulo n
#### $\defn$ – Congruent
![[Congruent]]
Given a natural number $n$, we say integers $a$ and $b$ are congruent modulo $n$, denoted $a \equiv b (\mod n)$, if $a \mod n = b \mod n$, i.e., they have the same remainder 
when divided by $n$. The equivalence classes with respect to this relation are called 
congruence classes and denoted $[a] = \{b \in\Z : a \equiv b (\mod n)\}$. It is common to use the notation $[a]_{n}$ in place of simply $[a]$ when the modulus $n$ needs emphasizing, but the subscript is otherwise typically left off. We note the equivalent statements 
$[a]n = [b]n \Longleftrightarrow a \equiv b (\mod n) \Longleftrightarrow n | a - b$.
#### $\ex$ – 
Consider congruence modulo 7 on Z, where two integers are con- 
gruent if they have the same remainder when divided by 7. Since there are only 
7 possible remainders when divided by 7, there are 7 disjoint equivalence classes 
of Z under this equivalence relation: [0], [1], [2], [3], [4], [5], and [6], where 
[a] consists of those integers n such that n \mod 7 = a. The Division Algorithm 
confirms the results of Lemma 4.1.5 in this case: every integer is in exactly one of 
these 7 classes. Of course, we can refer to an equivalence class by any of its other 
elements as well (other representatives of the equivalence class). For example, 
we have 
\cdots = [-9] = [-2] = [5] = [12] = [19] = \cdots.
#### $\defn$ – $\Z_{n}$
![[Z(n)]]
#### $\lem$ – Well-definedness of Modular Arithmetic
![[Lemma – Well-definedness of Modular Arithmetic]]
#### $\ex$ – 
Compute 39 \cdot 99 + 95 \cdot 64 \mod 19. 
Solution First, observe that a naive solution technique certainly exists. We could 
compute, in Z, the value of 39 \cdot 99 + 95 \cdot 64, and then use long division to find 
the remainder when this result is divided by 19. Much more expedient is to employ 
Lemma 4.1.5, which shows us that the answer to this question remains unchanged 
if we replace any of 39, 99, 95, or 64 with any other congruent-mod-19 value. In 
particular, mental arithmetic provides for us 
39 \equiv 1 \mod 19, 99 \equiv 4 \mod 19, 95 \equiv 0 \mod 19, and 64 \equiv 7 \mod 19, 
and so making these substitutions, we find 
39 \cdot 99 + 95 \cdot 61 \equiv 1 \cdot 4 + 0 \cdot 7 \equiv 4 (\mod 19). 
We conclude that 39 \cdot 99 + 95 \cdot 64 \mod 19 = 4.
## Reduce First and ask Questions Later
#### $\ex$ – 
Example 4.3.1 The bread and butter calculations of modular arithmetic mirror 
those of Example 4.2.5, involving only addition and multiplication of integers. A 
streamlined version of this might look like 
38 \cdot 17 + 40 \equiv 3 \cdot 3 + 5 \equiv 9 + 5 \equiv 2 + 5 \equiv 0 (\mod 7), 
which shows that 7 | 38 \times 17 + 40.
#### $\ex$ – 
Example 4.3.2 Compute 173 \mod 5. 
Solution Since exponentiation is simply repeated multiplication, we find 
173 \equiv 17 \cdot 17 \cdot 17 \equiv 2 \cdot 2 \cdot 2 \equiv 2 3 \equiv 3 (\mod 5), 
so 173 \mod 5 = 3.
#### $\lem$ – Functions and Modular Arithmetic
![[Lemma – Functions and Modular Arithmetic]]
#### $\ex$ – 
To compute 71,423 \mod 9, we note 
71,423 = 7 \cdot 10 4 + 1 \cdot 10 3 + 4 \cdot 10 2 + 2 \cdot 10 1 + 3 
\equiv 7 \cdot 14 + 1 \cdot 13 + 4 \cdot 12 + 2 \cdot 11 + 3 
\equiv 7 + 1 + 4 + 2 + 3 
\equiv 17 
\equiv 8 (\mod 9).

#### $\thm$ – Divisibility-by-9 Test
![[Theorem – Divisibility-by-9 Test]]
#### $\rem$ – 
Since 10k \equiv 1 (\mod 3), the analogous test works for divisibility 
by 3 as well. In fact, it’s not hard to see that such a divisibility-by-n test exists 
if and only if 10 \equiv 1 (\mod n). In turn, this holds if and only if n | 10 - 1, i.e., 
only when n = 3 or n = 9 (fine, fine, and n = 1). One more clean divisibility 
test is worth mentioning (Exercise 4.2), coming from the observation that 10k \equiv 
(-1)k \mod 11.
#### $\lem$ – Diophantine Equation with No Solutions
![[Lemma – Diophantine Equation with No Solutions]]
#### $\defn$ – Modular Reduction
![[Modular Reduction]]
#### $\ex$ – 
If E is the elliptic curve y^{2} = x3 + 16x - 22, reducing E \mod 7 
gives us the reduced curve y^{2} = x3 + 2x + 6. In looking for the set of solutions 
E(\Z/(7)), we start by examining the possible values of y^{2} \in\Z/(7), 
[0]2 = [0], [1]2 = [6]2 = [1], [2]2 = [5]2 = [4], and [3]2 = [4]2 = [2]. 
Thus, we need to find values of x \in\Z/(7) such that x3 + [2]x + [6] \in 
{[0], [1], [2], [4]}. Since \Z/(7) is pretty small, we can just work our way through the possibilities. For x = [0], [1], \dots, [6], we get x3 + [2]x + [6] is equal to 
[6], [2], [4], [4], [1], [1], and [3], respectively. Matching these outputs with val- 
ues of y^{2} we find there are no solutions with x = [0] or [6], and all other values of 
x yield two solution points (x, y) \in E(\Z/(7)) = {([1], [3]), ([1], [4]), ([2], [2]), 
([2], [5]), ([3], [2]), ([3], [5]), ([4], [1]), ([4], [6]), ([5], [1]), ([5], [6])} for a 
total of 10 points (out of 49 possible in \Z/(7) \times \Z/(7)).
#### $\thm$ – Mod-$n$ Root Test
![[Theorem – Mod-$n$ Root Test]]
## Division, Exponentiation, and Factorials in $\Z/(n)$
#### $\ex$ – 
Solve 3x \equiv 5 (\mod 11).
#### $\rem$ – 
Note that if the ring is non-commutative, we must take care to 
multiply on the same side: ax = b implies a-1ax = a-1b, not a-1ax = ba-1. 
The non-commutative case will not occupy much of our attention, but serves as 
explanation for the decision to consistently write “a-1b” instead of “ b 
a ” in most 
ring settings, as the fraction notation gives us the heebie-jeebies in a general ring.
#### $\thm$ – Inverses in $\Z/(n)$
![[Theorem – Inverses in $Z(n)$]]
#### $\ex$ – 
Find [7] -1 in \Z/(93).
#### $\cor$ – $\Z/(n)$ and Fields
![[Corollary – Z(n) and Fields]]
#### $\rem$ – 
Also in Lemma 3.1.11 is the observation that not every integral 
domain is a field (e.g., R = Z). However, while we do not prove it here, it is true 
that for rings with finitely many elements, the two notions are equivalent, and the 
above Corollary is a special case of this result.
#### Question
What is the sum of all of the elements of \Z/(n)?
#### Question
What is the product of all of the non-zero elements in \Z/(n)?
#### $\lem$ – Inverses in $\Z/(n)$
![[Lemma – Inverses in $Z(n)$]]
#### $\rem$ – 
Alternative proof: \pm1 are clearly solutions to x^{2} -1 \equiv 0 (\mod p). 
Further, since \Z/( p) is an integral domain, the polynomial x^{2} - 1 \in\Z/( p)[x] has 
at most two roots by Lemma 3.1.13, so [1] and [-1] are the only two solutions in 
\Z/( p).
#### $\thm$ – Wilson's Theorem
![[Theorem – Wilson's Theorem]]
#### $\ex$ – 
Reduce 1162 \mod 5.
We can multiply either before or after reducing \mod 5, so could either: 
(a) Compute the decimal expansion of 1162 first, and then do long division to com- 
pute its remainder when divided by 5 or 
(b) Remember to reduce first and ask questions later, in which case we note 1162 \equiv 
162 \equiv 1 (\mod 5).
#### $\ex$ – 
Reduce 1162 \mod 37.
## Group Theory & Rings of Integers mod $n$
#### $\defn$ – Group
![[Group]]
#### $\defn$ – Abelian Group
![[Abelian Group]]
#### $\defn$ – Order
![[Order]]
#### $\defn$ – Group of Units
![[Group of Units]]
#### $\thm$ – Group of Units is a Group
Let $R$ be a ring with unity. Then $\R^{\times}$ forms a multiplicative group.

##### *Proof.*
Let R be a ring with unity, with multiplicative identity 1, and let R^{\times} be the 
set of units of R. We show that R is a group (using the multiplication of R as its 
operation). First, 1 \in\R^{\times} and is clearly the identity of R^{\times}. Multiplication in R^{\times} is 
associative because R is a ring (and one of the axioms of a ring is associativity of 
multiplication). The inverse of a unit of R is also a unit of R, and so R^{\times} contains a 
multiplicative inverse for each element. All that remains to show is closure, that the 
product of two units in R is again a unit in R. Given units u1, u2 of R, we claim that 
u1u2 is again a unit, with inverse u-1 
2 u-1 
1. Indeed we compute, using associativity, 
that 
(u1u2)(u-1 
2 u-1 
1 ) = u1(u2u-1 
2 )u-1 
1 = u1 1u-1 
1 = u1u-1 
1 = 1, 
and likewise (u-1 
2 u-1 
1 )(u1u2) = 1. Thus, u1u2 is a unit and an element of R^{\times}, and 
we conclude that R^{\times} is a group.
#### $\ex$ – 
We have the following groups of units: 
• R^{\times} = R - {0} 
• Q\times = Q - {0} 
• C\times = C - {0}, 
• Z\times = {\pm1}. 
• \Z[i] \times = {\pm1, \pmi}. 
• R[x] \times = {non-zero constants}.
#### $\ex$ – 
#### $\lem$ – Order and Modular Exponents
![[Lemma – Order and Modular Exponents]]
#### $\ex$ – 
#### $\defn$ – Order (Element)
![[Order]]
#### $\lem$ – Order is Smallest Power
![[Lemma – $x^m = e to x big m$.]]

##### *Proof.*
It is clear that |g| \leq b since |g| is by definition the least positive exponent such 
that g|g| = 1. For divisibility, we observe that gb \mod |g| = 1 by Lemma 4.5.5, which 
contradicts that |g| was the smallest positive such exponent unless b \mod |g| = 0. 
A slightly more general version of the lemma is left to Exercise 4.41.
#### $\lem$ – All Orders Finite in Finite Group
In a finite group $G$, every element has finite order.

##### *Proof.*
Let g \in G and consider the sequence 
1, g, g2, g3, \dots 
Since G is both closed under the group operation and finite, this infinite list of 
elements of G can’t all be different, so there must be some gm = gn with m > n. 
Multiplying both sides by g-n gives gm-n = 1, so g has order at most m - n.
#### $\defn$ – Euler's Totient Function
![[Euler's Totient Function]]
#### $\lem$ – Totient Function and Distinct Primes
![[Lemma – Totient Function and Distinct Primes]]
#### $\thm$ – Decimal Expansions and $\Z/(n)$
![[Theorem – Decimal Expansions and $Z(n)$]]
## Lagrange’s Theorem & Euler's Totient Function
#### $\defn$ – Subgroup
![[Subgroup]]
#### $\ex$ – 
#### $\defn$ – Cyclic Group
![[Cyclic]]
#### $\thm$ – Generated Cyclic Group
Given a group $G$ and an element $g \in G$, the set of elements $g= \{g^{k} : k\in\Z\}$ 
forms a subgroup of $G$ called the cyclic subgroup generated by $g$

##### *Proof.*
Associativity in g is inherited from the larger group G, we have the identity 
g0 = 1 \in g, and we also have inverses since (gk )-1 = g-k. Finally, closure under 
multiplication follows from gm \cdot gn = gm+n.
#### $\ex$ – 
#### $\cor$ – Order of Cyclic Group
Suppose $g \in G$ has finite order. Then the order of the cyclic subgroup generated 
by $g$ is equal to the order of $g$ in $G$, i.e., $|g| = |g|$.

##### *Proof.*
#### $\defn$ – Congruent (Group)
Let $G$ be a group and $H$ a subgroup of $G$. For $a, b \in G$ we say a is (left) congruent 
to $b \mod H$ if $a\inv b \in H$ and write $a \equiv b \mod H$.
#### $\thm$ – Group Congruence
Given a group $G$ and a subgroup $H$, congruence $\mod H$ is an equivalence 
relation on the set $G$

##### *Proof.*
To check reflexivity, we have for all a \in G that a \equiv a \mod H since a-1a = e, 
and e \in H since H is a subgroup of G. For symmetry, suppose a \equiv b \mod H. Then 
a-1b \in H, and since H is closed under inverses, (a-1b)-1 = b-1a \in H, so b \equiv 
a \mod H. Finally, for transitivity, suppose that a \equiv b \mod H and b \equiv c \mod H. 
Then a-1b \in H and b-1c \in H, so their product a-1bb-1c = a-1c is also in H, 
giving a \equiv c \mod H.
#### $\defn$ – Coset
Given a group $G$ with element a and subgroup $H$, the set $a H = \{ah : h \in H \}$ is called the left coset of $H$ containing $a$
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\rem$ – 
#### $\lem$ – Cardinality and Cosets
Let $G$ be a finite group and $H$ a subgroup of $G$. Then for all $a \in G$, we have $|a H | = |H |.$ That is, all left cosets of $H$ have the same size as $H$.

##### *Proof.*
We show that the function f : H \to a H defined by f (h) = ah for all 
h \in H is a bijection. Since surjectivity follows for free from the definition of a H, 
we need only show injectivity. Suppose f (h1) = f (h2) for some h1, h2 in H. Thus 
ah1 = ah2. Multiplying both sides by a-1 on the left gives 
a-1(ah1) = a-1(ah2) 
(a-1a)h1 = (a-1a)h2 
h1 = h2, 
so f is injective, and hence a bijection, so |H | = |a H |.
#### $\thm$ – Lagrange's Theorem
![[Theorem – Lagrange's Theorem]]

##### *Proof.*
As the left cosets of H are the equivalence classes under congruence modulo 
H, by Lemma 4.1.5 they partition the set: 
G = a1 H \cup a^{2} H \cup \cdots \cup a k H, 
where a1 H, \dots, a k H represent the distinct, and therefore disjoint, cosets. It follows 
from the previous lemma that 
|G| = |a1 H | + |a^{2} H | + \cdots + |a k H | = |H | + |H | + \cdots + |H | = k|H |. 
Thus |H | divides |G|.
#### $\thm$ – Euler's Theorem
![[Theorem – Euler's Theorem]]
#### $\cor$ – Fermat's Little Theorem
![[Corollary – Fermat's Little Theorem]]
#### $\cor$ – Orders in $\Z/(n)$ and $\varphi(n)$
![[Corollary – Orders in $Z(n)$ and $varphi(n)$]]
#### $\cor$ – Modular Exponentiation
![[Corollary – Modular Exponentiation]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\cor$ – Cubes and $\Z/(p)$
![[Corollary – Cubes and Z(p)]]
#### $\thm$ – The Freshman's Dream
![[Theorem – The Freshman's Dream]]
#### $\rem$ – 
## Sunzi’s Remainder Theorem and $\varphi(n)$
#### $\lem$ – Varying Moduli
![[Lemma – Varying Moduli]]
#### $\thm$ – Cartesian Product is a Ring
![[Theorem – Cartesian Product is a Ring]]
#### $\ex$ – 
#### $\ex$ – 
#### $\thm$ – Sunzi's Remainder Theorem
![[Theorem – Sunzi's Remainder Theorem]]
#### $\rem$ – 
This theorem frequently goes by the name of The Chinese Remain- 
der Theorem, but it has been remarked that this is somewhat like referencing the 
Pythagorean Theorem as The Greek Triangle Theorem or Fermat’s Little Theo- 
rem as The French Power Postulate. In the interest of giving credit where credit is 
due, we include it here with the name of the 3rd-century Chinese mathematician, 
Sunzi, to whom the result is often attributed.
#### $\rem$ – 
An algebraic perspective on Sunzi’s Remainder Theorem is that 
when \gcd(m, n) = 1, the rings \Z/(mn) and \Z/(m) \times \Z/(n) are essentially “the 
same.” Namely, if every time someone mentioned \Z/(12) you secretly thought 
of the corresponding elements of \Z/(3) \times \Z/(4), no one would ever be the wiser. 
While we will not introduce the phrase as a term of art, the algebraic way of saying 
this is that the rings \Z/(mn) and \Z/(m) \times \Z/(n) are isomorphic (from the Greek: 
iso (same) and morph (form)), and the bijection that demonstrates this—in this case, the one described in Sunzi’s Remainder Theorem—is called an isomorphism 
from one ring to the other.
#### $\ex$ – 
#### $\cor$ – $\varphi$ Preserves Multiplication
![[Corollary – Totient Preserves Multiplication]]
#### $\rem$ – 
If f : Z \to Z is a function such that f (mn) = f (m) f (n) when- 
ever \gcd(m, n) = 1, we say that f is a multiplicative function. We have argued 
previously that the “number of divisors” function is multiplicative, and Corollary 4.7.9 provides \varphi as a second example. We will explore other multiplicative 
functions in the exercises
#### $\cor$ – Evaluating $\varphi(n)$
![[Corollary – Evaluating Totient Function]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
## Phis, Polynomials, and Primitive Roots
#### $\defn$ – Primitive Root
![[Primitive Root]]
#### $\ex$ – 
#### $\thm$ – Principal Counting Mechanism
![[Theorem – Principal Counting Mechanism]]
#### $\ex$ – 
#### $\thm$ – Primitive Root Theorem
![[Theorem – Primitive Root Theorem]]
# $\Z[i]$ of the Storm
## Gaussian Divisibility
#### $\defn$ – Divides
![[Divides]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\rem$ – 
A reasonable concern is that we now in principle have two different 
definitions of the symbol 3 | 6, depending on whether we parse it as “Does 3 
divide 6 in Z?” or “Does 3 divide 6 in \Z[i]?” Fortunately, the two questions are 
equivalent (see Exercises 5.17 and 5.18), so we need not be concerned\dots for now.
#### $\lem$ – Linear Combination Lemma (Gaussian)
![[Lemma – Linear Combination Lemma (Gaussian)]]
#### $\lem$ – Norms and Divisibility
![[Lemma – Norms and Divisibility]]
#### $\defn$ – Prime (Gaussian)
![[Prime]]
#### $\thm$ – Prime Norm Makes Prime
![[Theorem – Prime Norm Makes Prime]]
#### $\thm$ – Rational Prime and Sum of Squares
![[Theorem – Rational Prime and Sum of Squares]]
#### $\cor$ – Primes Congruent to 3 Mod 4
![[Corollary – Primes Congruent to 3 Mod 4]]
## Gaussian Modular Arithmetic
#### $\defn$ – Mod (Gaussian)
![[Mod#$ defn$ – Mod (Gaussian)]]
#### $\defn$ – Zn (Gaussian)
![[Z(n)#$ defn$ – $ Z[i]/( beta)$]]
## Gaussian Division Algorithm
#### $\thm$ – Gaussian Division Algorithm
#### $\thm$ – Gaussian Division Algorithm
If $\a, \beta \in\Z[i]$ with $\beta\neq 0$, then there exist Gaussian integers $\chi$ and $\rho$ with 
$0 \leq N (\rho ) < N (\beta )$ and $\a = \chi \beta + \rho$. Equivalently, for all $\beta \neq 0$, there exists a system of coset representatives $\mod \beta$ where each representative has norm less than $N (\beta )$.

##### *Proof.*
By analogy with the proof in Z, we define S = {\a - \chi \beta : 
\chi \in\Z[i]}, and let N = {N (z) : z \in S}. Note that N is a non-empty set of non- 
negative integers, so has a least element r by the Well-Ordering Principle. Thus we 
can write r = N (\rho ), where \rho \in S, and so there exists some \chi such that \rho = \a - \chi \beta, 
which implies \a = \chi \beta + \rho. Now, if N (\rho ) \geq N (\beta ), then the distance between \a and 
\chi \beta is at least the side length of the square fundamental domain for \beta. This implies 
that some vertex \chi \beta in that lattice is nearer to \a than is \chi \beta, which contradicts the 
minimality of r. Thus N (\rho ) < N (\beta ).
#### $\ex$ – 
## A Gausso-Euclidean Algorithm
#### $\lem$ – The Reduction Lemma (Gaussian)
![[Lemma – The Reduction Lemma (Gaussian)]]
#### $\thm$ – The Euclidean Algorithm for Gaussian Integers
![[Theorem – The Euclidean Algorithm for Gaussian Integers]]
#### $\ex$ – 
#### $\thm$ – Bézout’s Identity (Gaussian)
![[Theorem – Bézout’s Identity (Gaussian)]]
#### $\cor$ – Relatively Prime Int and Gauss
![[Corollary – Relatively Prime Int and Gauss]]
#### $\lem$ – Euclid's Lemma (Gaussian)
![[Lemma – Euclid's Lemma (Gaussian)]]
#### $\lem$ – Gaussian Prime Divisor Property
![[Lemma – Gaussian Prime Divisor Property]]
#### $\thm$ – Fundamental Theorem of Gaussian Arithmetic
![[Theorem – Fundamental Theorem of Gaussian Arithmetic]]
## Gaussian Primes and Prime Factorizations
#### $\thm$ – Fermat’s Two-Square Lemma
![[Theorem – Fermat’s Two-Square Lemma]]
#### $\thm$ – Lagrange’s Lemma
![[Theorem – Lagrange’s Lemma]]
#### $\lem$ – Primes and -1 Mod p
![[Lemma – Primes and -1 Mod p]]
#### $\thm$ – Equivalencies for Rational Primes
![[Theorem – Equivalencies for Rational Primes]]
#### $\lem$ – Gaussian Prime Divides Rational Prime
![[Lemma – Gaussian Prime Divides Rational Prime]]
#### $\thm$ – Classifying Gaussian Primes
![[Theorem – Classifying Gaussian Primes]]
#### $\ex$ – 
#### $\ex$ – 
#### $\defn$ – Valuation (Gaussian)
![[Valuation]]
#### $\ex$ – 
## Applications to Diophantine Equations
#### $\thm$ – Sum of Two Integer Squares
![[Theorem – Sum of Two Integer Squares]]
#### $\cor$ – Sum of Two Rational Squares
![[Corollary – Sum of Two Rational Squares]]
#### $\thm$ – Classification of Pythagorean Triples
![[Theorem – Classification of Pythagorean Triples]]
#### $\lem$ – Gaussian Power Lemma
![[Lemma – Gaussian Power Lemma]]
#### $\thm$ – Integer Cubes and Squares
![[Theorem – Integer Cubes and Squares]]
# From Where We $\R$ to Across the $\C$
## From -1 to -d
#### $\ex$ – 
#### $\ex$ – 
#### $\thm$ – The Fundamental Meta-Theorem of Arithmetic
![[Theorem – The Fundamental Meta-Theorem of Arithmetic]]
## Algebraic Numbers and Rings of Integers
#### $\defn$ – Algebraic Number
![[Algebraic Element]]
#### $\lem$ – MinPoly Unique
![[Lemma – MinPoly Unique]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\rem$ – 
#### $\ex$ – 
#### $\thm$ – Transcendental Decimal
![[Theorem – Transcendental Decimal]]
#### $\thm$ – e is Transcendental 
![[Theorem – e is Transcendental]]
#### $\thm$ – π is Transcendental 
![[Theorem – π is Transcendental]]
#### $\defn$ – Algebraic Integer
![[Algebraic Integer]]
#### $\thm$ – Algebraic Numbers is a Field
![[Theorem – Algebraic Numbers is a Field]]
#### $\rem$ – 
A principal theme of recent sections has been to extend Z by the 
adjoining of algebraic integers like i and √-2. Armed with the new ring Z, it 
is initially tempting to bypass such “small” extensions \Z[i] and Z[√-2] and try 
to work directly in Z. But it is worth noting that Z and Q really are quite exotic 
worlds to work in. For example, it is not hard to show that if \a \in\Z, then √\a \in\Z 
as well (Exercise 6.28), so the identity 
\a = √\a \cdot √\a = 4 
√\a \cdot 4 
√\a \cdot 4 
√\a \cdot 4 
√\a = \cdots 
shows that there are no prime elements at all in Z, and hence no notion of a prime 
factorization.
## Quadratic Fields: Integers, Norms, and Units
#### Pickle
Should 1 be considered square-free? If so, is it the unique square-free square? If 
not, why not? What about 0? Choose a side and pick a fight with someone on 
these very topics
#### $\defn$ – Quadratic Field
![[Quadratic Field]]
#### $\defn$ – Conjugate (Quadratic Field)
![[Conjugate (Quadratic Field)]]
#### $\defn$ – Ring of Integers
![[Ring of Integers]]
#### $\thm$ – Algebraic Integers in Quadratic Field
![[Theorem – Algebraic Integers in Quadratic Field]]
#### $\lem$ – Norms and Divisibility in Ring of Integers
![[Lemma – Norms and Divisibility in Ring of Integers]]
#### $\lem$ – Norms and Units
![[Lemma – Norms and Units]]
#### $\cor$ – Units in Integer Rings
![[Corollary – Units in Integer Rings]]
#### $\cor$ – Integer Ring and Infinite Units
![[Corollary – Integer Ring and Infinite Units]]
## Euclidean Domains
#### $\defn$ – Euclidean Domain
![[Euclidean Domain]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\defn$ – GCD (ED)
![[GCD]]
#### $\defn$ – Relatively Prime
![[Relatively Prime]]
#### $\lem$ – Norm of 0 is a Unit
![[Lemma – Norm of 0 is a Unit]]
#### $\thm$ – Bézout's Identity (ED)
![[Theorem – Bézout's Identity (ED)]]
#### $\defn$ – Prime
![[Prime]]
#### $\defn$ – Irreducible
![[Irreducible]]
#### $\lem$ – Norm and Irreducibility
![[Lemma – Norm and Irreducibility]]
#### $\lem$ – Prime is Irreducible in Integral Domain
![[Lemma – Prime is Irreducible in Integral Domain]]
#### $\thm$ – Euclid’s Lemma (ED)
![[Theorem – Euclid’s Lemma (ED)]]
#### $\cor$ – Prime Divisor Property (ED)
![[Corollary – Prime Divisor Property (ED)]]
## Unique Factorization Domains
#### $\defn$ – UFD
![[Unique Factorization Domain]]
#### $\thm$ – Prime iff Irreducible in UFD
![[Theorem – Prime iff Irreducible in UFD]]
#### $\thm$ – The Fundamental Meta-Theorem of Arithmetic
![[Theorem – The Fundamental Meta-Theorem of Arithmetic]]
#### $\lem$ – Norm and Units
![[Lemma – Norm and Units]]
#### $\lem$ – Norm and Divisors
![[Lemma – Norm and Divisors]]
#### $\rem$ – 
Since the notions of prime and irreducible are synonymous in UFDs, 
we can interchangeably speak either of unique prime factorizations or of unique 
factorizations into irreducibles
#### $\ex$ – 
## Euclidean Rings of Integers
#### $\thm$ – Z(√-2) an ED
![[Theorem – Z(√-2) an ED]]
#### $\ex$ – 
#### $\thm$ – Z(2) an ED
![[Theorem – Z(2) an ED]]
#### $\thm$ – Ring of Eisenstein Integers
![[Theorem – Ring of Eisenstein Integers]]
#### $\ex$ – 
#### $\ex$ – 
# Roots and Reciprocity
## Quadratic Residues and Legendre Symbols
#### $\defn$ – Quadratic Residue
![[Quadratic Residue]]
#### $\ex$ – 
#### $\defn$ – Legendre Symbol
![[Legendre Symbol]]
## Quadratic Residues and Non-Residues mod $p$
#### $\lem$ – Primitive Roots and Quadratic Residues
![[Lemma – Primitive Roots and Quadratic Residues]]
#### $\cor$ – Half of Elements of Z(p) are Square
![[Corollary – Half of Elements of Z(p) are Square]]
#### $\thm$ – Euler’s Criterion
![[Theorem – Euler’s Criterion]]
#### $\cor$ – Legendre Symbol of Products
![[Corollary – Legendre Symbol of Products]]
## Application: Counting Points on Curves
#### $\thm$ – Quadratics, Conics, Points
![[Theorem – Quadratics, Conics, Points]]
#### $\cor$ – Quadratics, Conics, Points (2)
![[Corollary – Quadratics, Conics, Points (2)]]
## The Quadratic Reciprocity Law: Statement and Use
#### $\thm$ – Quadratic Reciprocity, Supplemental Law 1
![[Theorem – Quadratic Reciprocity, Supplemental Law 1]]
#### $\thm$ – Quadratic Reciprocity, Supplemental Law 2
![[Theorem – Quadratic Reciprocity, Supplemental Law 2]]
#### $\thm$ – Quadratic Reciprocity
![[Theorem – Quadratic Reciprocity]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
## Some Unexpected Helpers: Roots of Unity
#### $\defn$ – Root of Unity
![[Root of Unity]]
#### $\defn$ – Cyclotomic Integers
![[Cyclotomic Integers]]
#### $\thm$ – Cyclotomic Integers are Algebraic Integers
![[Theorem – Cyclotomic Integers are Algebraic Integers]]
#### $\thm$ – Inverses and Roots of Unity
![[Theorem – Inverses and Roots of Unity]]
## A Proof of Quadratic Reciprocity
#### $\defn$ – Gauss Sum
![[Gauss Sum]]
#### $\ex$ – 
#### $\ex$ – 
#### $\thm$ – Squares of Gauss Sums
![[Theorem – Squares of Gauss Sums]]
#### $\cor$ – Gauss Sums and 3 mod 4
![[Corollary – Gauss Sums and 3 mod 4]]
#### $\thm$ – Quadratic Reciprocity Restated


##### *Proof.*
![[Theorem – Quadratic Reciprocity, Supplemental Law 2]]
#### $\ex$ – 
#### $\thm$ – Mod-$p$ Quadratic Formula
![[Theorem – Mod-$p$ Quadratic Formula]]
#### $\ex$ – 
## Quadratic UFDs
#### $\thm$ – Equivalencies for Rational Primes
![[Theorem – Equivalencies for Rational Primes]]
#### $\thm$ – Primes in Z√2
![[Theorem – Primes in Z√2]]
# Unleashed: Release $\Z_{p}$!
## The Analogy between Numbers and Polynomials
#### $\defn$ – Base Expansion
![[Base Expansion]]
#### $\lem$ – Valuations and Base Expansions
![[Lemma – Valuations and Base Expansions]]
## The $p$-adic World: An Analogy Extended
#### $\ex$ – 
#### $\defn$ – p-Adic Number
![[p-Adic Number]]
#### $\ex$ – 
#### $\ex$ – 
#### $\defn$ – Modular Reduction (2)
![[Modular Reduction]]
#### $\defn$ – Valuation (2)
![[Valuation]]
#### $\ex$ – 
## $p$-adic Arithmetic: Making a Ring
#### $\thm$ – p-Adic Integers is a Ring
![[Theorem – p-Adic Integers is a Ring]]
#### $\ex$ – 
#### $\defn$ – p-Adic Absolute Value
![[p-Adic Absolute Value]]
#### $\defn$ – p-Adic Arithmetic
![[p-Adic Arithmetic]]
#### $\lem$ – Properties of p-Adic Arithmetic
![[Lemma – Properties of p-Adic Arithmetic]]
## Which numbers are $p$-adic?
#### $\ex$ – 
#### $\lem$ – p-Adic Units
![[Lemma – p-Adic Units]]
#### $\rem$ – 
This again mirrors the situation in calculus. If f is a rational function 
with f (a)  = 0 (that is, the constant term of f ’s Taylor expansion at a is not zero), 
then 1 
f is also a rational function with a Taylor expansion at a. But if f (a) = 0, 
then 1 
f is not defined at a and so does not have a Taylor expansion there, and we 
must instead use a Laurent expansion.
#### $\cor$ – All p-Adic Elements Product of Unit and p
![[Corollary – All p-Adic Elements Product of Unit and p]]
#### $\cor$ – p-Adic Integers are a UFD
![[Corollary – p-Adic Integers are a UFD]]
#### $\rem$ – 
#### $\cor$ – Rationals Contained in p-Adic Rationals
![[Corollary – Rationals Contained in p-Adic Rationals]]
## Hensel’s Lemma
#### Claim
There is a square root of 7 in Q3 but not in Q5 or Q7.
#### $\rem$ – 
As with real numbers, we might encode the first claim as the ex- 
pression √7 \in\Q3, though in this case only while grimacing slightly internally. 
In R, the symbol √7 references “the unique positive real number whose square 
is 7.” In Q3, without an obvious notion of positiveness, the √7 then somewhat 
ambiguously refers to one of the two such elements. That will not stop us from 
occasionally employing this abuse of notation for visual or dramatic effect. Just 
don’t tell anyone.
#### $\thm$ – Hensel’s Lemma
![[Theorem – Hensel’s Lemma]]
#### $\rem$ – 
Lifting is a convenient verb for the act of taking an element of 
\Z/( p) and finding an appropriate element of Zp (or sometimes Z) that reduces 
to it \mod p. In this language, Hensel’s Lemma provides conditions under which 
we can lift a \Z/( p)-root of a polynomial f to a Zp-root.
#### $\rem$ – 
#### $\cor$ – Square Roots of p-Adic and Mod Integers
![[Corollary – Square Roots of p-Adic and Mod Integers]]
#### $\lem$ – Square Roots in 2-Adic Integers
![[Lemma – Square Roots in 2-Adic Integers]]
#### $\ex$ – 
#### $\cor$ – Squares in $\Q_{p}$
![[Corollary – Squares in $Q_{p}$]]
#### $\ex$ – 
#### $\rem$ – 
The argument can be repeated nearly verbatim for any prime p \equiv 
2 \mod 3 in place of 11. If p \equiv 1 (\mod 3), then there are three cube roots of unity 
\mod p and only a third of the elements of \Z/( p) will have cube roots. We would 
need a “cubic reciprocity law” to streamline results in the same way as we did in 
Example 8.5.8. Such laws exist but are beyond the scope of this book.
#### Pickle
Which roots of unity are in Zp?
## Local-Global Philosophy & the Infinite Prime
#### $\ex$ – 
## Local-Global Principle for Quadratic Equations
#### $\thm$ – Hasse’s Local-Global Principle
![[Theorem – Hasse’s Local-Global Principle]]
#### $\defn$ – Hilbert Symbol
![[Hilbert Symbol]]
#### $\rem$
#### $\ex$ – 
#### $\lem$ – Properties of the Hilbert Symbol
![[Lemma – Properties of the Hilbert Symbol]]
#### $\thm$ – Diophantine Equations & p-Adic Numbers 
![[Theorem – Diophantine Equations & p-Adic Numbers]]
#### Pickle
In Example 8.7.4 we found that (9, 15)p = +1 for all p. How do we go from this 
to, say, a Q7 -solution to 
9x^{2} + 15y^{2} = 1?
## Computations: Quadratic Equations Made Easy
#### $\thm$ – Diophantine Equations & p-Adic Numbers (2)
![[Theorem – Diophantine Equations & p-Adic Numbers (2)]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
#### $\thm$ – Hilbert Symbols Product Formula
![[Theorem – Hilbert Symbols Product Formula]]
#### $\cor$ – Hilbert Symbols and Primes
![[Corollary – Hilbert Symbols and Primes]]
#### $\ex$ – 
#### $\ex$ – 
#### $\ex$ – 
## Synthesis and Beyond: Moving Between Worlds
# The Adventure Continues
## Exploration: Fermat’s Last $\thm$ for Small $n$
#### $\thm$ – Fermat’s Last $\thm$
Let n > 2 be a natural number. Then there are no positive integer solutions to 
the equation 
x n + y n = z n.

##### *Proof.*
#### $\lem$ – Principle of Infinite Descent
If the existence of a natural number n that satisfies some set of properties automatically implies the existence of a smaller natural number n < n that also 
satisfies the properties, then there cannot exist any natural number satisfying the 
given properties.

##### *Proof.*
#### Prompt
#### Prompt
#### Prompt
#### $\thm$ – 


##### *Proof.*
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### $\thm$ – 


##### *Proof.*
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
#### Prompt
## Exploration: Lagrange’s Four-Square $\thm$ – 
$\thm$ – Lagrange’s Four-Square $\thm$ – 
Prompt
Prompt
Prompt
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
$\defn$ – 
Prompt
Prompt
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
$\ex$ – 
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
Prompt
$\defn$ – 
$\rem$ – 
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
## Exploration: Public Key Cryptography
Prompt
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
## Elliptic Curve Cryptography
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – Point Addition Formulas
Prompt
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
## Elliptic ElGamal Public Key Cryptosystem
$\rem$ – 
Prompt
Prompt
Prompt
## Exploration: Units of Real Quadratic Fields
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – Brahmagupta’s Composition Formula
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
Prompt
$\thm$ – Dirichlet’s Pigeonhole Principle
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
## Exploration: Ideals and Ideal Numbers
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\defn$ – 
Prompt
$\rem$ – 
Prompt
Prompt
Prompt
Prompt
$\rem$ – 
Prompt
$\defn$ – 
Prompt
Prompt
Prompt
$\defn$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – 
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
Prompt
$\thm$ – Baker-Heegner-Stark $\thm$ – 
Prompt
Prompt
Conjecture
Prompt