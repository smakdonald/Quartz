## Section I: Group theory
Solve two of the following three problems.  
### Problem 1 #unfinished 
Let $p$ be a prime and $H$ a finite $p$-group.

(a) Suppose $H$ acts on the finite set $S$, and let $S_0$ be the fixed points of the action, i.e.,
$$S_0 = \{x \in S | hx = x \text{ for all }h \in H\}.$$Prove that $|S| \equiv |S_0|\mod{p}$.
(b) Suppose $G$ is a finite group and $H \leq G$ (where $H$ is still a finite $p$-group). Prove that  $[N_G(H) : H]\equiv[G : H]\mod{p}).$

##### *Proof.*
Let $p$ be a prime and $H$ a finite $p$-group.
###### Part (a)
Suppose $H$ acts on the finite set $S$, and let $S_0$ be the fixed points of the action. Let $x\in S_0$, and note that $\Stab_H(x)=H$. By Orbit-Stabilizer we see $|\Orb_H(x)|=1$. 

The orbits of an action partition the set $S$, and as orbits are either disjoint or equal, we see $|S|=\sum\limits_{x\in S}|\Orb_H(s)|$. 
***
###### Part (b)
***
### Problem 2 #unfinished 
A normal subgroup $H$ of $G$ is called a *direct factor* of $G$ if there is some normal subgroup $K$ of $G$ such that $G = H \times K$ (internal direct product).

(a) If $H$ is a direct factor of $G$, $L$ is any group, and $\phi : H \to L$ is any group homomorphism, prove that $\phi$ extends to a homomorphism $\widetilde{\phi} : G \to L$ such that $\widetilde\phi(h) = \phi(h)$ for all $h \in H$.
(b) Provide a counter-example (with justification) to the previous part if $H$ is assumed  
to be a normal subgroup of $G$, but not a direct factor. Hint: One such example involves $G = \Z$.

##### *Proof.*
##### Part (a)
Let $L$ be a group, $H$ be a direct factor of $G$, and $\phi : H \to L$ a group homomorphism. As $H$ is a direct factor of $G$, there exists some $K\nsg G$ such that $G=H\times K$. Thus there exists some isomorphism $\psi:G\to H\times K$. Define $\widetilde{\phi} : G \to L$ such that $\widetilde{\phi}(g)=h$, where $\psi(g)=(h,k)$. 
Let $x,y\in G$, and notice $$\psi(x)=(h,k)\psi(y)=(h',k')=(hh',kk')=\psi(xy),$$ as $\psi$ is an isomorphism. 
Observe $\widetilde{\phi}(xy)=hh'=\widetilde{\phi}(x)\widetilde{\phi}(y)$. Thus $\widetilde{\phi}$ is a homomorphism, and for any $h\in H$ we have $\widetilde{\phi}(h)=h$. 
***
###### Part (b)

***
### Problem 3 – Group of Order 18515 Abelian
[[Problem – Group of Order 18515 Abelian]]
## Section II: Field Theory and Galois Theory
Solve two of the following three problems.  
### Problem 4 – Positive Quartic and Basis
[[Problem – Positive Quartic and Basis]]
### Problem 5 – January 2014 (4a)
[[Problem – January 2014 (4a)]]
### Problem 6 #unfinished 
Let $L$ be a finite Galois field extension of $\Q$. Let $E$ and $F$ be subfields of $L$ such that $EF = L, E/\Q$ is normal, and $E\cap F = \Q$. Prove that $[L : Q] = [E : Q][F : Q].$

##### *Proof*.

***
## Section III: Ring theory and Linear Algebra
Solve two of the following three problems.
### Problem 7 – Diagonalizable if MinPoly Splits
[[Problem – Diagonalizable if MinPoly Splits]]
### Problem 8 #unfinished 
Prove the ideal $I = (2, 1 + \sqrt{-13})$ of the commutative ring $R = \Z[\sqrt{-13}]$ is not a principal ideal.

##### *Proof*.
Define norm function, yada yada
***
### Problem 9 #unfinished 
Let $I$ be an ideal in a commutative ring $R$, let $M$ and $N$ be $R$-modules and let $f : M \to N$ be an $R$-module homomorphism.

(a) Prove there is a unique $R$-module homomorphism $\ov{f} : M/IM \to N/IN$ such that $\ov{f} \circ p = q \circ f$, where $p : M\to M/IM$ and $q : N\to N/IN$ are the canonical quotient maps
(b) Prove that if $I^2 = 0$ and $\ov{f}$ is surjective, then so is $f$ . (Recall that $I^2$ is the ideal  
generated by all elements of the form $ab$, where $a, b \in I$.)

##### *Proof.*
###### Part (a) 
***
###### Part (b) 
***