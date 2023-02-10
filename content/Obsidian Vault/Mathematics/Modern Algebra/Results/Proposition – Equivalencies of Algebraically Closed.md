#### $\prop$ – Equivalencies of Algebraically Closed
The following are equivalent for a [[Field|field]] $L$:
1. $L$ is [[Algebraically Closed|algebraically closed]].
2. Every non-constant polynomial with coefficients in $L$ splits completely into (not necessarily distinct) linear factors.
3. There are no non-trivial algebraic extensions of $L$: If $L \subseteq E$ is an [[Algebraic Extension|algebraic]] field [[Field Extension|extension]] then $L = E$.

##### *Proof.*
(1) $\Rightarrow$ (2): Given a non-constant $f(x) \in L[x]$, by assumption $f$ has a root $a \in L$ and thus $f(x) = (x - a)g(x)$ with $g(x) \in L[x]$. But then $g$ also has a root and so it too factors, and so on.

(2) $\Rightarrow$ (3): Say $L \subseteq E$ is algebraic. Pick $\a \in E$. Then $\a$ is a root of some $f(x) \in F[x]$. But since $f$ factors completely, $\a \in L$.

(3) $\Rightarrow$ (1). Pick a non-constant $f(x) \in L[x]$. By Proposition \ref{prop:degreeF(a)}, there there is finite extension $L'$ of $L$ in which $f$ does have a root. By assumption $L = L'$ and so this root must be in $L$.
***