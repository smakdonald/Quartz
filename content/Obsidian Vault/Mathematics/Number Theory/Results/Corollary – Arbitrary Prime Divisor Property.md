#### $\cor$ – Arbitrary Prime Divisor Property
If $a_{1}, \dots  , a_{n} \in\Z$[^1] and $p$ is a [[Prime|prime]] with $p|a_{1} \cdots a_{n}$,[^2] then $p | a_{i}$ for some  $1 \leq  i \leq  n$.

##### *Proof.*
We induct on $n$, the number of factors. The base case of $n = 2$ is the previous lemma. Now we assume that whenever $p$ divides a product of $n - 1$ factors for $n > 2$, it divides one of the $n - 1$ individual factors, and prove the analogous statement for $n$. Suppose $p | a_{1} \cdots  a_{n} = a_{1}(a_{2} \cdots  a_{n} )$. By the previous lemma, $p | a_{1} or p|a_{2} \cdots  a_{n}$. But by the induction hypothesis, the latter case implies that $p | a_{i}$ for some $2 \leq  i \leq  n$. In either case, $p$ divides one of the $a_{i}$ and we are done.

[^1]: Notation: [[Integers]]
[^2]: Notation: [[Divides]]