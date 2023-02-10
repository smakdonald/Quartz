#### $\defn$ – Valuation (Integer)
For a non-zero [[Integers|integer]] $n$ and [[Prime|prime]] $p$, define the $p$-*adic valuation* of $n$, denoted $v_{p}(n)$, to be the power of $p$ appearing in the [[Theorem – Prime Factorization|prime factorization]] of $n$. In other words, $v_{p}(n)$ is the unique integer such that we can write $n = p^{v_{p}(n)}n'$ for some integer $n'$ with $p\not\mid n'$[^1]

[^1]: Notation: [[Divides]]

#### $\defn$ – Valuation (Gaussian)
For non-zero $\a \in\Z[i]$ and Gaussian prime $\pi$, define the $\pi$-adic valuation of $\a$, 
denoted $v_{\pi} (\a )$, to be the power of $\pi$ that appears in the prime factorization of $\a$. 
In other words, $v_{\pi} (\a)$ is the unique integer such that we can write 
$$\a = \pi^{v_{\pi}(\a)}\a'$$
for some $\a' \in\Z[i]$ with $\pi\not\mid\a'$.

#### $\defn$ – Valuation (p-Adic)
For non-zero $\a \in\Q_{p}$ as in (∗), the $p$-adic valuation $v_{p}(\a )=-k$ is the least power of $p$ appearing in its $p$-adic expansion. As in Lemma 8.1.2, we can alternatively view it as the largest power of $p$ dividing every term in the $p$-adic expansion of $\a$. By factoring it out, we can write any $\a \in\Q_{p}$ uniquely in the $$\a = p^{v_{p}(\a)}\a'$$where $\a'\in\Z_{p}$ and $v_{p}(\a') = 0$ (i.e., $\a'\mod p\neq 0$). As we did in $\Z$, define $v_{p}(0) = \infty$. Note the $p$-adic integers $\Z_{p}$ are characterized precisely as those $p$-adic numbers $\a$ with $v_{p}(\a ) \geq 0.$