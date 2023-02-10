#### $\defn$ – Presentation of $R$-Module
Let $R$ be a non-zero [[Commutative Ring|commutative]] [[Ring|ring]], let $A \in \Mat_{m,n}(R)$, and let $T_A: R^n \to R^m$ be the $R$-[[Module|module]] [[Homomorphism|homomorphism]] [[Homomorphism Matrix|represented]] by $A$ with respect to the standard [[Basis and Free Module|bases]]; that is, define $T_A(v)=A \cdot v$. The  $R$-*module presented by* $A$ is the $R$-module $\coker(T_A) = R^m/\im(T_A)$.

Equivalently, the module presented by $A$ is $$\frac{R^m}{R v_1 + \cdots + R v_n}$$ where $v_1, \dots, v_n$ are the columns of $A$. 

If an $R$-module $M$ is [[Isomorphism|isomorphic]] to $\coker(T_A)$ for some (finite) matrix $A$, we say $M$ is *finitely presented*. 
***