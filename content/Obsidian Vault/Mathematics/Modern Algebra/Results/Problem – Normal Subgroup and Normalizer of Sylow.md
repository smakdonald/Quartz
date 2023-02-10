### Problem 3 – Normal Subgroup and Normalizer of Sylow
Let $H$ be a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] of a [[Order|finite]] [[Group|group]] $G$, $p$ a prime dividing the [[Order|order]] of $H$, and $P$ a [[Sylow p-Subgroup|Sylow]] $p$-subgroup of $H$. Prove that $G = H N_G(P )$ (See: [[Centralizer & Normalizer|Normalizer]], [[HK]]).  
*Hint*: For g ∈ G, consider the subgroup $gPg\inv$.

##### *Proof.*
First, note that $N_G(P)=\{g\in G|gPg\inv=P\}$. 

Let $G$ [[Group Action|act]] on $\Syl_p(G)$ by conjugation, which is a [[Transitive Action|transitive]] action by part (2) of [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]]. Therefore $H$ acts transitively on this set as well. Under this action, $N_G(P)=\Stab_G(P)$. 

Let $g\in G$, and let $x\in N_G(P)$. Consider $g\inv x$. As the action by $H$ is transitive there exists some $h\in H$ such that $hg\inv\cdot x=x$. This means that $hg\inv$ stabilizes $x$. Then $(hg\inv)\inv=gh\inv$ stabilizes $x$ as well, so $gh\inv\cdot x=x$. But notice that $gh\inv h=g$, where $gh\inv\in N_G(P)$ and $h\in H$. Thus $G = H N_G(P )$.
***
#qual