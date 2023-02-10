#### $\thm$ – Spectrum Analogue of Strong Nullstellensatz
Let $R$ be a ring, and $I$ be an ideal. For $f\in R$,[^1]$$V(I) \subseteq V(f) \Longleftrightarrow f\in \sqrt{I}.$$Moreover[^2]$$\sqrt{I} = \bigcap_{P \in V(I)} P = \bigcap_{P \in \Min(I)} P.$$
##### *Proof.*
First to justify the equivalence of the two statements we observe: 
\[V(I) \subseteq V(f) \Longleftrightarrow f\in P \ \text{for all} \ P \in V(I)  \Longleftrightarrow f \in \bigcap_{P \in V(I)} P.\]
Now we will show that $\displaystyle\bigcap_{P \in V(I)} P = \sqrt{I}$:

$(\supseteq)$: It suffices to show that $P \supseteq I$ implies $P \supseteq \sqrt{I}$, and indeed 
$$f \in \sqrt{I} \implies f^n\in I \subseteq P \implies f\in P.$$

$(\subseteq)$: If $f\notin \sqrt{I}$, consider the multiplicatively closed set $W=\{1,f,f^2,f^3,\ldots\}$. We have $W\cap I=\varnothing$ by hypothesis. By \Cref{lemma spec strong nullstellensatz}, there is a prime $P$ in $V(I)$ that does not intersect $W$, and hence $P$ does not contain $f$.

Finally, $\Min(I) \subseteq V(I)$, and since by \Cref{lemma every prime contains minimal prime} every prime in $V(I)$ contains a minimal prime of $I$, we conclude that 
$$\bigcap_{P \in V(I)} P = \bigcap_{P \in \Min(I)} P.$$

[^1]: Notation: [[V(I)]], [[Radical Ideal]]
[^2]: Notation: [[Minimal Prime]]