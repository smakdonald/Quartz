#### $\thm$ – The Lattice Isomorphism Theorem
Let $G$ be a [[Group|group]] and $N$ a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] with canonical [[Homomorphism|homomorphism]] $\pi:G\to G/N$. There is an containment-preserving bijection 
$$\Psi:
\{\text{subgroups of $G$ that contain $N$}\} \xra{\text{bijective}}
\{\text{subgroups of $G/N$}\}
$$
given by $\Psi(H)= H/N$[^1] for $N \leq H \leq G$[^2]. The inverse is defined for  $\cH \leq G/N$ by $$\Phi(\cH)=\pi^{-1}(\cH) = \{x \in G \mid \pi(x) \in \cH\}$$where $\pi: G \onto G/N$ is the quotient map. We denote $\Psi(H)=H/N=\ov H$. 
Then this bijection enjoys the following properties:
1. (normal) subgroups correspond to normal subgroups i.e., 
	1. $H\leq G$ iff $\ov H\leq \ov G$ and $\cH\leq \ov G$ iff $\Phi(\cH)\leq G$
	2. $H\norm G$ iff $\ov H\norm \ov G$ and $\cH\norm \ov G$ iff $\Phi(\cH)\norm G$
2. [[Index|indices]] are preserved; i.e.,  $[G:H] = [\ov G : \ov H]$ and $[G: \Phi(\cH)] = [\ov G : \cH]$.
3. the supremums and infimums are preserved (this makes $\Phi$ and $\Psi$ [[Poset and Lattice|lattice]] isomorphisms)
	1. $\ov{H} \cap \ov{K} = \ov{H \cap H}$  and $\langle \ov{H}\cup \ov{K} \rangle = \ov{\langle H\cup K \rangle}$[^3]
	2. $\Phi(\cH) \cap \Phi(\cK) = \Phi(\cH \cap \cK)$  and $\langle \Phi(\cH)\cup\Phi(\cK) \rangle = \Phi\left(\langle \cH\cup\cK \rangle\right)$

###### *Proof.* 
We have previously [[Lemma – Quotient Map is Surjective Homomorphism|shown]] that the quotient map $\pi:G\to G/N$ is a surjective group homomorphism. 
-  $\Psi$ is well defined (correct codomain) since for $H\leq G$ we have $\pi(H)\leq G/N$ (since images of subgroups through group homomorphisms are subgroups).
- $\Phi$ is well defined (correct codomain) since for $\cH\leq G$ we have $\pi^{-1}(\cH)\leq G$ (since preimages of subgroups through group homomorphisms are subgroups) and for any $\cH\leq G$ we have $\{e_GN\}\subseteq \cH$, hence[^4]$$N=\ker(\pi)=\pi^{-1}(\{e_GN\})\subseteq \pi^{-1}(\cH)=\Phi(\cH).$$
-  $\Phi$ and $\Psi$ are mutual inverses: $$(\Psi\circ\Phi)(\cH)=\pi(\pi^{-1}(\cH))=\cH$$since $\pi$ is surjective and $$(\Phi\circ\Psi)(H)=\pi^{-1}(\pi(H))=\pi^{-1}(H/N)=H,$$with the last equality justified by $$\begin{align*}x\in \pi^{-1}(H/N) &\iff \pi(x)\in H/N \iff xN=hN \text{ for some } h\in H \\& \iff x\in hN \text{ for some } h\in H \iff x\in H \text{ (using that } N\subseteq H).\\\end{align*}$$Thus, the two functions defined in the statement are well-defined and are mutually inverse. Since $\pi$ and $\pi^{-1}$ preserve containments, each of $\Psi$, $\Psi^{-1}$ preserves the order relation of containment.

I will only prove some parts of statements (1), (2), (3) in the theorem.

(1) If $N \leq H \leq G$ and $H \nsg G$, then $H/N \nsg G/N$ holds by part of the [[Theorem – Third Isomorphism Theorem|Third Isomorphism Theorem]] or by the exercise #fix below, since $\pi$ is surjective. The fact that the inverse function also sends normal subgroups to normal subgroups is a consequence of the statement that inverse images of normal subgroups are normal subgroups (see HW~4).  

(2) In the interest of time, I'll only prove the assertion about indices in the special case when $H$ is normal. In that case this fact is also an immediate consequence
of the Third Isomorhism Theorem since for $N \leq H \leq G$ with $H \nsg G$ we have
$$
[G:H] = |G/H| = \left|(G/N)/(H/N)\right| = [G/N: H/N]=[\ov G:\ov H].
$$
The general case is a consequence of an exercise from HW~5.

(3) The proof of (3) is omitted.

***

[^1]: See: [[Quotient Group]]
[^2]: See: [[Subgroup]]
[^3]: See: [[Generator]]
[^4]: See: [[Kernel]]

#### $\thm$ – Lattice Theorem for Quotient Rings
Suppose $R$ is a ring and $I$ is a two-sided ideal of $R$, and write $\pi: R \to R/I$ for the quotient ring homomorphism. There is a bijection
$$\Psi:\{\text{subrings of }R\text{ containing }I\}\to \{\text{subrings of }R/I\}, \Psi(S)=\pi(S)=S/I$$
with inverse 
$$\Phi:\{\text{subrings of }R/I\}\to\{\text{subrings of }R\text{ containing }I\}, \Phi(S)=\pi^{-1}(S).$$
Moreover this bijection induces a bijection between
$$\{\text{ideals of }R\text{ containing }I\}\leftrightarrow \{\text{ideals of }R/I\}$$
since $J$ is an ideal of $R$ containing $I$ if and only if  $\Psi(J)$ is an ideal of $R/I$.

###### *Proof.* 
***