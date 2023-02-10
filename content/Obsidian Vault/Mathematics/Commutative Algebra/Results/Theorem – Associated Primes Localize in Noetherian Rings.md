#### $\thm$ – Associated Primes Localize in Noetherian Rings
Let $R$ be a [[Noetherian Ring|noetherian ring]], $W$ a [[Multiplicatively Closed Set|multiplicative set]], and $M$ a module. Then[^1] $$\Ass_{W^{-1}R}(W^{-1}M)=\{W^{-1}P  \ | \ P \in \Ass_R(M), \, P \cap W = \varnothing\}.$$
##### *Proof.*
Given $P \in \Ass_R(M)$ such that $P \cap W= \varnothing$, \Cref{localization ideals} says that $W^{-1}P$ is a prime in $W^{-1}R$. Then $W^{-1}R /W^{-1}P \cong W^{-1}(R/P) \hookrightarrow W^{-1}M$ by exactness (see \Cref{localization is exact}), so $W^{-1}P$ is an associated prime of $W^{-1} M$. 

Now suppose that $Q \in \Spec(W^{-1}R)$ is associated to $W^{-1}M$. By \Cref{localization ideals}, we know this is of the form $W^{-1}P$ for some prime $P$ in $R$ such that $P \cap W = \varnothing$. Since $R$ is noetherian, $P$ is finitely generated, say $P = (f_1, \ldots, f_n)$ in $R$, and so $Q = \left( \frac{f_1}{1}, \ldots, \frac{f_n}{1} \right)$.


By assumption, $Q = \ann(\frac{m}{w})$ for some $m \in M$, $w \in W$. Since $w$ is a unit in $W^{-1}R$, we can also write $Q = \ann(\frac{m}{1})$. By definition, this means that for each $i$$$\frac{f_i}{1} \frac{m}{1} = \frac{0}{1} \, \Longleftrightarrow \, u_i f_i m = 0 \textrm{ for some } u_i \in W.$$Let $u = u_1 \cdots u_n \in W$. Then $u f_i m = 0$ for all $i$, and thus $P u m = 0$. We claim that in fact $P = \ann(um)$ in $R$. Consider $v \in \ann(um)$. Then $u (vm) = 0$, and since $u \in W$, this implies that $\frac{vm}{1} = 0$. Therefore, $\frac{v}{1} \in \ann(\frac{m}{1}) = W^{-1}P$, and $vw \in P$ for some $w \in W$. But $P \cap W = \varnothing$, and thus $v \in P$. Thus $P \in \Ass(M)$.

[^1]: Notation: [[Associated Prime]], [[Localization]]