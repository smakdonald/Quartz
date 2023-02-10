#### $\prop$ – Supp v Ann
Given $M$ a [[Module Finite|finitely generated]] $R$-module over a ring $R$,[^1] $$\Supp(M)=V(\ann_R(M)).$$ In particular, $\Supp(R/I)=V(I)$.

##### *Proof.*
Let $M= R m_i + \cdots + R m_n$. We have $$\ann_R(M)=\bigcap_{i=1}^n \ann_R(m_i),$$ so by \Cref{properties of V}, $$V(\ann_R(M))=\bigcup_{i=1}^n V( \ann_R(m_i)).$$ Notice that we need finiteness here.
Also, we claim that 
$$\Supp(M) = \bigcup_{i=1}^n \Supp(R m_i).$$
To show $(\supseteq)$, notice that $(R m_i)_P \subseteq M_P$, so
$$P \in \Supp(R m_i) \implies 0 \neq (R m_i)_P \subseteq M_P \implies P \in \Supp(M).$$
On the other hand, the images of $m_1, \ldots, m_n$ in $M_P$ generate $M_P$ for each $P$, and thus $P \in \Supp(M)$ if and only if $P \in \Supp(R m_i)$ for some $m_i$. Thus, we can reduce the equality $\Supp(M)=V(\ann_R(M))$ to the case of a cyclic module $R m$. By \Cref{lemma zero in localization}, $\frac{m}{1}=0$ in $M_P$ if and only if $(R\setminus P) \cap \ann_R (m) \neq \varnothing$, which is equivalent to $ \ann_R (m)  \not\subseteq P$.

[^1]: Notation: [[Support]], [[V(I)]], [[Annihilator]]