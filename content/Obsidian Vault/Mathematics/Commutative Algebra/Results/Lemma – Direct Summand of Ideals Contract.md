#### $\lem$ – Direct Summand of Ideals Contract
Let $R$ be a [[Direct Summand|direct summand]] of $S$. Then, for any ideal $I \subseteq R$, we have $IS \cap R=I$[^1].

##### *Proof.*
Let $\pi$ be the corresponding splitting. Clearly, $I \subseteq IS \cap R$. Conversely, if $r \in IS \cap R$, we can write $r = s_1 f_1 + \cdots + s_t f_t$ for some $f_i \in I$, $s_i \in S$. Applying $\pi$, we have
$$r = \pi(r) = \pi \left( \sum_{i=1}^t s_i f_i \right) = \sum_{i=1}^t \pi\left( s_i f_i \right) = \sum_{i=1}^t \pi \left( s_i \right) f_i \in I.$$

[^1]: Notation: [[Contraction]]