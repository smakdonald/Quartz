#### $\prop$ – Characteristic and Prime Fields
Let F be a [[Field|field]]. 
1. The [[Mathematics/Modern Algebra/Definitions/Ring Characteristic|characteristic]] $\char(F)$ is either $0$ or a prime number $p$.
2. $\char(F) = 0$ if and only if the [[Prime Field|prime]] [[Subring|subfield]] of $F$ is [[Isomorphism|isomorphic]] to $\Q$; $\char(F) = p$ for a prime integer $p$ if and only if the prime subfield of $F$ is isomorphic to $\Z/p$.

##### *Proof.*
For the first assertion, consider the unique ring homomorphism $\varphi:\Z \to F$. Since $F$ is a domain, the kernel of $\varphi$ is a prime ideal (since $\Z/\ker(\varphi) \cong \im(\varphi)$ and $\im(\varphi)$ is a subring of $F$). The result holds since the only prime ideals of $\Z$ are $(0)$ and $(p)$ for a prime integer $p$. (Note that this proof shows that, more generally, the characteristic of an integral domain must be either $0$ or a prime.)

For the second assertion, observe that the smallest {\em sub-ring} of $F$ is the image of the ring map $\varphi: \Z \to F$, and by the first assertion, this image is isomorphic to either $\Z$ or $\Z/p$. The latter is already a field and hence it is the prime field of $F$.  In the former case, the prime subfield is isomorphic to the field of fractions of $\Z$, which is $\Q$.
***