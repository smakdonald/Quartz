#### $\thm$ – Going Down
Suppose that $R$ is a [[Normal Domain|normal domain]], $S$ is a domain, and $R\subseteq S$ is [[Integral Element|integral]]. Then, for every $P \subsetneq P'$ in $\Spec(R)$[^1] and $Q'$ in $\Spec(S)$ with $Q' \cap R = P'$[^2], there is some $Q \in \Spec(S)$ with $Q \subsetneq Q'$ and $Q \cap R = P$.

##### *Proof.*
Let $W=(S \setminus Q')(R \setminus P)$ be the multiplicative set in $S$ consisting of products of elements in $S \setminus Q'$ and $R \setminus P$. Note that each of the sets $S \setminus Q'$ and $R \setminus P$ contains $1$, so $S \setminus Q'$ and $R \setminus P$ are both contained in $W$. We will show that $W \cap P S$ is empty. Once we do that, it will follow from \Cref{lemma spec strong nullstellensatz} that there is a prime ideal $Q$ in $S$ containing $P S$ such that $W \cap Q$ is empty. Since $S \setminus Q' \subseteq W$, our new prime $Q$ must necessarily be contained in $Q'$.

Moreover, $R \setminus P \subseteq W$, so $(Q \cap R) \cap (R \setminus P)$ is empty, or equivalently, $Q \cap R \subseteq P$. Since $Q \cap R \subseteq P$ and $Q \cap R \supseteq P$, we conclude that $Q \cap R = P$.
 
So our goal is to show that $W \cap P S$ is empty. We proceed by contradiction, and assume there is some $x \in P S \cap W$. We can write $x=rs$ for some $r\in R \setminus P$ and $s \in S \setminus Q'$. Moreover, since $x \in P S$, $x$ is integral over $P$, by \Cref{extension contraction for integral extensions}.

Consider the minimal polynomial of $x$ over $\mathrm{frac}(R)$, say$$h(x) = x^n + a_1 x^{n-1} + \cdots + a_n = 0.$$By \Cref{lemma minimal polynomial}, each $a_i\in P' \subseteq R$. Then substituting $x=rs$ in $\textrm{frac}(R)$ and dividing by $r^n$ yields $$g(s) = s^n + \frac{a_1}{r} s^{n-1} + \cdots + \frac{a_n}{r^n} = 0.$$We claim that this is the minimal polynomial of $s$. If $s$ satisfied a monic polynomial of degree $d < n$, multiplying by $r^d$ would give us a polynomial of degree $d$ that $x$ satisfies, which is impossible. So indeed, this is the minimal polynomial of $s$.

Since $s\in S$, and thus integral over $R$, \Cref{lemma minimal polynomial} says that each $\frac{a_i}{r^i} =: v_i\in R$. Since $r \notin P$ and $r^i v_i =a_i \in P$, we must have $v_i\in P$. The equation $g(s)=0$ then shows that $s \in \sqrt{P S}$. Since $Q' \in \Spec(S)$ contains $P' S$ and hence $P S$, we have $s \in \sqrt{P S} \subseteq Q'$. This is the desired contradiction, since $s \notin Q'$ by construction.

[^1]: Notation: [[Prime Spectrum]]
[^2]: Notation: [[Contraction]]