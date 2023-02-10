#### $\lem$ – Mod-Fin-Compose
If $R\subseteq S$ is [[Module Finite|module-finite]] and $N$ is a [[Finitely Generated Module|finitely generated]] $S$-module, then $N$ is a finitely generated $R$-module by [[Proposition – Restriction of Scalars|restriction of scalars]]. In particular, the composition of two module-finite ring maps is module-finite.

##### *Proof.*
Let $S = R a_1 + \cdots + R a_r$ and $N = S b_1 + \cdots + S b_s$[^1]. Then we claim $$N=\sum_{i=1}^{r}\sum_{j=1}^{s} R a_i b_j.$$ Indeed, given $n = \sum_{j=1}^{s} s_j b_j$,[^2] rewrite each $s_j=\sum_{i=1}^{r} r_{ij} a_{i}$[^3] and substitute to get 
$$n=\sum_{i=1}^{r}\sum_{j=1}^{s} r_{ij} a_i b_j$$
as an $R$-[[Linear Combination|linear combination]] of the $a_i b_j$.[^4]

[^1]: This [[Lemma – Mod Finite and Algebra Finite Expressions|Lemma]] lets us write $S = R a_1 + \cdots + R a_r$, as $S$ is module-finite over $R$. We are really saying that $\{b_{1},\dots,b_{s}\}$ is the finite [[Generator#$ defn$ – Generated Submodule|generating set]] for $N$ in $S$, which lets us write $N = S b_1 + \cdots + S b_s$. Note that all $a_{i}$ and $b_{i}$ are contained in $R$. 
[^2]: Structure: Here we are taking an arbitrary element in $N$ and showing that it can be expressed as an $R$-linear combination of elements. 
[^3]: We can do this because $S = R a_1 + \cdots + R a_r$, so every element of $S$ can be written as a $R$-linear combination of elements in $\{b_{1},\dots,b_{n}\}$. This is the restriction of scalars. 
[^4]: This [[Lemma – Generated Module Equivalencies|Lemma]] allows us to complete the proof, as every element of $N$ can now be expressed as a linear combination of elements in $R$. The set $\{a_1,\dots,a_{r},b_{1},\dots,b_{s}\}$ generates $N$ as a module, making $N$ finitely generated.