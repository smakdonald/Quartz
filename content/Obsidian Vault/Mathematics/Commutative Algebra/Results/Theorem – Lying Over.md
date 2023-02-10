#### $\thm$ – Lying Over
If $R\subseteq S$ is an [[Integral Element|integral]] extension, then $P S \cap R = P$[^1] for every $P \in \Spec(R)$[^2], and the induced map $\Spec(S) \longrightarrow \Spec(R)$ is surjective.

##### *Proof.*
Let $I$ be any ideal in $R$. Given any $r \in \overline{I}$, we have$$r^n + a_1 r^{n-1} + \cdots + a_{n-1} r + a_n = 0$$for some $n$ and some $a_i \in I^i$ for all $i$, so$$r^n = - a_1 r^{n-1} - \cdots - a_{n-1} r - a_n \in I.$$Thus $\overline{I} \subseteq \sqrt{I}$.
Therefore, if $P$ is a prime in $R$, by \Cref{extension contraction for integral extensions} we have $P S \cap R \subseteq \overline{P}$, and$$P S \cap R \subseteq \overline{P} \subseteq \sqrt{P} = P.$$Then $P S \cap R = P$, and by \Cref{image criterion} we conclude that $P$ is in the image of the map on Spec.

[^1]: Notation: [[Contraction]]
[^2]: Notation: [[Prime Spectrum]]