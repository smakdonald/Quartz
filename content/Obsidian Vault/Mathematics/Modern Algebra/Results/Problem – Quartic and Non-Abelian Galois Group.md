### Problem 9 – Quartic and Non-Abelian Galois Group
Let $K$ be the [[Splitting Field|splitting field]] of $x^4-3$ over $\Q$
(a) Find a [[Basis and Free Module|basis]] for $K$ as a [[Vector Space|vector space]] over $\Q$.
(b) Show that $\Aut(K/Q)$[^1] is not [[Abelian Group|abelian]].

##### *Proof.*
Let $K$ be the splitting field of $f(x)=x^4-3$ over $\Q$

###### Part (a) 
First, note that $f$ is irreducible in $\Q[x]$ by Eisenstein's Criterion ($p=3$)
The roots of $f$ are 
- $\sqrt[4]3$,
- $\sqrt[4]3i$,
- $-\sqrt[4]3$, and
- $-\sqrt[4]3i$.
Let $F=\Q(\sqrt[4]3)$ and notice $[F:\Q]=4$. As $F\subseteq\R$ we see that $[F(i):F]=2$, and thus $[K:\Q]=8$, meaning our basis will have eight elements:
1. 1
2. $\sqrt[4]3$
3. $(\sqrt[4]3)^2$
4. $(\sqrt[4]3)^3$
5. $i$
6. $\sqrt[4]3i$
7. $(\sqrt[4]3)^2i$
8. $(\sqrt[4]3)^3i$
***
###### Part (b) 
Now that $K$ has been verified to be a splitting field, we see that $\Aut(K/Q)$ is isomorphic to a subgroup of $S_4$ of degree $8$. 

Any subgroup of $S_4$ of order $8$ is a Sylow $2$-subgroup. By Sylow’s theorems,  
the number of Sylow $2$-subgroups is either $1$ or $3$.

If there are three they are all conjugate, and conjugation induces an isomorphism on the group, we see that all three subgroups are isomorphic. 

Let $X$ be the set of left cosets of the subgroup $\{e,s\}$ of $D_8$. Note that $|X| = 4$. Let $G$ act on $X$ by left multiplication. This action induces a homomorphism $\varphi : G \to P(X)$ where $P(X)\cong S_4$ is the permutation group on $X$. As shown in class, the kernel of this homomorphism is the largest normal subgroup contained in $\{e,s\}$, which is $\{e\}$. Thus, $\varphi$ is injective and the image of $\varphi$ is a subgroup of $S_4$ isomorphic to $D_8$.
***
#qual

[^1]: Notation: [[Automorphism]]