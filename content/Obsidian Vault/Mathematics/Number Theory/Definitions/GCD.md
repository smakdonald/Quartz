#### $\defn$ – GCD (ED)
Given elements $a, b$, not both $0$, of a [[Euclidean Domain|Euclidean domain]] $R$ with Euclidean norm 
$N$, a $\gcd$ of $a$ and $b$ is an element $g \in\R$ such that:
- $g | a$[^1] and $g | b$; and
- If $d | a$ and $d | b$, then $N (d) \leq N (g)$.

[^1]: Notation: [[Divides]]

#### $\defn$ – GCD (Commutative Ring)
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] and let $a,b \in R$.
A *greatest common divisor*, or *gcd*, of $a$ and $b$ is an element $d \in R$ satisfying $d | a, d | b$, and whenever $d' | a$ and $d' | b$, then $d' | d$.

#### $\defn$ – LCM
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] and let $a,b \in R$.
A *least common multiple*, or *lcm*, of $a$ and $b$ is an element $m \in R$ satisfying $a | m, b | m$, and whenever $a | m'$ and $b | m'$ then $m | m'$.
***
#### $\defn$ – GCD (Matrix)
For a matrix $A$ with entries in a [[Principal Ideal Domain|PID]] $R$, let $\gcd_k(A)$ denote the [[GCD|gcd]] of all the $k \times k$ minors of $A$.