#### $\thm$ – Primitive Root Theorem
Let $p$ be [[Prime|prime]]. For a [[Divides|divisor]] $d$ of $p - 1$, the number of elements of [[Order|order]] $d$ in $\Z/( p)^{\times}$[^1] is $\varphi(d)$[^2]. In particular, there are $\varphi( p - 1)$ [[Primitive Root|primitive roots]] (so at least one!) [[Mod|modulo]] each prime $p$.

##### *Proof.*
Let d be a divisor of p - 1, let Td be the set of elements of \Z/( p)\times of order  
d. Since every element of \Z/( p)\times has order dividing p - 1 (Corollary 4.6.18), these  
sets partition \Z/( p)\times. The set Td is a subset of the elements x \in\Z/( p) satisfying  
x d = [1], and by Lemma 3.1.13, there are at most d such elements since \Z/( p)  
is an integral domain. If a is any element of Td , then since a has order d the set  
{a, a^{2}, \dots  , a d } consists of exactly d distinct elements of \Z/( p)\times that satisfy the  
equation x d = [1], so must represent all such solutions. This implies that Td must  
consist entirely of powers a k of a, and in particular the ones with order exactly d—  
those with \gcd(k, d) = 1 (Exercise 4.44). Since there are \varphi(d) of these, we conclude  
that |Td | is either 0 (if no such a existed) or \varphi(d) (if there is at least one such a). To  
deduce the statement of the theorem, we have left to show that |Td | is never zero, for  
which we employ Theorem 4.8.3: since the Td partition \Z/( p)\times and |Td | \leq  \varphi(d) for each d | n, the chain  
p - 1 = \sum   
d| p-1  
|Td | \leq  \sum   
d| p-1  
\varphi(d) = p - 1  
implies that each summand on the left of the middle inequality must in fact be equal  
to its corresponding summand on the right, and so |Td | = \varphi(d) for each d | n.

[^1]: Notation: [[Z(n)]], [[Group of Units]]
[^2]: Notation: [[Euler's Totient Function]]