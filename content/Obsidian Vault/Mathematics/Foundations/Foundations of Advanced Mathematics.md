# Proofs
## Strategies for Proofs
### Direct Proofs
#### $\defn$ – Direct Proof
![[Direct Proof]]
#### $\defn$ – Even and Odd
![[Even and Odd]]
#### $\thm$ – Sums of Evens and Odds
![[Theorem – Sums of Evens and Odds]]
#### $\defn$ – Divisible
![[Divides]]
#### $\thm$ – Division is Transitive
![[Theorem – Division is Transitive]]
#### $\thm$ – Any Integer Divides Zero
![[Theorem – Any Integer Divides Zero]]
### Contradiction and Contrapositive
#### $\defn$ – Contrapositive
![[Contrapositive]]
#### $\thm$ – Odd Squares
![[Theorem – Odd Squares]]
#### $\defn$ – Contradiction
![[Contradiction]]
#### $\thm$ – Consecutive Pythagorean Triples
![[Theorem – Consecutive Pythagorean Triples]]
#### $\defn$ – Rational Number
![[Rational Numbers]]
#### $\defn$ – Square Root
![[Square Root]]
#### $\thm$ – Root 2 is Irrational
![[Theorem – Root 2 is Irrational]]
#### $\defn$ – Prime
![[Prime]]
#### $\thm$ – Infinite Primes
![[Mathematics/Foundations/Results/Theorem – Infinite Primes]]
### Cases, If and Only If
#### $\thm$ – $n^2+n$ is Even
![[Theorem – $n2+n$ is Even]]
#### $\thm$ – If Product is Irrational, so is a Factor
![[Theorem – If Product is Irrational, so is a Factor]]
#### $\thm$ – Mutual Divisibility
![[Theorem – Mutual Divisibility]]
#### $\thm$ – Odd Products
![[Theorem – Odd Products]]
### Quantifiers in Theorems
### Writing Mathematics
#### (a) A Written Proof Should Stand on Its Own
#### (b) Write Precisely and Carefully
#### (c) Prove What Is Appropriate
#### (d) Be Careful with Saying Things Are “Obvious”
#### (e) Use Full Sentences and Correct Grammar
#### (f) Use “=” Signs Properly
#### (g) Define All Symbols and Terms You Make Up
#### (h) Break Up a Long Proof into Steps
#### (i) Distinguish Formal vs. Informal Writing
#### (j) Miscellaneous Writing Tips
# Fundamentals
## Sets
### Basic Definitions
#### $\defn$ – Set
![[Set]]
#### $\defn$ – Element
![[Element]]
#### $\ex$ – Sets of Numbers
There are four sets of numbers that we will use regularly:
- The set of *natural* numbers, denoted $\N$;
- The set of *integers*, denoted $\Z$;
- The set of *rational* numbers, denoted $\Q$; and
- The set of *real* numbers, denoted $\R$.
#### $\ex$ – The Null Set
An extremely valuable set we will regularly encounter is the *empty* set (also called the *null* set) which is the set that does not have any elements in it. That is, the empty set is the set $\{ \}$. This set is denoted $\es$. It may seem strange to consider a set that doesn’t have anything in it, but the role of the empty set in set theory is somewhat  
analogous to the role of zero in arithmetic.
#### $\defn$ – Interval
![[Interval]]
#### $\defn$ – Subset
![[Subset]]
#### $\ex$
(a) Let $A = \{1, 2, 3, 4\}$ and $B = \{1, 3\}$. Then $B ⊆ A$ and $A \not\sse B$.
(b) Let $M$ be the set of all men, and let $T$ be the set of all proctologists. Then $T \not\sse M$ because not all proctologists are men, and $M \not\sse T$ because not all men are proctologists.
#### $\lem$ – Subsets
![[Lemma – Subsets]]
#### $\defn$ – Set Equality
![[Set Equality]]
#### $\ex$
(a) Let $A$ and $B$ be the sets in Example 3.2.3 (1). Then $B$ is a proper subset of $A$.
(b) Let $X = {a, b, c}$, and let $Y = {c, b, a}$. Then clearly $X ⊆ Y$ and $Y ⊆ X$, so $X = Y$.
(c) Let $$P = \{x ∈ \R | x^2 − 5x + 6 < 0\} \text{ and } Q = \{x ∈ \R | 2 < x < 3\}.$$We will show that $P = Q$, putting in more detail than is really necessary for a problem at this level of difficulty, but we want to make the proof strategy as explicit as possible.

First, we show that $P ⊆ Q$. Let $y ∈ P$. Then $y^2 −5y+6 < 0$. Hence $(y−2)(y−3) <  0$. It follows that either $y − 2 < 0$ and $y − 3 > 0$, or that $y − 2 > 0$ and $y − 3 < 0$. If $y−2 < 0$ and $y−3 > 0$, then $y < 2$ and $3 < y$; because there is no number that satisfies both these inequalities, then this case cannot occur. If $y − 2 > 0$ and $y − 3 < 0$, then $2 < y$ and $y < 3$. Hence $2 < y < 3$. It follows that $y ∈ Q$. Therefore $P ⊆ Q$.  

Next, we show that $Q ⊆ P$. Let $z ∈ Q$. Then $2 < z < 3$. Hence $2 < z$ and $z < 3$, and so $z − 2 > 0$ and $z − 3 < 0$. Therefore $(z − 2)(z − 3) < 0$, and therefore $z^2 − 5z + 6 < 0$. Hence $z ∈ P$. Therefore $Q ⊆ P$.  

By combining the previous two paragraphs we deduce that $P = Q$.
#### $\lem$ – Subset Equalities
![[Lemma – Subset Equalities]]
#### $\defn$ – Power Set
![[Power Set]]
#### $\ex$
(a) Because $/0 ⊆ /0$, then $P ( /0) = \{ /0\}$. In particular, we see that $P ( /0) 6 = /0$.
(b) Let $A = \{a, b, c\}$. Then the subsets of A are /0, {a}, {b}, {c}, {a, b}, {a, c}, {b, c} and {a, b, c}. The last of these subsets is not proper, but we need all subsets, not only the proper ones. Therefore
P (A) = { /0, {a}, {b}, {c}, {a, b}, {a, c}, {b, c}, {a, b, c}}

It can be seen intuitively that if A is a finite set with n elements, then P (A) is a finite set with 2n elements; by Part (1) of this exercise we see that this formula holds even when n = 0. This formula is proved in Theorem 7.7.10 (1).
### Set Operations
#### $\defn$ – Union
![[Union]]
#### $\defn$ – Intersection
![[Intersection]]
#### $\ex$
#### $\thm$ – Properties of Unions & Intersections
![[Theorem – Properties of Unions & Intersections]]
#### $\defn$ – Disjoint
![[Disjoint]]
#### $\ex$
#### $\defn$ – Set Difference
![[Set Difference]]
#### $\rem$
#### $\ex$
#### $\thm$ – Properties of Set Differences
![[Theorem – Properties of Set Differences]]
#### $\defn$ – Cartesian Product
![[Cartesian Product]]
#### $\ex$
#### $\ex$
#### $\thm$ – Properties of Cartesian Products
![[Theorem – Properties of Cartesian Products]]
#### $\ex$
### Families of Sets
#### $\ex$
#### $\defn$ – Family of Sets
![[Family of Sets]]
#### $\ex$
#### $\thm$ – Families of Sets
![[Theorem – Families of Sets]]
### Axioms for Set Theory
#### $\axiom{Axiom}$ – Extensionality
Let $x$ and $y$ be sets. If $x$ and $y$ have the same elements, then $x = y$.
#### $\axiom{Axiom}$ – Empty Set
There is a set $z$ such that $x\not\in z$ for all sets $x$.
#### $\axiom{Axiom}$ – Pairing
Let $x$ and $y$ be sets. There is a set $z$ such that $w \in z$ if and only if $w = x$ or $w = y$.
#### $\axiom{Axiom}$ – Union
Let $x$ be a set. There is a set $z$ such that $w \in z$ if and only if there is some $y \in x$ such that $w \in y$.
#### $\axiom{Axiom}$ – Power Set
Let $x$ be a set. There is a set $z$ such that $w \in z$ if and only if $w \sse x$.
#### $\axiom{Axiom}$ – Regularity
#### $\axiom{Axiom}$ – Selection
#### $\axiom{Axiom}$ – Infinity
#### $\axiom{Axiom}$ – Replacement
#### $\axiom{Axiom}$ – Choice
Let $x$ be a set. Suppose that if $y, w \in x$, then $y\neq\es$ and $y \cap w = \es$. Then there is a set $z$ such that if $y \in x$, then $y \cap z$ contains a single element.
#### $\defn$ – Pairwise Disjoint
![[Pairwise Disjoint]]
#### $\axiom{Axiom}$ – Choice for Pairwise Disjoint Sets (Family of Sets Version)
#### $\thm$ – Axiom of Choice (Family of Sets Version)
![[Theorem – Axiom of Choice (Family of Sets Version)]]
#### $\defn$ – Maximal Element
![[Maximal Element]]
#### $\ex$
#### $\thm$ – Zorn's Lemma
![[Mathematics/Foundations/Results/Theorem – Zorn's Lemma]]
## Functions
### Functions
#### $\defn$ – Function
![[Function]]
#### $\defn$ – Domain and Codomain
![[Domain and Codomain]]
#### $\ex$
#### $\defn$ – Canonical Map
![[Constant Map]]
#### $\defn$ – Identity Map
![[Identity Map]]
#### $\defn$ – Inclusion Map
![[Inclusion Map]]
#### $\defn$ – Restriction
![[Restriction]]
#### $\defn$ – Extension
![[Extension (Function)]]
#### $\defn$ – Projection Map
![[Projection Map]]
#### $\ex$
### Image and Inverse Image
#### $\defn$
![[Image]]
#### $\defn$
![[Preimage]]
#### $\ex$
#### $\ex$
#### $\thm$ – Properties of Image and Preimage
![[Theorem – Properties of Image and Preimage]]
### Composition and Inverse Functions
#### $\defn$
![[Function Composition]]
#### $\ex$
#### $\defn$
![[Coordinate Function]]
#### $\ex$
#### $\lem$ – Properties of Compositions
![[Lemma – Properties of Compositions]]
#### $\defn$
![[Function Inverse]]
#### $\lem$ – Properties of Function Inverses
![[Lemma – Properties of Function Inverses]]
#### $\ex$
### Injectivity, Surjectivity, Bijectivity
#### $\ex$
#### $\defn$
![[Injective]]
#### $\defn$
![[Surjective]]
#### $\defn$
![[Bijective]]
#### $\ex$
#### $\lem$ – Compositions and 'Jectivity
![[Lemma – Compositions and 'Jectivity]]
#### $\thm$ – Inverses and 'Jectivity
![[Theorem – Inverses and 'Jectivity]]
#### $\thm$ – Injective and Surjective Compositions
![[Theorem – Injective and Surjective Cancellation]]
## Relations
### Relations
#### $\defn$
![[Mathematics/Foundations/Definitions/Relation]]
#### $\ex$
#### $\defn$
![[Relation Class]]
#### $\ex$
#### $\defn$
![[Reflexive, Symmetric, Transitive]]
#### $\ex$
### Congruence
#### $\defn$
![[Congruent]]
#### $\ex$
#### $\lem$ – Mod is an Equivalence Relation
![[Lemma – Mod is an Equivalence Relation]]
#### $\thm$ – Modular Division Algorithm
![[Theorem – Modular Division Algorithm]]
#### $\cor$ – Integers and Remainders
![[Corollary – Integers and Remainders]]
#### $\cor$ – Integers are Even or Odd
![[Corollary – Integers are Even or Odd]]
#### $\thm$ – Partitioning the Integers
![[Theorem – Partitioning the Integers]]
#### $\defn$
![[Integers Modulo]]
#### $\ex$
#### $\lem$ – Modular Arithmetic
![[Lemma – Modular Arithmetic]]
#### $\cor$ – Mod and Relation Classes
![[Corollary – Mod and Relation Classes]]
#### $\lem$ – UMP for Modular Arithmetic
![[Lemma – UMP for Modular Arithmetic]]
#### $\lem$ – UMP is Operation Preserving
![[Lemma – UMP is Operation Preserving]]
### Equivalence Relation
#### $\defn$ – Equivalence Relation
![[Equivalence Relation]]
#### $\ex$
#### $\defn$ – Equivalence Class
![[Equivalence Class]]
#### $\thm$ – Equivalence Classes Partition
![[Theorem – Equivalence Classes Partition]]
#### $\cor$ – Similarity and Equivalence Class
![[Corollary – Similarity and Equivalence Class]]
#### $\defn$ – Quotient Set
![[Quotient Set]]
#### $\ex$
#### $\defn$ – Canonical Map
![[Canonical Map]]
#### $\lem$ – UMP for Equivalence Relations
![[Lemma – UMP for Equivalence Relations]]
#### $\defn$ – Partition
![[Partition]]
#### $\ex$
#### $\cor$ – Equivalence Relation Partitions
![[Corollary – Equivalence Relation Partitions]]
#### $\ex$
#### $\defn$ – $\phi$ and $\psi$
#### $\lem$ – Phi and Psi
![[Lemma – Phi and Psi]]
#### $\ex$
#### $\thm$ – Phi and Psi are Inverses
![[Theorem – Phi and Psi are Inverses]]
## Finite and Infinite Sets
### Properties of the Natural Numbers
#### $\axiom{Axiom}$ – Peano Postulates
#### $\defn$
![[Natural Numbers]]
#### $\thm$ – Definition by Recursion
![[Theorem – Definition by Recursion]]
#### $\thm$ – Properties of Natural Numbers
![[Theorem – Properties of Natural Numbers]]
#### $\thm$ – Well-Ordering Principle
![[Theorem – Well-Ordering Principle]]
### Mathematical Induction
#### $\thm$ – Mathematical Induction
![[Theorem – Mathematical Induction]]
#### $\prop$ – Induction (1)
![[Proposition – Induction (1)]]
#### $\prop$ – Induction (2)
![[Proposition – Induction (2)]]
#### $\ex$
#### $\ex$
#### $\thm$ – Mathematical Induction (Variant 1)
![[Theorem – Mathematical Induction (Variant 1)]]
#### $\prop$ – Induction (3)
![[Proposition – Induction (3)]]
#### $\thm$ – Mathematical Induction (Variant 2)
![[Theorem – Mathematical Induction (Variant 2)]]
#### $\thm$ – Mathematical Induction (Variant 3)
![[Theorem – Mathematical Induction (Variant 3)]]
#### $\thm$ – Prime Factorization
![[Theorem – Prime Factorization]]
#### $\thm$ – Functions and Natural Numbers
![[Theorem – Functions and Natural Numbers]]
### Recursion
#### $\thm$ – Definition by Recursion
![[Theorem – Definition by Recursion]]
#### $\ex$
#### $\thm$ – Natural Numbers and Products
![[Theorem – Natural Numbers and Products]]
#### $\ex$
#### $\thm$ – Natural Numbers and Products (2)
![[Theorem – Natural Numbers and Products (2)]]
#### $\prop$ – Fibonacci
![[Proposition – Fibonacci]]
#### $\thm$ – Natural Numbers and Products (3)
![[Theorem – Natural Numbers and Products (3)]]
### Cardinality of Sets
#### $\defn$ – Cardinality
![[Cardinality]]
#### $\lem$ – Cardinality is Equivalence Relation
![[Lemma – Cardinality is Equivalence Relation]]
#### $\ex$
#### $\defn$ – Finite Set
![[Finite Set]]
#### $\defn$ – Countably Infinite Set
![[Countably Infinite Set]]
#### $\lem$ – Natural Numbers are Infinite
![[Lemma – Natural Numbers are Infinite]]
#### $\ex$
#### $\thm$ – Cardinality of Power Set
![[Theorem – Cardinality of Power Set]]
#### $\cor$ – Power Set of Naturals Uncountable
![[Corollary – Power Set of Naturals Uncountable]]
#### $\thm$ – Schroeder–Bernstein Theorem
![[Theorem – Schroeder–Bernstein Theorem]]
#### $\lem$ – Cardinality and Injectivity
![[Lemma – Cardinality and Injectivity]]
#### $\ex$
#### $\thm$ – Trichotomy Law for Sets
![[Theorem – Trichotomy Law for Sets]]
### Finite and Countable Sets
#### $\lem$ – Equality of Natural Numbers
![[Lemma – Equality of Natural Numbers]]
#### $\cor$ – Finite Sets and Cardinality
![[Corollary – Finite Sets and Cardinality]]
#### $\thm$ – Subsets of Finite Sets
![[Theorem – Subsets of Finite Sets]]
#### $\cor$ – Infinite Subsets
![[Corollary – Infinite Subsets]]
#### $\thm$ – Countable Subsets are Countable
![[Theorem – Countable Subsets are Countable]]
#### $\thm$ – Countability and Functions
![[Theorem – Countability and Functions]]
#### $\thm$ – Countable Unions & Intersections
![[Theorem – Countable Unions & Intersections]]
#### $\thm$ – Countable Products
![[Theorem – Countable Products]]
#### $\thm$ – Proper Subsets and Finite Sets
![[Theorem – Proper Subsets and Finite Sets]]
### Cardinality of the Number Systems
#### $\thm$ – Rationals are Countable
![[Theorem – Rationals are Countable]]
#### $\thm$ – Algebraic Numbers are Countable
![[Theorem – Algebraic Numbers are Countable]]
#### $\thm$ – Real Numbers are Uncountable
![[Theorem – Real Numbers are Uncountable]]
#### $\thm$ – Irrationals are Uncountable
![[Theorem – Irrationals are Uncountable]]
#### $\thm$ – $|\R^n|=|\R|$
![[Theorem – Rn=R]]
#### $\ex$
# Extras
## Selected Topics
### Binary Operations
$\defn$ – Binary Operation
$\ex$
$\defn$ – Commutative Law
$\ex$
$\defn$ – Associative Law
$\ex$
$\defn$ – Identity Law
$\ex$
$\lem$
$\defn$ – Inverse Law
$\ex$
### Groups
$\defn$ – Group
$\defn$ – Abelian Group
$\ex$
$\lem$
$\thm$
$\defn$ – Subgroup
$\thm$
$\cor$
$\ex$
$\ex$
### Homomorphisms and Isomorphisms
$\defn$ – Homomorphism
$\ex$
$\thm$
$\thm$
$\defn$ – Kernel
$\ex$
$\thm$
$\defn$ – Isomorphism
$\thm$
### Partially Ordered Sets
$\defn$ – Antisymmetric
$\defn$ – Partial Ordering
$\defn$ – Total Ordering
$\ex$
$\defn$ – Cover
$\ex$
$\defn$ – Greatest and Least Element
$\ex$
$\defn$ – Maximal and Minimal Element
$\ex$
$\thm$
$\defn$ – Upper and Lower Bound
$\defn$ – Supremum and Infimum
$\ex$
$\lem$
$\thm$
$\ex$
$\defn$ – Order Homomorphism
$\lem$
$\ex$
$\thm$
### Lattices
$\defn$ – Join
$\defn$ – Meet
$\defn$ – Lattice
$\ex$
$\thm$
$\thm$
$\defn$ – Join and Meet Homomorphism
$\ex$
$\thm$
$\thm$
$\cor$
### Counting: Products and Sums
Fact – Product Rule
$\ex$
$\thm$
$\thm$
Fact – Sum Rule
$\ex$
$\thm$ – Sum Rule
$\ex$
$\thm$
$\cor$
$\ex$
$\cor$
### Counting: Permutations and Combinations
Fact – Counting Rules (Permutations)
$\defn$ – Permutation
$\ex$
$\thm$ – Counting Rules (Permutations)
Fact – Counting Rules (Combinations)
$\defn$ – Combination
$\ex$
$\defn$ – Notation
$\ex$
$\thm$ – Counting Rules (Combinations)
$\ex$
$\thm$
$\thm$
$\thm$ – Binomial $\thm$
$\thm$
### Limits of Sequences
## Explorations
### Greatest Common Divisors
$\defn$ – GCD
$\lem$
$\defn$ – Relatively Prime
$\prop$
$\thm$
$\thm$
### Real-Valued Functions
$\defn$ – Real Valued Function
$\defn$ – Sum
$\lem$
### Iterations of Functions
$\defn$ – Iteration
$\defn$ – Nilpotent Function
$\defn$ – Hidempotent Function
$\defn$ – Constantive Function

