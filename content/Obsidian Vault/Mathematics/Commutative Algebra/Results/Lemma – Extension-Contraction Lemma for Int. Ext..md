#### $\lem$ – Extension-Contraction Lemma for Int. Ext.
Let $R \subseteq S$ be [[Integral Element|integral]], and $I$ be an ideal of $R$. Then $IS \subseteq\overline{I}^S$[^1], and hence $I S \cap R \subseteq \overline{I}$.

##### *Proof.*
Let $x\in IS$. We can write $x = a_1 s_1 + \cdots + a_t s_t$ for some $a_i\in I$. Moreover, taking $S'=R[s_1,\dots,s_t]$, we also have $x\in IS'$. We will show that $x \in \overline{I}^{S'}$, so $x \in \overline{I}^{S}$ follows as a corollary. So we might as well replace $S$ with $S'$, so that $R \subseteq S$ is also integral and module-finite.  By \Cref{characterization of mod-fin alg-fin integral}, the extension is also module-finite.

Let $S= R b_1 + \cdots + R b_n$. We can write 
$$x b_i = \left(\sum_{k=1}^t a_k s_k \right) b_i = \sum_j a_{ij} b_j$$ 
with $a_{ij}\in I$. We can write these equations in the form $x v = Av$, where $v=(b_1,\dots,b_u)$, and $A=[a_{ij}]$. By the determinantal trick, \Cref{determinantal trick}, we have $\det(xI-A)v=0$. Since we can assume $b_1=1$, we have $\det(xI-A)=0$. The fact that this is the type of equation we want follows from the monomial expansion of the determinant: any monomial is a product of $n$ terms where some of them are copies of $x$, and the rest are elements of $I$. Since this is a product of $n$ terms, a term in $x^i$ has a coefficient coming from a product of $n-i$ elements of $I$.

So this shows that $IS \subseteq\overline{I}^S$. Now notice that $\overline{I}^S \cap R = \overline{I}$ is immediate from the definition, as noted in \Cref{integral closure contraction}.

[^1]: Notation: [[Integral Closure]]