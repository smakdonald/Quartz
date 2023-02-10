### Problem 3 – Centralizer, Normalizer, and Automorphism
Let $G$ be a [[Group|group]] and $H$ a [[Subgroup|subgroup]] of $G$. Recall that the [[Centralizer & Normalizer|centralizer]] of $H$  
in $G$ is $$C_H(G)=\{g\in G|gh=hg\text{ for all }h\in H\}$$Prove that if $H$ is [[Normal Subgroup|normal]] in $G$, then so is $C_G(H)$ and that $G/C_G(H)$[^1] is [[Isomorphism|isomorphic]] to a subgroup of the [[Automorphism|automorphism]] group of $H$.

###### *Proof.*
Let $G$ be a group and $H\nsg G$. Let $x\in C_H(G)$, and consider $gxg\inv$. Let $h\in H$. As $H\nsg G$ we have $h=gh'g\inv$ for some $h\in H$, and thus that
1. $g\inv h=h'g\inv$ and 
2. $hg=gh'$.
Consider $gxg\inv h$. By (1), we see $gxg\inv h=gxh'g\inv$. As $x$ commutes with everything in $H$ we have $gh'xg\inv$, and by (2) we have $hgxg\inv$. Thus $C_H(G)\nsg G$. 

Let $G$ act on the left cosets of $C_G(H)$ by left multiplication, giving rise to the permutation representation homomorphism $\rho:G/C_G(H)\to\Aut(H)$. By the First Isomorphism Theorem we see that $G/C_G(H)$ is isomorphic to a subgroup of the automorphism group of $H$.
***
#qual

[^1]: Notation: [[Quotient Group]]

### Problem 2 – Centralizer, Normalizer, and HK

Let $H$ be a [[Subgroup|subgroup]] of a [[Group|group]] $G$. Recall that the [[Centralizer & Normalizer|centralizer]] of $H$ is the subgroup of $G$ defined by $C_G(H) = \{g \in G | gh = hg ∀h \in H\}$ and the [[Centralizer & Normalizer|normalizer]] of $H$ is the subgroup of $G$ defined by $N_G(H) = \{g \in G | gHg\inv = H\}$.

(a) Show that the centralizer $C_G(H)$ of $H$ in $G$ is a [[Normal Subgroup|normal subgroup]] of the normalizer $N_G(H)$ of $H$ in $G$.
(b) Show that the [[Quotient Group|quotient]] $N_G(H)/C_G(H)$ is [[Isomorphism|isomorphic]] to a subgroup of the [[Automorphism|automorphism group]] $\Aut(H)$ of $H$.

##### *Proof.*
Let $H$ be a subgroup of a group $G$. 

###### Part (a)
Let $G$ act on $H$ by conjugation. Thus the associated permutation homomorphism $\rho$ is defined such that $\rho(g)=\phi_g$, where $\phi_g(h)=ghg\inv$. Notice that when $x\in C_G(H)$ we have $\phi_x(h)=xhx\inv=h$ for all $h\in H$, and thus $x\in\Ker(\rho)$. If $x\in\Ker(\rho)$ then $xhx\inv=h$ for all $h\in H$, and thus $x\in C_G(H)$. Thus $C_G(H)=\Ker(\rho)$ and $C_G(H)\nsg N_G(H)$. 
***
###### Part (b)
From the above permutation representation we have a homomorphism $\rho: G\to S_{|H|}\cong\Aut(H)$. As $C_G(H)=\ker(\rho)$, by the First Isomorphism Theorem we have $G/C_G(H)\cong\im(\rho))$, a subgroup of $\Aut(H)$. 
***
#qual

### Problem 1 – Centralizers and Normal Subgroups
Recall that the [[Centralizer & Normalizer|centralizer]] of a [[Subgroup|subgroup]] $H$ in a [[Group|group]] $G$ is $$C_G(H) = \{g ∈ G | gh = hg \text{ for all }h ∈ H\}.$$(a) Prove that if $H$ is [[Normal Subgroup|normal]] in $G$, then $C_G(H)$ is normal in $G$.
(b) Prove that if $H$ is normal in $G$, then $G/C_G(H)$ is [[Isomorphism|isomorphic]] to a subgroup of $\Aut(H)$ (the group of automorphisms of H)

##### *Proof.*
###### Part (a)
Let $G$ [[Group Action|act]] on $H$ by conjugation, yielding the [[Homomorphism|homomorphism]] $\rho$ via the [[Proposition – Permutation Representation|permutation representation]] that maps $g$ to $\s_g$, where $\s_g(h)=ghg\inv$. This is the trivial permutation exactly when $g\in C_G(H)$, making $C_G(H)$ the [[Kernel|kernel]] of $\rho$. Thus $C_G(H)$ is normal in $G$ (See: [[Corollary – Normal iff Kernel of Homomorphism|Result]]) 
***
###### Part (b)
From the above permutation representation we have a homomorphism $\rho: G\to S_{|H|}\cong\Aut(H)$. As $C_G(H)=\ker(\rho)$, by the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]] we have $G/C_G(H)\cong\im(\rho))$, a subgroup of $\Aut(H)$. 
***
#qual