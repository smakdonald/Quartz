#### $\prop$ – Automorphisms and Permutations (Fields)
Suppose $F \subseteq K$ is a [[Field|field]] [[Field Extension|extension]] and $f(x) = F[x]$. Let $R = \{\a \in K \mid f(\a) = 0\}$, the set of roots of $f$ in $K$. 
1. For any $\a \in K$ and $\s \in \Aut(K/F)$[^1], we have $\s(f(\a)) = f(\s(\a))$. 
2. If $\a \in R$ then $\s(\a) \in R$ for all $\s \in \Aut(K/F)$.
3. The function $\phi: \Aut(K/F) \to \Perm(R)$[^2] given by $\phi(\s)(\a) = \s(\a)$ for $\a \in R$ is a [[Homomorphism|homomorphism]] of [[Group|groups]]. 
4. If $K= F(R)$[^3] then $\phi$ is one-to-one.
In particular, if $K$ is the [[Splitting Field|splitting]] field over $F$ of $f(x)$, then $\Aut(L/K)$ is [[Isomorphism|isomorphic]] to a [[Subgroup|subgroup]] of $S_n$ where $n$ is the number of roots of $f$ in $L$. (Note that $n \leq \deg(f)$[^4].) 

##### *Proof.*
Say $f = \sum_i c_i x^i$ with $c_i \in F$. Then $$\s(f(\a)) = \s \left(\sum_i c_i \a^i\right) = \sum_i \s(c_i) \s(\a)^i = \sum_i c_i \s(\a)^i = f(\s(\a)).$$This proves (1) and (2) is an immediate consequence.
  
To show (3) we need to first prove that for all $\s \in \Aut(K/F)$, the function $\phi(\s): R \to R$ is a bijection. (The target of this function is indeed $R$ by (2).)  Since $R$ is finite, we just need to show its one-to-one. This holds since $\s$ itself is one-to-one. (If $\phi(\s)(\a) = \phi(\s)(\a')$ for $\a, \a' \in R$ then $\s(\a) = \s(\a')$ and, since $\s$ is one-to-one, we have $\a = \a'$.) Since the group laws of $\Aut(K/F)$ and $\Perm(R)$ are both given as function composition, it is clear that $\phi$ is a group homomorphism. In detail, $$\phi(\s \circ \tau)(\a) = \s(\tau(\a)) = (\phi(\s)\circ \phi(\tau))(\a)$$ for all $\a$ and so $\phi(\s \circ \tau) = \phi(\s) \circ \phi(\tau)$.

Now asssume $K = F(R)$. We show $\phi$ is one-to-one by showing its kernel is trivial. Suppose $\phi(\s) = \id_{\Perm(R)}$; that is, suppose $\s(\a) = \a$ for all $\a \in R$. We show $\s = \id_K$. Define 
$$K^\sigma := \{\beta \in K \mid \s(\beta) = \beta\},$$
the so-called {\em fixed field} of $\s$. Note that $F \subseteq K^\s$ since $\s \in \Aut(K/F)$ and we also have $R \subseteq K^\s$ by assumption. It is easy to see that $K^\s$ is a subfield of $K$. (Here are the details: Clearly $1 \in K^\s$. For $\beta_1, \beta_2 \in K^\s$, we have $$
\s(\beta_1 \pm \beta_2) = \s(\beta_1) \pm \s(\beta_2)  = \beta_1 \pm \beta_2,$$$$\s(\beta_1 \cdot\beta_2) = \s(\beta_1) \cdot \s(\beta_2)  = \beta_1 \cdot \beta_2,$$and, if $\beta_2 \ne 0$, $$\s(1/\beta_2) =1 /\s(\beta_2)  =1/ \beta_2,$$
and thus $\beta_1 \pm \beta_2, \beta_1 \cdot \beta_2, 1/\beta_2 \in K^\s$.)  So, $K^\s$ is a subfield of $K$ that contains $F$ and $R$, but recall that $F(R)$ is the {\em smallest} subfield of $K$ that contains $F$ and  $R$, and so we must have $K^\s = K$. But then $\s(\a) = \a$ for all $\a \in K$ and hence $\s = \id_K$.

[^1]: See: [[Automorphism]]
[^2]: See: [[Permutation Group]]
[^3]: See: [[Field Extension]]
[^4]: See: [[Polynomial Degree]]