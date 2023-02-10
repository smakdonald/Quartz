#### $\lem$ – Module Finite Implies Algebra Finite
If $S$ is a [[Module Finite|module-finite]] $R$-[[Algebra|algebra]], then it is also [[Algebra Finite|algebra-finite]].[^1]

##### *Proof.*
Let $S = R f_1 + \cdots + R f_n$, meaning that $f_1, \ldots, f_n$ is a set of [[Generator#$ defn$ – Generated Submodule|module generators]] for $S$ over $R$. Note that every $R$-[[Linear Combination|linear combination]] of $f_1, \ldots, f_n$ is also an element of $R[f_1, \ldots, f_n]$, and thus $S$ is a subalgebra of $R[f_1, \ldots, f_n]$. On the other hand, since $f_1, \ldots, f_n \in S$ and $S$ is an $R$-algebra, every polynomial in $f_1, \ldots, f_n$ with coefficients in $R$ is also in $S$, and thus $S = R[f_1, \ldots, f_n]$, so that $S$ is algebra-finite over $R$.

[^1]: .$\rem$ The converse, however, is false: it is *harder* to be module-finite than algebra-finite.