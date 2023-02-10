### Problem 2 – Odd Order and Conjugacy
Prove that if $G$ is a [[Order|finite]] [[Group|group]] of odd [[Order|order]], then for any non-identity element $x\in G$, $x$ is not [[Conjugacy Class|conjugate]] to $x\inv$.

##### *Proof.*
Let $G$ be a finite group of odd order, and let $G$ act on itself via conjugation. Under this action, the orbit of an element is exactly its conjugacy class. By the Orbit-Stabilizer Theorem we have $|G|=|\Orb(x)|\cdot|\Stab(x)|$. Thus the order of an element divides the order of the group, and so every orbit must have odd order.

Suppose there exists an element $x$ such that $gxg\inv=x\inv$ for some $g\in G$. Thus $x\inv\in\Orb(x)$. Let $y\in\Orb(x)$. Thus $y=hxh\inv$ for some $h\in G$. Then $y\inv=h\inv x\inv h$. However, as $x\inv=gxg\inv$, we have $y\inv=h\inv gxg\inv h$. As $h\inv g$ and $g\inv h$ are both in $G$, we see that $y\inv\in\Orb(x)$ as well. As $e\in\Stab(x)$, we see that this means that the orbit of $x$ would have even order, which is not possible.
***
#qual