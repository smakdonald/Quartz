#### $\lem$ – Graded Primes
If $R$ is a $\Z$-[[Graded Ring|graded]] ring, then any ideal $I$ with the property[^1]
$$
\text{ for any homogeneous elements }r,s\in R, \quad rs\in I \Rightarrow r\in I \ \text{or} \ s\in I
$$
is [[Prime Ideal|prime]].

##### *Proof.*
We need to show that this property implies that for any $a,b\in R$ not necessarily homogeneous, $ab\in I$ implies $a\in I$ or $b\in I$. We do this by induction on the number of nonzero homogeneous components of $a$ plus the number of nonzero homogeneous components of $b$. This is not interesting if $a = 0$ or $b=0$, so the base case is when this is two. In that case, both $a$ and $b$ are homogeneous, so the hypothesis already gives us this case. For the induction step, write $a=a' + a_m$ and $b=b'+b_n$, where $a_m,b_n$ are the nonzero homogeneous components of $a$ and $b$ of largest degree, respectively. We have $ab=(a'b'+a_m b' + b_n a') + a_m b_n$, where $a_m b_n$ is either the largest homogeneous component of $ab$ or zero. Either way, $a_m b_n\in I$, so $a_m\in I$ or $b_n\in I$; without loss of generality, we can assume $a_m\in I$. Then $a b= a' b + a_m b$, and $ab, a_m b\in I$, so $a' b\in I$, and the total number of homogeneous pieces of $a'b$ is smaller, so by induction, either $a'\in I$ so that $a\in I$, or else $b\in I$.

[^1]: See: [[Homogeneous Element]]