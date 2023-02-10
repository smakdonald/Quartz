### Problem 1 – Group of Order 36
Prove that any group of order $36$ has a normal subgroup of order $3$ or $9$. 

##### *Proof.*
Let $G$ be a group of order $36=2^2\cdot 3^2$. 
By Sylow's Theorem we have $n_3|4$ and $n_3\equiv 1\mod{3}$, and thus $n_3=1,4$. If $n_3=1$ then the unique Sylow $3$-subgroup is normal, giving us a normal subgroup of order $9$. 

Suppose then that $n_3=4$,  let $P$ be one of the subgroups of order $9$, and let $G$ act on the cosets of $H$ by left multiplication giving rise to the permutation representation homomorphism $\rho:G\to S_4$. This is because there are $9$ elements in $P$, and thus there are $4$ left cosets by Lagrange's Theorem.

As $|S_4|=24<36=|G|$, we see that $\rho$ cannot be injective and thus $N=\Ker(\rho)$ is a non-trivial normal subgroup of $G$.

Recall that the action of $G$ on its cosets by left multiplication is always a transitive action, meaning there is exactly one orbit, $\Orb(sP)$ for some $sP\in G/P$, which must then have all $4$ elements of $G/P$ in it. By Orbit-Stabilizer, $|G|=|\Orb(sP)|\cdot|\Stab(sP)|$, and thus $|\Stab(s)|=9$. So there are $9$ elements in $G$ that fix $s$ for any $sP\in G/P$. 

Let $xP \in G/P$ and $g\in N$. Notice that $g\cdot xP=gxP$. As $g\in N$, We know that $\rho(g)$ yields the identity permutation, and thus that $gxP=xP$. 

Thus $N\subseteq\Stab(xP)$, which has order 9
***
#qual