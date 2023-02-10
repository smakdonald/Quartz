#### $\thm$ – Factorizations, Permutations, and Associates
Assume $R$ is a [[Principal Ideal Domain|PID]] $r\in R$ is non zero and not a [[Unit|unit]] and $r = p_1 \cdots p_n = q_1 \cdots q_m$ are two different irreducible factorization of $r$. Then $n=m$ and there is a [[Permutation Group|permutation]] $\sigma$ such that, for all $i$, we have $p_i$ and $q_{\sigma(i)}$ are [[Associates|associates]].

###### *Proof.* 
Without loss of generality, assume $n \leq m$. We induct on $m$. 

If $m =1$ then $n=1$ as well since $n\leq m$ and $n=0$ would yield $r = p_1 \cdots p_n =1$, a contradiction. 
If $n=m=1$ we have $p_1=q_1$ and there is nothing more to prove. 

Assume $m > 1$ and that irreducible factorizations with $\leq m$ factors  are unique up to reordering factors and taking associates.

 Since $R$ is a PID, irreducible elements are prime by Theorem \ref{prop2-1}. Since $p_1 \cdots p_n\in (p_n)$ we have that $q_1 \cdots q_m\in (p_n)$ and since $(p_n)$ is a prime ideal it follows that 
$q_i \in (p_n)$ for some $i$. Upon reordering, we may as well assume $q_m\in (p_n)$. Thus $q_m = p_n u$ for some $u \in R$. Since $q_m$ is irreducible and $p_n$ is not a unit, $u$ must be a unit. We get
$$
p_1 \cdots p_n = q_1 \cdots q_{m-1} up_n
$$
and hence, since $R$ is an integral domain, we may divide by $p_n$ to
obtain
$$
p_1 \cdots p_{n-1}   = q_1 \cdots q_{m-2} (q_{m-1}u).
$$
Notice that $(q_{m-1}u)=(q_{m-1})$ is a prime ideal so $q_{m-1}u$ is irreducible by Theorem \ref{prop2-1}. 

By the inductive hypothesis we deduce that $n-1=m-1$ hence $n=m$ and also that $p_1, \ldots, p_{n-1}$ are associates to $q_1, \ldots, q_{m-2}, q_{m-1}u$ in some order. This together with $p_n$ associate to $q_m$ establishes the claim.
***