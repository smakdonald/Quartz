#### $\thm$ – $R$ a UFD iff $R[x]$ a UFD
For a [[Ring|ring]] $R$, $R$ is a [[Unique Factorization Domain|UFD]] if and only if $R[x]$[^1] is a UFD.

###### *Proof.* 
$(\Leftarrow)$ We note that an element $p$ of $R$ is irreducible in $R$ iff it is irreducible in $R[x]$ --- this holds by degree considerations. Moreover, $R[x]^\times = R^\times$. It follows pretty quickly from these facts that if $R[x]$ is a UFD,  then $R$ is a UFD, but we skip the details.

$(\Rightarrow)$ The other implication is more interesting. Assume $R$ is a UFD.

We first show factorizations exist. Let $f(x) \in R[x]$. Since $R$ is UFD, we may consider its content $c = \cont(f)$, so that $f(x) = c f'(x)$ with $f'(x)$ primitive. Now $c$ factors in $R$ into irreducibles and this remains an irreducible factorization of $c$ in $R[x]$. So it suffices to prove $f'(x)$ has an irreducible factorization too.

{\bf Claim:} Any primitive polynomial $f'(x)$ of positive degree in $R[x]$ factors as a product of primitive irreducible polynomials.

{\em Proof of claim:} If $f'(x)$ is irreducible, there is nothing to prove. Otherwise there is a non-trivial factorization $f'(x) = a(x) b(x)$,  and since $f'(x)$ is primitive,  we must have $\deg(a(x)) <\deg(f(x)), \deg(b(x)) <\deg(f(x))$. Moreover, by Lemma \ref{lem:content}, each of $a(x)$ and $b(x)$ must also be primitive. The existence of irreducible factorizations for primitive polynomials thus follows by induction on degree. 

For uniqueness, suppose we have two products of irreducible elements of $R[x]$ that are equal. Among the factors involved, we first write the constant factors and the the non-constant ones, getting an equation of the form
$$
d_1 \cdots d_m p_1(x) \cdots p_n(x) =
e_1 \cdots e_s q_1(x) \cdots q_t(x),
$$
where $d_i, e_j$ are irreducible elements of $R$ and $p_i, q_j$ are irreducible polynomials of degree at least one. Note that each of $p_i, q_j$ must be primitive  (since a non-primitive polynomial $p(x)$ factors as $\cont(p) p'(x)$).

By the Lemma, $p_1(x) \cdots p_n(x)$ and $q_1(x) \cdots q_t(x)$ are also primitive. It follows that
$d_1 \cdots d_m$ is the content of $d_1 \cdots d_m p_1(x) \cdots p_n(x)$ and $e_1 \cdots e_m$ is the content $e_1 \cdots e_s q_1(x) \cdots q_t(x)$. Since these are equal, $d_1 \cdots d_m$ and $e_1\cdots e_s$ agree up to a unit factor and hence, since $R$ is a UFD, we have $s = m$ and, after reordering, $d_i$ and $e_i$ are associates,  for all $i$.

We may now divide by $d_1 \dots, d_m$ to get that
$$
p_1(x) \cdots p_n(x) = u q_1(x) \cdots q_t(x)
$$
for some unit $u$ of $R$, and it remains to prove $n = t$ and, after
reordering, that $p_i$ and  $q_i$ are associates, for all $i$. Let $F$ be the field of fractions of $R$.  We know $F[x]$ is a Euclidean domain and hence it is a PID and hence a UFD. Moreover, by Gauss' Lemma, each $p_i, q_j$ remains irreducible in $F[x]$. Thus $n = t$ and, after reordering, $p_i(x)$ and $q_i(x)$ are associate in $F[x]$, for all $i$. This means that for each $i$ we have $p_i(x) = \frac{r_i}{s_i} q_i$, for some non-zero elements $r_i,s_i$ of $R$,   and hence $s_i p_i(x) = r_i q_i(x)$. But since $p_i, q_j$ are primitive, we have $s_i = \cont(s_i p_i(x))$ and  $r_i = \cont(r_i q_i(x))$. It follows that  $s_i$ and  $r_i$ are associates in $R$ and hence $p_i = u q_i$ for some unit $u$.
***

[^1]: See: [[Polynomial Ring]]