#### $\thm$ – Fundamental Theorem of Galois Theory
Suppose $F \subseteq L$ is a ([[Degree of Field Extension|finite]]) [[Galois Extension|Galois]] [[Field|field]] [[Field Extension|extension]]. Then the functions[^1] 
$$\Psi:\left\{\text{intermediate fields $E$, with $F\subseteq E \subseteq L$}\right\} \to\left\{\text{subgroups $H$ of $\Gal(L/F)$}\right\}$$given by $$\Psi(E)=\Gal(L/E)$$is a bijection whose inverse $$\Psi^{-1}:
\left\{\text{subgroups $H$ of $\Gal(L/F)$}\right\} \to
\left\{\text{intermediate fields $E$, with $F \subseteq E \subseteq L$}\right\}$$is given by $$\Psi^{-1}(H)=L^H.$$ Moreover, this bijective correspondence enjoys the following properties:
1. $\Psi$ and $\Psi^{-1}$ each reverse the order of inclusions.
2. $\Psi$ and $\Psi^{-1}$ convert [[Degree of Field Extension|degrees]] of extensions to [[Index|indices]] of [[Subgroup|subgroups]]: 
	1. $[\Gal(L/F) : H] = [L^H:F]$ or, equivalently, 
	2. $[\Gal(L/F) : \Gal(L/E)] = [E:F]$.
3. Normal subgroups correspond to [[Intermediate Field|intermediate fields]] that are Galois over $F$:
	1. If $N \nsg G$ then $L^N/F$ is Galois.[^2]
	2. If $E/F$ is Galois, then $\Gal(L/E) \nsg \Gal(L/F)$.
4. If $E = L^N$ for a [[Normal Subgroup|normal]] subgroup $N \nsg \Gal(L/F)$, then $\Gal(E/F) \cong \Gal(L/F)/N$.
5. If $H_1, H_2$ are subgroups of $G$ with corresponding [[Fixed Subfields|fixed subfields]] $E_1=L^{H_1}$ and $E_2=L^{H_2}$, then 
	1. $E_1\cap E_2=L^{<H_1,H_2>}$ and $\Gal(L/E_1\cap E_2)=\langle H_1,H_2\rangle$
	2. $E_1 E_2=L^{H_1\cap H_2}$ and $\Gal(L/E_1E_2)=H_1\cap H_2$.

##### *Proof.*
***

[^1]: See: [[Intermediate Field]], [[Galois Extension|Galois Group]]
[^2]: See: [[Normal Subgroup]]