#### $\lem$ – Quotient Map is $R$-module Homomorphism
Let $R$ be a [[Ring|ring]], let $M$ be an $R$-[[Module|module]], and let $N$ be a [[Submodule|submodule]] of $M$. The rule for scaling introduced above is well-defined and it, along with the rule for $+$,  makes $M/N$ into an $R$-module. Moreover, the canonical quotient map $\pi: M \to M/N$, defined by $\pi(m) = m + N$,  is an $R$-module [[Homomorphism|homomorphism]] whose [[Kernel|kernel]] is $\ker(\pi) = N$.

###### *Proof.* 
Among the many things to check here, we will only check a couple.

We need to prove the rule for scaling by $R$ on $M/N$ is well-defined: If $m+N=m'+N$ then $m-m'\in N$ so $r(m-m')\in N$ by the definition of submodule. This gives that $rm-rm'\in N$, hence $rm+N=rm'+N$. The module axioms are then pretty straightforward. We already know from 817 that $M/N$ is an abelian group under $+$.

Let us check one of the four axioms involving scaling. We have $$r( (m_1 +N) + (m_2 +N)) = r((m_1 + m_2) + N) = (r(m_1+m_2)) + N = (rm_1 + rm_2) + N = (rm_1 + N) + (rm_2 + N),$$
which gives the third such axiom. The other three are also straightforward.

The fact that $\pi$ is an $R$-module homomorphism is also straightforward. Its kernel is $\{m \in M \mid m + N = N\}$, which is equal to $N$. 
***