#### $\thm$ – Divisors and Subgroups of Cyclic Group
Let $G=\langle x\rangle$[^1], where $x$ has finite [[Order|order]] $n$. Then
1. $G=\{e,x,\ldots,x^{n-1}\}$.
2. There is a bijection $$\Psi : \{\text{divisors of } |G|\} \to \{\text{subgroups of } G\} \text{ given by } \Psi(d) = \langle x^{\frac{|G|}{d}}  \rangle$$for each divisor $d$ of $|G|$. Moreover, for each [[Subgroup|subgroup]] $H$ of $G$, $\Psi^{-1}(H) = |H|$. In particular, all subgroups of $G$ are cyclic and there is a unique subgroup of each order.

###### *Proof.* 
By this [[Lemma – Elements of $langle X rangle$|lemma]] the group $G$ has the following elements $G=\{x^i \mid i\in \Z\}$.

If $0\leq i<j<n$ and $x^i=x^j$ then $x^{j-i}=e$ and $1\leq j-i<n$, contradicting the minimality[^2] of the order of $x$. Thus the elements $x^0, x^1, \dots, x^{n-1}$ are distinct, and so $|G|\geq n$. 

For any $m\in \Z$ division by $n$ yields integers $q,r$ with $0\leq r\leq n-1$ such that $m=nq+r$. Then $$x^m=x^{nq+r}=(x^n)^qx^r=x^r\in\{x^0, x^1, \dots, x^{n-1}\}.$$ Thus $G\subseteq\{x^0, x^1, \dots, x^{n-1}\}$ and $|G|\leq n$. 

Let $\Phi:\{\text{subgroups of } G\} \to  \{\text{divisors of } |G|\}$ be given by $\Phi(H)=|H|$. Suppose $d\big||G|$. We have $$(\Psi\circ\Phi)(d)=\left| \langle g^{\frac{|G|}{d}}\rangle\right|=\left| g^{\frac{|G|}{d}}\right|=\frac{|G|}{\gcd(|G|/d,|G|)}=\frac{|G|}{|G|/d}=d.$$Now suppose $H\leq G$. Set $k=\min\{i \mid i\in \Z, i>0, g^i\in H\}$. Since $H\subseteq G=\langle g\rangle$ any element of $H$ is of the form $g^m$ for some $m\in \Z$. By the Division Theorem #later$m=kq+r$ for some $r\in \Z$, $0\leq r<k$. Since $g^m$ and $g^k$ are elements of $H$, $g^r=g^m(g^{k})^{-q}\in H$. Since $r<k$ and $g^r\in H$,  by the minimality of $k$ it follows that $r$ cannot be positive and thus $r=0$. Therefore $m=kq$ and we have shown that $H\subseteq \langle g^k \rangle$. The opposite containment follows because $g^k\in H$ and $\langle g^k \rangle$ is the smallest subgroup of $G$ containing $g^k$[^3]. Thus $H=\langle g^k \rangle$.

Thus $H\leq G$ is either $H=\{e\}$, for which $(\Phi\circ\Psi)(\{e\})=\Phi(1)=\langle g^{|G|} \rangle=\{e\}$ or is of the form $H=\langle g^k \rangle$. In the latter case, setting $|G|=n$ we have $|H|=|g^k|=\frac{n}{\gcd(n,k)}$ and $$(\Phi\circ\Psi)(H)=\langle g^{\frac{n}{n/\gcd(n,k)}} \rangle=\langle g^{\gcd(n,k)}\rangle.$$It remains to show that $\langle g^{\gcd(n,k)}\rangle=\langle g^k\rangle=H$. By Bezout's Identity #later , $\gcd(n,k)=an+bk$ for some integers $a,b$. Since $g^{\gcd(n,k)}=(g^n)^a(g^k)^b=e^a(g^k)^b=(g^k)^b\in \langle g^k \rangle$ if follows that $\langle g^{\gcd(n,k)}\rangle \subseteq \langle g^k \rangle$. On the other hand $k$ is a multiple of $\gcd(n,k)$ so $g^k\in \langle g^{\gcd(n,k)}\rangle$ and thus $\langle g^k \rangle \subseteq \langle g^{\gcd(n,k)}\rangle$. Finally, we conclude that  $(\Phi\circ\Psi)(\langle g^k \rangle)=\langle g^{\gcd(n,k)}\rangle=\langle g^k \rangle$ for any $k\in \Z,k>0$.

Thus $\Phi$ is a two sided inverse to $\Phi$, hence $\Phi$ is a bijection.
***

[^1]: Notation: $\langle x\rangle$ denotes the [[Cyclic|cyclic]] [[Subgroup|subgroup]] of $G$ [[Generator|generated]] by the element $x$. This tells us that $G$ is itself a cyclic group.
[^2]: From this [[Lemma – $x^m = e to x big m$.|lemma]], the order of $x$ is the smallest number $n$ such that  $x^n=e$. 
[^3]: From the definition of [[Generator|generated subgroup]] we see that $\langle g^k \rangle$ is the intersection of all subgroups containing $g^k$, making it the smallest one with respect to containment.