#### $\thm$ – Lagrange's Theorem
If $H$ is a [[Subgroup|subgroup]] of a [[Order|finite]] [[Group|group]] $G$, then $|H|$ divides $|G|$[^1].

###### *Proof.* 
Let $G$ be a finite group, suppose $H\leq G$, and let $H$ [[Group Action|act]] on $G$ by left multiplication. Let $h\in H$. By its definition, the [[Orbit|orbit]] of $h$ under this action is the set $$\Orb_H(g)=\{hg|h\in H\}.$$Notice that under this action, each of the orbits corresponds to a left [[Coset|coset]] of $H$ in $G$.  By Part (c) of this [[Lemma – $bigcap$s and $bigcup$s of Orbits|lemma]], $G$ is the union of pairwise disjoint orbits of this action. Thus  $|G|=\sum_{g\in G}|\Orb_H(g)|$ for distinct orbits. By this [[Lemma – Cosets Partition the Group|lemma]], all cosets have the same cardinality (the cardinality of $H$ itself), and thus each of the orbits in this relation have the same order, and thus we have $|G|=\sum_{g\in G}|H|$ for distinct orbits. Let $x$ denote the number of distinct orbits in this action. Thus we have $|G|=|H|\cdot x$. Hence $|H|$ divides $|G|$. #fix using vocab from later, should use group actions more instead
***
#### Corollary – $|x|\big| |G|$
If $x\in G$ and $G$ is a finite group, then $|x|$ divides $|G|$.

###### *Proof.* 
***

[^1]: Notation: $|G|$ denotes the order of the group $G$.