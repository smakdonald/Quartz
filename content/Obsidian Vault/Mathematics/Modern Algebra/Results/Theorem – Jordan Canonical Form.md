#### $\thm$ – Jordan Canonical Form
Let $F$ be a [[Field|field]], let $V$ be a [[Dim (Vector Space)|finite dimensional]] $F$-[[Vector Space|vector space]], and let $g: V \to V$ be a [[Linear Transformation|linear transformation]] satisfying the property that the [[Characteristic Polynomial|characteristic polynomial]] $\cp_g(x)$ of $g$ factors completely in $F[x]$[^1] into linear factors. Then there is an ordered [[Basis and Free Module|basis]] $B$ for $V$ such that[^3] 
$$[g]_B^B = J_{e_1}(r_1) \oplus \dots \oplus J_{e_s}(r_s)=
\begin{bmatrix}
J_{e_1}(r_1) & 0 & 0 & \cdots & 0 \\
0 &  J_{e_2}(r_2)  & 0 & \cdots & 0 \\
\vdots & \vdots & \ddots &  & \vdots \\
0 & 0 & \cdots & 0 &  J_{e_m}(r_m) \\
\end{bmatrix},
$$
where  $m$, the $e_i$'s, and the $r_i$'s are such that $(x - r_1)^{e_1}, \ldots, (x - r_m)^{e^m}$ are the [[Elementary Divisor|elementary divisors]] of the $F[x]$-[[Module|module]] $V_g$[^2]. Moreover, this matrix is unique up to ordering of the [[Jordan Block|Jordan blocks]], and it is known as "the'' *Jordan Canonical Form* of $g$. 

###### *Proof.* 
The proof is similar to the proof the RCF theorem, using the idea of Example \ref{ex45} above, but starting with the FTFGMPIDEDF (instead of the FTFGMPIDIFF). Here are the details:

We consider the $F[x]$-module $V_g$. Since we assume $\cp_g(x)$ factors completely, the only irreducible polynomials in its factorization are linear. Thus the invariant factors of $V_g$ are products of polynomials of the form $(x-r)^e$ for various $r \in F$ and integers $e \geq 1$. It follows that the elementary divisors have this  form too. The FTFGMPIDEDF therefore gives an isomorphism of $F[x]$-modules $$ V_g\cong \frac{F[x]}{(x - r_1)^{e_1}} \oplus \frac{F[x]}{(x -r_2)^{e_2}} \oplus \cdots \oplus\frac{F[x]}{(x - r_s)^{e_s}}. $$Now pick ordered bases $B_i=\{\ov{1}, \ov{x-r_i},  \ldots, \ov{(x-r_i)^{e_i-1}}\}$ for each of the summands and set $B$ to be their "ordered union''  just as we did for the proof of the Theorem on RCF. By the same argument as in Example \ref{ex45} applied to each summand individually, the matrix representing multiplication by $x$ on each summand is $J_{e_i}(r_i)$. This gives the existence of the JCF.

The uniqueness follows from the uniqueness clause in the FTFGMPIDEDF.
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Fx-Module V_g|Vg]]
[^3]: See: [[Homomorphism Matrix]], [[Jordan Block]], [[Block Diagonal Matrix]]