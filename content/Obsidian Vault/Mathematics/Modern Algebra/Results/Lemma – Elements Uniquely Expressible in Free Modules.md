#### $\lem$ – Elements Uniquely Expressible in Free Modules
Suppose $M$ is a [[Basis and Free Module|free]] $R$-[[Module|module]] and $A$ is a [[Basis and Free Module|basis]] of $M$. Then every element of $M$ is uniquely expressible as an $R$-[[Linear Combination|linear combination]] of elements of $A$.

More precisely, for each $m$ there is unique family of elements $(r_a)_{a \in A}$, with $r_a \in R$ for all $a$, such that $r_a = 0$ for all but a finite number of indices $a \in A$ and $m = \sum_{a \in A} r_a a$.

###### *Proof.* 
Given $m \in M$, the fact that
$$m = \sum_a r_a a$$
for at least one family of elements $(r_a)_{a \in A}$ with $r_a = 0$ for all but a finite number of $a$'s is the definition of what it means for $A$ to generate $M$. 

Suppose $(s_a)_{a \in A}$ is another such family with $m = \sum_a s_a a$.
Then $$0 = m-m = \sum_a r_a a - \sum_a s_a a = \sum_a (r_a - s_a) a.$$
Since $A$ is linearly independent, by definition $r_a - s_a = 0$ for all $a$.
***