#### $\lem$ – Nonzero Element Localizes
Let $R$ be a ring, $M$ an $R$-module, and $m\in M$. The following are equivalent:
(a) $m=0$ in $M$.
(b) $\frac{m}{1}=0$ in $M_P$ for all $P \in \Spec(R)$[^1].
(c) $\frac{m}{1}=0$ in $M_P$ for all $P \in \mSpec(R)$.

##### *Proof.*
The implications $1) \Rightarrow 2) \Rightarrow 3)$ are clear. To show $3) \Rightarrow 1)$, we prove the contrapositive. Given $m \neq 0$, its annihilator is a proper ideal, which must be contained in a maximal ideal by \Cref{every ideal is contained in a maximal ideal}. In particular, $V(\ann_R m)=\Supp(Rm)$ contains a maximal ideal, say $P$, so $\frac{m}{1} \neq 0$ in $M_P$.

[^1]: Notation: [[Localization]], [[Prime Spectrum]]