### Problem 3 – Group of Order 10976
Let G be a [[Group|group]] of [[Order|order]] $2^5\cdot 7^3$. Prove that $G$ is not [[Simple Group|simple]].

###### *Proof.*
By [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]] we know that $\Syl_7(G)\equiv 1\mod{7}$ and $\Syl_7(G)|2^5=32$. Thus our options are $1$ and $8$. Suppose that $\Syl_7(G)=8$. 

Let $G$ [[Group Action|act]] on $\Syl_7(G)$ by conjugation, yielding the [[Homomorphism|homomorphism]] $$\rho: G \to S_8$$via the [[Proposition – Permutation Representation|permutation representation]]. This map is non-trivial from part (2) of Sylow's Theorem, but $2^5\cdot 7^3$ does not divide $|S_8|=8!$, and thus $\rho$ cannot be injective. Then the [[Kernel|kernel]] of this homomorphism is non-trivial, [[Normal Subgroup|normal]] [[Subgroup|subgroup]] of $G$ (See: [[Corollary – Normal iff Kernel of Homomorphism|Result]]). Thus $G$ is not simple.
***
#qual