#### $\lem$ – Quotient Map is Surjective Homomorphism
For any [[Group|group]] $G$ and [[Normal Subgroup|normal]] [[Subgroup|subgroup]] $N$ of $G$, the map $\pi:G \to G/N$[^1] defined by $\pi(g)=gN$ is a surjective group [[Homomorphism|homomorphism]] with [[Kernel|kernel]] $\ker(\pi)=N$. 

###### *Proof.* 
Let $gN\in G/N$[^2] and notice that $\pi(g)=gN$, making $\pi$ surjective. The group homomorphism property follows from the computation below which uses the definition of $\pi$ and the rule for multiplying cosets in $G/N$: $$\pi(gg')=(gg')N=gN\cdot g'N=\pi(g)\pi(g').$$Finally, using this [[Lemma – Equivalencies of Cosets|lemma]], we have $\ker(\pi)=\{g\in G\mid gN=e_GN\}=N$.
***

[^1]: See: [[Quotient Group]]
[^2]: See: [[Coset]]