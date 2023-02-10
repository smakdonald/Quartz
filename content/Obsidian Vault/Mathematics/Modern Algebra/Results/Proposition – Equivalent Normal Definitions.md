#### $\prop$ – Equivalent Normal Definitions 
Let $N$ be a [[Subgroup|subgroup]] of a [[Group|group]] $G$. The following are equivalent: 
1. $N \norm G$[^1] 
2. $gNg^{-1}\subseteq N$ for all $g \in G$. 
3. $gN = Ng$[^2] for all $g \in G$.

###### *Proof.* 
Let's show the equivalence of 1. and 2. Assume $gNg^{-1} \subseteq N$ for all $g$. Let's show that $gNg^{-1} = N$ for all $g$. If $gNg^{-1} \subseteq N$ for all $g$, then for all $g$ we have $g^{-1}Ng \subseteq N$ and hence $$g(g^{-1}Ng) g^{-1} \subseteq gNg^{-1} \subseteq N$$holds. But $$g^{-1} (gNg^{-1}) g = \{g^{-1}ghg^{-1}g \mid h \in N\} = N,$$so $N \subseteq gNg^{-1} \subseteq N$ holds for all $g$.

As for the equivalence of 1. and 3., it follows from this chain of equivalences which use this [[Mathematics/Modern Algebra/Examples & Exercises|exercise]] #fix 
$$N\norm G\iff gNg^{-1}=N, \forall g\in G \iff gNg^{-1}g=Ng, \forall g\in G \iff gN=Ng, \forall g\in G .$$
***

[^1]: See: [[Normal Subgroup]]
[^2]: See: [[Coset]]