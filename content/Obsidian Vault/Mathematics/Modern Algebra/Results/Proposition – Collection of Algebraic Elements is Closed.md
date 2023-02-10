#### $\prop$ – Collection of Algebraic Elements is Closed
Let[^1] $$\ov{\Q} := \{ z \in \C \mid z\text{ is algebraic over }\Q\}.$$ Then $\ov{\Q}$ is an [[Algebraic Closure|algebraic closure]] of $\Q$.

More generally, if $F \subseteq L$ is a [[Field|field]] [[Field Extension|extension]] and $L$ is [[Algebraically Closed|algebraically closed]], then the collection $\ov{F}$ of elements of $L$ that are algebraic over $F$ is an algebraic closure of $F$.

##### *Proof.*
It is far from clear that $\ov{F}$ is a subfield of $L$, and so we first prove that: Given $\a, \beta \in \ov{F}$, we have that $[F(\a): F]$ and $[F(\a, \beta): F(\a)]$ are finite and hence so is $[F(\a, \beta): F]$. Thus, every element of $F(\a, \beta)$ is algebraic over $F$; that is, $F(\a, \beta) \subseteq \ov{F}$. Since $F(\a, \beta)$ is a field, it follows that $\ov{F}$ contains $\a \pm \beta$,  $\a \cdot \beta$ and $\a^{-1}$ if $\a \ne 0$. This proves that $\ov{F}$ is indeed a subfield of $L$.

It is clear from the definition that $F \subseteq \ov{F}$ is an algebraic field extension. 

Given a non-constant $g(x) \in \ov{F}[x]$, let $\a$ be one of its roots in $L$ (which exists since we assume $L$ is algebraically closed). Then $\ov{F} \subseteq \ov{F}(\a)$ is an algebraic extension and hence so is $F \subseteq \ov{F}(\a)$ by Proposition \ref{prop:algebraictower}. This proves $\a \in \ov{F}$ and hence that $\ov{F}$ is algebraically closed.
***

[^1]: See: [[Algebraic Element|Algebraic]]