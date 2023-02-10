#### $\prop$ – Properties of V
Let $R$ be a ring, and $I_{\lambda},J$ be ideals, not necessarily proper.
(a) $V(R) = \varnothing$ and $V(0) = \Spec(R)$[^1].
(b) If $I \subseteq J$, then $V(J)\subseteq V(I)$.
(c) $V(I) \cup V(J) = V(I \cap J)=V(IJ)$.
(d) $\bigcap_{\lambda} V(I_{\lambda}) =V(\sum_{\lambda} I_{\lambda})$.

##### *Proof.*
Both $(0)$ and $(1)$ are straightforward, so we just prove $(2)$.

To see $V(I)\cup V(J) \subseteq V(I \cap J)$, just observe that if $P \supseteq I$ or $P \supseteq J$, then $P \supseteq I \cap J$.
Since $IJ \subseteq I \cap J$, we have $V(I \cap J) \subseteq V(IJ)$. To show $V(IJ) \subseteq V(I) \cup V(J)$, if $P$ is a prime and $P \notin V(I) \cup V(J)$, then $P \not\supseteq I, P \not\supseteq J$. Thus we can find $f \in I$, and $g \in J$ such that $f, g \notin P$. Since $P$ is prime, $fg \notin P$, while also $fg \in IJ$. Therefore, $P \nsubseteq IJ$.

To show $(3)$, since ideals are closed for sums, if $P \supseteq I_\lambda$ for all $\lambda$, then $P \supseteq \sum_{\lambda} I_{\lambda}$. Moreover, if $P \supseteq \sum_{\lambda} I_{\lambda}$, then in particular $P \supseteq I_\lambda$.

[^1]: Notation: [[V(I)]],  [[Prime Spectrum]]