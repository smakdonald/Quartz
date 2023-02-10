### Problem 2 – June 2014 (3a)
Let $G$ be a group acting on a set $A$, and let $H$ be a subgroup of $G$ satisfying that the induced action of $H$ on $A$ is transitive (that is, for all a$, b\in A$ there is an $h\in H$ with $h\cdot a = b$). Let $t\in A$, and let $\Stab_G(t)$ be the stabilizer of $t$ in $G$. Show that $G = H\Stab_G(t)$.

##### *Proof.*
Let $G$ be a group acting on a set $A$, and let $H$ be a subgroup of $G$ satisfying that the induced action of $H$ on $A$ is transitive. Let $t\in A$, and let $\Stab_G(t)$ be the stabilizer of $t$ in $G$. 

Let $g\in G$. Note that $e\in\Stab_G(t)$ for all $t\in A$. If $g\in H$ then $g=ge$. Suppose then that $g\not\in H$. Suppose $gt=a$ for some $a\in A$. As $H$ acts transitively on $A$ there exists some $h$ such that $ht=a$. So $h\inv gt=a$, placing $h\inv g\in\Stab(t)$. Thus $g=h(h\inv g)$, so $G=H\Stab_G(t)$. 
***
#qual