### Problem 2 – Transitive Actions and Fixed Points
Let $G$ be a [[Group|group]] [[Group Action|acting]] [[Transitive Action|transitively]] on a set $S$. For $a\in S$, let $G_a = \{g\in G | ga = a\}$ be the stabilizer of $a$ under the action from $G$.

(a) Let $a, b\in S$. Prove there exists $g\in G$ such that $G_b = gG_ag\inv$.
(b) Suppose $S$ has more than one element and that $G$ is [[Order|finite]]. Prove that there exists $g\in G$ which has no fixed point, that is, for all $a\in S, ga\neq a$

##### *Proof.*
Let $G$ be a group acting transitively on a set $S$.

###### Part (a)
The action is transitive, so there exists some $g\in G$ such that $ga=b$. 

Let $x\in\Stab(a)$, consider $gxg\inv$b. Since $g\inv b=a$, we have $gxa$, $x$ stabilizes $a$ so now $ga$, but $ga=b$. So $g\Stab(a)g\inv\subseteq\Stab(b)$. 

Let $x\in\Stab(b)$. We know $xb=b$ and also $ga=b$, and so $xga=ga$. Applying $g\inv$ to both to see $g\inv xga=a$. This puts $g\inv xg\in\Stab(a)$. Thus $x\in g\Stab(a)g\inv$, completing the proof.
***
###### Part (b) 
The action is transitive, so there is only one orbit, and so $\Orb(a)=\Orb(b)=G$. Since $G$ is finite, the Orbit-Stabilizer Theorem tells us $|\Orb(a)|=|G|/|\Stab(a)|$. Since every orbit has the same order as $G$, we see $\Stab(a)=\{e\}$ for all $a\in S$. Thus there cannot exist any fixed points. 
***
#qual