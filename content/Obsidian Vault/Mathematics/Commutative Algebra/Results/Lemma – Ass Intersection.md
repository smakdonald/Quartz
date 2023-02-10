#### $\lem$ – Ass Intersection
If $I_1,\dots,I_t$ are ideals, then[^1] $$\Ass \left( R/ \bigcap_{j=1}^t I_j \right) \subseteq \bigcup_{j=i}^t \Ass(R/I_j).$$ 
##### *Proof.*
The canonical map $R \to R/I_1 \oplus R/I_2$ sending $r \mapsto (r+I_1, r+I_2)$ has kernel $I_1 \cap I_2$, so there is an inclusion $R/(I_1 \cap I_2) \subseteq R/I_1 \oplus R/I_2$. Hence, by \Cref{ass ses} and \Cref{ass direct sum}, $$\Ass(R/(I_1\cap I_2)) \subseteq \Ass(R/I_1 \oplus R/I_2) = \Ass(R/I_1) \cup \Ass(R/I_2).$$The statement for larger $t$ follows by an easy induction.

[^1]: Notation: [[Associated Prime]]