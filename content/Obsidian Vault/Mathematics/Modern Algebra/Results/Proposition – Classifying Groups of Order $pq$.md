#### $\prop$ – Classifying Groups of Order $pq$ 
Let $p<q$ be primes.
1. If $p\nmid q-1$ there is a unique [[Group|group]] of [[Order|order]] $pq$ up to [[Isomorphism|isomorphism]], namely $C_{pq}$[^1].
2. If $p\mid q-1$ there are exactly two groups of order $pq$ up to isomorphism, namely $C_{pq}$ and a non-[[Abelian Group|abelian]] group.

###### *Proof.* 
Let $G$ be a group of order $pq$ and let $H, K$ be Sylow subgroups of order $q$ and $p$ respectively. We see that $H$ is a normal subgroup using a HW problem, since $[G:H]=p$ is the smallest prime that divides $|G|$.

Furthermore, since $H\cap K$ is a subgroup of both $H$ and $K$ we have by Lagrange's theorem that $|H\cap K|\mid \gcd(q,p)=1$, so that $H\cap K=\{e_G\}$. From here it follows that
\[
|HK|=\frac{|H||K|}{|H\cap K|}=\frac{q\cdot p}{1}=pq=|G|
\]
and so $HK=G$. The recognition theorem now yields that 
$$
G \cong H \sdp_\rho K \cong C_q\sdp_\rho C_p.
$$
for some homomorphism $\rho: K \to \Aut(H)$, equivalently $\rho: C_p \to \Aut(C_q)$.
By the UNM of cyclic groups to give such a homomorphism $\rho$ is equivalent to giving an element $z\in \Aut(C_q)$ so that $z^p=\id$, which will give $\rho(y^j)=z^j$ for $C_p=\langle y\rangle$. Thus $|z|\mid p$ yielding that either $|z|=1$ or $|z|=p$.

{\em Case 1:} if $|z|=1$ then $\rho$ is the trivial homomorphism and thus $G\cong C_q\times C_p\cong C_{pq}$.

{\em Case 2:} if $|z|=p$ then it must be the case by Lagrange that $p\mid |\Aut(C_q)$. By Lemma \ref{lem:Aut(C_p)} we know that $\Aut(C_q)\cong C_{p-1}$ is a cyclic group. Therefore we have that $p\mid (q-1)$ if and only if there exists an element $z\in \Aut(C_q)$ of order $p$ by Theorem \ref{thm:cyclic} (2) . Moreover any such element $z$ generates a subgroup of  $\Aut(C_q)$ of order $p$. Since there is a unique subgroup of a cyclic group of a given order by Theorem \ref{thm:cyclic} (2) we see that the image of $\rho$ is independent of the choice of $z$. Thus by Proposition \ref{prop:conjugateAut} we conclude that all subgroups resulting from any choice of $z$ of order $p$ are isomorphic.

Moreover, from the explicit presentation of semidirect products of cyclic groups given in a homework problem we see that the resulting group is non-abelian; in particular it is not isomorphic to $C_{pq}$.
***

[^1]: See: [[Cyclic]]