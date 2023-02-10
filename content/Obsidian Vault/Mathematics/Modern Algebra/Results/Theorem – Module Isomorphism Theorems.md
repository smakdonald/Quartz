#### $\thm$ – Module Isomorphism Theorems
Let $R$ be a ring, and let $M$ be a $R$-module.\footnote{Recall that,
by default, "module'' means "left module''. But everything in this theorem is also true for right modules.} 
- (UMP for Quotient Modules) Let $N$ be a submodule of $M$, let $T$ be an $R$-module, and let $f: M \to T$ be an $R$-module homomorphism. If $f(M) = 0$ (i.e., if $N \subseteq \ker(f)$)  then the function $\ov{f}: M/N \to T$ given by $\ov{f}(m + N) = f(m)$ is a well-defined, $R$-module homomorphism. In fact, $\ov{f}: M/N \to T$ is the unique $R$-module homomorphism  such that $\ov{f}\circ \can = f$ where $\can$ denotes the canonical surjection $M \onto M/N$.  
- (First Isomorphism Theorem) Let $T$ be an $R$-module and let $h: M \to T$ be an $R$-module homomorphism. Then $\ker(h)$ is a submodule of $M$ and there is an $R$-module isomorphism $M/\ker(h) \cong \im(h)$ given by $m + \ker(h) \mapsto h(m)$. 
- (Second Isomorphism Theorem) Let $A$ and $B$ be submodules of $M$, and define $A + B = \{a+b \mid a \in A, b \in B\}$. Then $A + B$ is a submodule of $M$, $A \cap B$ is a submodule of $A$, and there is an $R$-module isomorphism $(A + B)/B \cong A/(A \cap B)$. 
- (Third Isomorphism Theorem) Let $A$ and $B$ be submodules of $M$ with $A \subseteq B$. Then $B/A$ is a submodule of $M/A$ and there is an $R$-module isomorphism $(M/A)/(B/A) \cong M/B$ given by sending $(m + A) + B/A$ to $m + B$. 
- (Lattice Isomorphism Theorem) Let $R$ be a ring, let $N$ be a R-submodule of $M$, and let $\pi: M \to M/N$ be the canonical quotient map. Then the function $$\Psi : \{R-\text{submodules of } M \text{ containing }N\} \to \{R-\text{submodules of }M/N\}$$defined by $\Psi(K) = K/N$ is a bijection, with inverse given by $\Psi^{-1}(T) = \pi^{-1}(T)$ for each $R$ submodule $T$ of $M/N$. Moreover, $\Psi$ and $\Psi^{-1}$ preserve sums and intersections.

###### *Proof.* 
Ignoring the rules for scaling by $R$, we know each of the frist four results holds for abelian groups (and the maps are the same). So, we merely 
need to prove that the rules for scaling are respected in each case. In more detail:

For the UMP, we already know that $\ov{f}$ is a well-defined homomorphism of groups under $+$ and that it is the unique one such that $\ov{f} \circ \can = f$.
It remains only to show $\ov{f}$ preserves scaling:
This follows quickly from the definitions:
$$
\ov{f}(r (m +N)) = \ov{f} (rm + N) = f(rm) = r f(m) = r \ov{f}(m + N).
$$
where the third equation uses that $f$ preserves scaling.

For the First Isomorphism Theorem, we already know 
that there is an isomorphism of abelian groups under $+$,
$$
\ov{h}: M/\ker(h) \xra{\cong} \im(h),
$$
given by $\ov{h}(m + \ker(h)) = h(m)$, and it remains only to show this map preserves scaling. This is a special case of what we proved in part (0).


For the second isomorphism theorem, we need to first check that $A+B$ and $A \cap B$ are submodules. From 817 we already know they are subgroups under $+$,
and it is evident from the definitions that each is closed under scaling by elements of $R$. 
Now, we know from 817 that there is an
isomorphism of abelian groups $h: A/(A \cap B) \xra{\cong} (A+B)/B$
given by $h(a + (A\cap B)) = a + B$. It remains only to show $h$
preserves scaling:
$$
h(r(a+(A \cap B))) = h(ra + A \cap B) = ra + B = r(a +B) = rh(a + (A \cap B)).
$$

For the third, we already know (from 817) that  $B/A$ is a subgroup of $M/A$ under $+$.
Given $r \in R$ and $b +A \in B/A$ we have $r(b+A) = rb + A$ which belongs
to $B/A$ since $rb \in B$. This proves $B/A$ is a submodule of $M/A$.
Also from 817 we know there is an isomorphism of abelian groups $h: (M/A)/(B/A) \to M/B$ given by $h((m+A) + B/A) = m + B$ and it remains only to show it is $R$-linear:
$h(r((m+A) + B/A)) =h(r(m+A) + B/A) = h((rm + A) + B/A) = rm   + B = r(m +B) = r h((m+A) + B/A)$.





The Lattice Theorem is the most complicaed to gerenlize. From 817 we know thre is a bijection between the set of sub groups of $M$ and that contain $N$
and subgroups of the quotient group $M/N$, and the maps are the same as given in the statment.
We just need to prove that these maps send submodules to submodules.
If $K$ is a submodule of $M$ containing $N$, then by part (3) we know $K/N$ is a submodule of $M/N$.
If $T$ is a submodule of $M/N$, then $\pi^{-1}(T)$ is an abelian group. For $r \in R$ adn $m \in \pi^{-1}(T)$ we have $\pi(m) \in T$
and hence $\pi(rm) = r\pi(m) \in T$ too, since $T$ is a submodule. This proves $\pi^{-1}(T)$ is a submodule.
***