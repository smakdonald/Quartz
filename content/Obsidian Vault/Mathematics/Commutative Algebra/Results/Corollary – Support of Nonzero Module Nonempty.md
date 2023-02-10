#### $\cor$ – Support of Nonzero Module Nonempty
Let $R$ be a ring, $M$ an $R$-module, and $m\in M$. The following are equivalent:
(a) $M=0$.
(b) $M_P=0$ in $M_P$ for all $P \in \Spec(R)$[^1].
(c) $M_P=0$ in $M_P$ for all $P \in \mSpec(R)$.[^2]

##### *Proof.*
The implications $\Rightarrow$ are clear. To show $3) \Rightarrow 1)$, we show the contrapositive. If $m\neq 0$, consider $Rm \subseteq M$. By \Cref{nonzero element localizes}, there is a maximal ideal in $\Supp(Rm)$, and by \Cref{ses support} applied to the inclusion $Rm \subseteq M$, this maximal ideal is in $\Supp(M)$ as well.

[^1]: Notation: For $M_P$, see: [[Localization]]. For $\Spec$, see: [[Prime Spectrum]]
[^2]: Notation: [[Prime Spectrum]]