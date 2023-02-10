#### $\thm$ – Main Theorem of Sylow Theory
Assume $G$ is a [[Group|group]] of order $p^e m$ where $p$ is prime, $e \geq 0$, and $\gcd(p,m) = 1$. 
1. $\Syl_p(G) \ne \emptyset$[^1] (there exists at least one [[Sylow p-Subgroup|Sylow]] $p$-[[Subgroup|subgroup]] of $G$).
2. If $P$ is a Sylow $p$-subgroup of $G$ and $Q \leq G$[^2] is any $p$-subgroup of $G$ (i.e., a subgroup whose [[Order|order]] is some power of $p$), then there is a $g$ such that $Q \leq gPg^{-1}$. In particular, the [[Group Action|action]] of $G$ on $\Syl_p(G)$ by conjugation is [[Transitive Action|transitive]] – i.e., any two Sylow $p$-subgroups are [[Conjugacy Class|conjugate]].
3. We have
$$| \Syl_p(G)| \equiv 1 \mod{p}.$$
4. For any $P \in \Syl_p(G)$[^3],  $$|\Syl_p(G)| = [G: N_G(P)],$$ and hence
$$|\Syl_p(G)| \mid m.$$

##### *Proof.* 
###### Part (1)
Recall that we write $|G| = p^em$ where $p \nmid m$.  We need to prove $G$ contains a subgroup of order $p^e$, and we proceed by induction on $|G|$. 

If $|G| = 1$ or, more generally, if $p \nmid |G|$, then  $\{e\}$ is a Sylow $p$-subgroup. We may thus assume $p \mid |G|$.
We proceed by considering two cases, depending on whether or not $p$ divides $|Z(G)|$. 

If $p \mid |Z(G)|$, then by Cauchy's Theorem, there is an element $z \in Z(G)$ of order $p$. Set $N = \langle z \rangle$. Since $z \in Z(G)$, we have $N \nsg G$. Since $|G/N| = p^{e-1}m$, by induction $G/N$ has a subgroup of order $p^{e-1}$ (i.e. of index $m$). By the Fourth Isomorphism Theorem, this subgroup corresponds to a subgroup of $G$ of index $m$, hence of order $p^e$.

For the second case, assume $p \nmid |Z(G)|$ and consider the class equation for $G$: $$|G| = |Z(G)| + \sum_{i=1}^k [G: C_G(g_i)]$$where $g_1, \dots, g_k$ are a complete and non-redundant list of non-central conjugacy class representatives. Since $p \nmid |Z(G)|$ and $p \mid |G|$, we must have $p \nmid [G:C_G(g_i)]$ for at least one $i$. For this $i$, we have $|C_G(g_i)|= p^e j$ where $p \nmid j$. Since $g_i$ is not central, $|C_G(g_i)| < |G|$ and hence, by induction, $C_G(g_i)$ contains a subgroup of order $p^e$. But this subgroup is also a subgroup of $G$.

###### Parts (2) and (3)
Let $P$ be a Sylow $p$-subgroup and let $Q$ be any $p$-subgroup. Let $\cS_P$ denote the collection of all conjugates of $P$: 
$$\cS_P = \{ gPg^{-1} \mid g \in G\}.$$
Part (3) tells us the $\cS_P$ consists of all Sylow $p$-subgroups of $G$, but we don't yet know this.
Nonetheless, $G$ acts (transitively) on $\cS_P$ by conjugation, and thus $Q$ also acts on $\cS_P$ (not necessarily transitively). The key to proving parts (2) and (3)  of the Sylow Theorem is to analyse the action of 
$Q$ on $\cS_P$ to establish \eqref{E1030} and \eqref{E1030b} below.

Let $O_1, \dots, O_s$ be the orbits of the action of $Q$ on $\cS_P$, and for each $i$ pick a representative $P_i \in O_i$. 
We have $$\Stab_Q(P_i) = \{q \in Q \mid qP_iq^{-1} = P_i\} = Q \cap N_G(P_i) = Q \cap P_i,$$where the last equation uses the Lemma. By LOIS, we thus have $|O_i| = [Q: Q \cap P_i]$ and hence $$\begin{equation}
|\cS_P |= \sum_{i=1}^s [Q: Q \cap P_i]
\end{equation}$$This equation holds for any $p$-subgroup $Q$ of $G$. In particular, we can take $Q = P_1$. In this case the first term is $1$ and, since $Q \cap P_i = P_1 \cap P_i <P_1 = Q$ for all $i \ne 1$, the remaining terms are divisible by $p$. This gives$$\begin{equation}|\cS_P| \equiv 1 \pmod{p}.\end{equation}$$(This does not yet prove part (3) since we don't yet know that $\cS_P$ consists of all Sylow $p$-subgroups.)

We can now prove part (2): By way of contradiction, suppose $Q$ is a $p$-subgroup of $G$ such that $Q$ is not contained in any of the subgroups belonging to $\cS_P$. Then $Q \cap P_i < Q$ for all $i$ and thus every term on the right-hand side of \eqref{E1030} is divisble by $p$, contrary to \eqref{E1030b}.
The second assertion in (2) follows by taking $Q$ to be a Sylow $p$-subgroup. 

This proves,  in particular, that $\cS_P$ in fact does consist of all Sylow $p$-subgroups. Part (3) thus follows from \eqref{E1030b}.

###### Part (4)
This is really immediate from the previous parts: For any $P \in \Syl_p(G)$, the stabilizer of $P$ for the action of $G$ on $\Syl_p(G)$ by conjugation is $N_G(P)$. Since we now know the action is transitive,
$$
|\Syl_p(G)| = [G: N_G(P)].
$$
Moreover, since $P \leq N_G(P)$ and $ |P| = p^e$, it follows that $[G: N_G(P)]\mid m$.
***

[^1]: See: [[Sylow p-Subgroup]]
[^2]: See: [[Subgroup]]
[^3]: See: [[Index]], [[Centralizer & Normalizer|Normalizer]]