#### $\lem$ – Multilinear Maps and Permutations
Assume  $\phi: V^{\times n} \to R$ is $R$-[[Multilinear and Alternating|multi-linear]] and [[Multilinear and Alternating|alternating]]. Then for any [[Permutation Group|permutation]] $\tau \in S_n$ and $v_1, \dots, v_n \in V$, we have $$\phi(v_1, \dots, v_n) = \sgn(\tau) \phi(v_{\tau(1)}, \dots, v_{\tau(n)})$$where $\sgn(\tau)$ is the sign of the permutation $\tau$.  

###### *Proof.* 
Let us first prove this in the case when $n = 2$ and $\tau$ is the only non-trivial element of $S_2$.  Say$$
  \psi: V^{\times 2} \to R
$$is $R$-multi-linear ($R$-bilinear) and alternating. The goal is to prove$$
\psi(v,w) = -\psi(w,v)$$for any $v,w$.

We have $$\psi(v+w, v+w) = 0$$on the one hand and $$\psi(v+w, v+w) = \psi(v, v+w) + \psi(w, v+w) = \psi(v,v) + \psi(v, w) + \psi(w,v) + \psi(w,w) = \psi(v, w) + \psi(w,v)  $$on the other hand. It follows that $$
  \psi(v, w) + \psi(w,v)  = 0
  $$which proves the Lemma in this case.

Now let $n$ be arbitrary and $\tau = (i \, j)$ for some $1 \leq i  < j \leq n$.   In this case we need to show$$
  \phi(v_1, \dots, v_n) = - \phi(v_1, \dots, v_{i-1}, v_{j}, v_{i+1}, v_{i+2}, \dots, v_{j-1}, v_i, v_{j+1}, \dots, v_n)
  $$for all $v_1, \dots, v_n \in V$.
Fix $n-2$ elements $v_1, \dots, v_{i-1}, v_{i+1}, \dots, v_{j-1}, v_{j+1}, \dots, v_n$ and define $$
  \psi: V^{\times 2} \to R
  $$by$$
\psi(v,w) = \phi(v_1, \dots, v_{i-1}, v, v_{i+1}, \dots, v_{j-1}, w,  v_{j+1}, \dots, v_n)
  $$for any $v,w \in V$.  With this notation the goal is to show $$\psi(v,w) = -\psi(w,v)$$Since $\phi$ is $R$-multi-linear and alternating, $\psi: V \times V\to R$ is $R$-bilinear  and alternating, and so the case already proven gives the result.

Finally let $n$ and $\tau$ be arbitrary. Then $\tau$ is a product of transpositions --- say $\tau = \tau_r \cdots \tau_1$ with each $\tau_i$ a transposition. Proceed by induction on $r$. The previous case establishes the result when $r = 1$. If $r \geq 2$, then using the previous case  gives
$$
\psi(v_\tau(1), \dots, v_\tau(n)) = -\psi(v_\tau'(1), \dots, v_\tau'(n))
$$
where $\tau' = \tau_{r-1} \cdots \tau_1$ and by induction $\psi(v_\tau'(1), \dots, v_\tau'(n)) = (-1)^{r-1}\psi(v_1, \dots, v_n)$. Hence
$$
\psi(v_\tau(1), \dots, v_\tau(n)) = (-1)^{r}\psi(v_1, \dots, v_n)
$$
which proves the result.
***