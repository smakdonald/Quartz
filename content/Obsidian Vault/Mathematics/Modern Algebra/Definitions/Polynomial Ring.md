#### $\defn$ – Polynomial Ring in $x$
For any [[Commutative Ring|commutative]] [[Ring|ring]] $R$, the *polynomial ring in the variable* $x$, written $R[x]$, is the set
$$R[x]=\{ a_nx^n+\ldots+a_1x+a_0\mid  n\in \Z, n\geq 0, a_i\in R\}$$
with addition defined by $$(a_nx^n+\ldots+a_1x+a_0)+(b_nx^n+\ldots+b_1x+b_0)=(a_n+b_n)x^n+\ldots+(a_1+b_1)x+(a_0+b_0)$$and multiplication defined by $$(a_nx^n+\ldots+a_1x+a_0)(b_mx^n+\ldots+b_1x+b_0)=\sum_{k=0}^{n+m}\left(\sum_{i=0}^k a_ib_{k-i}\right)x^i.$$For any commutative ring $R$, the *polynomial ring in* $x_1, \dots, x_n$, written $R[x_1, \dots, x_n]$, is defined inductively as $R[x_1, \dots, x_n]=R[x_1, \dots, x_{n-1}][x_n]$, but more easily thought of as the set consisting of (finite) sums of the form $$ R[x_1, \dots, x_n]=\left\{\sum_{e_1, \dots, e_n \in \Z_{\geq 0}} r_{e_1, \dots, e_n} x_1^{e_1} x_2^{e_2} \cdots x_n^{e_n}\right\}$$with addition and multiplication defined by rules similar to the ones seen above.
***

#### $\defn$ – Polynomial Ring
Let $G$ be a [[Free Group|free]] [[Abelian Group|abelian]] [[Group|group]] with [[Generator|generators]] $x_1, \dots, x_n$. For any commutative ring $R$, the *polynomial ring* in $x_1, \dots, x_n$, written $R[x_1, \dots, x_n]$, is the [[Subring|subring]] of $R[G]$[^1] consisting of (finite) sums of the form
$$\sum_{e_1, \dots, e_n \in \Z_{\geq 0}} r_{e_1, \dots, e_n} x_1^{e_1} x_2^{e_2} \cdots x_n^{e_n}.$$
***

[^1]: See: [[Group Ring]]