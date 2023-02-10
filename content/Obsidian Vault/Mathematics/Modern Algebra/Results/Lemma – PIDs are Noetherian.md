#### $\lem$ – PIDs are Noetherian
If $R$ is a [[Principal Ideal Domain|PID]] then $R$ is [[Noetherian Ring|noetherian]].

###### *Proof.* 
Consider and ascending chain of ideals of $R$; it must have the form
$$(a_1)\subseteq (a_2) \subseteq (a_3) \subseteq \cdots \subseteq (a_i)\subseteq (a_{i+1})\subseteq \cdots.$$
Consider $I=\bigcup_{i\geq 1} (a_i)$ which is an ideal of $R$ by the argument given in Theorem \ref{thm:maxexists}. Since $R$ is a PID, $I=(b)$ for some $b\in R$. Since $b\in I=\bigcup_{i\geq 1} (a_i)$, we must have $b\in (a_n)$ for some $n$.
Then we see that $I=(b)\subseteq (a_n)\subseteq (a_{n+1})\subseteq \cdots (a_j) \subseteq \cdots \subseteq I$ for all $j\geq n$, thus $I=(a_j)$ for $j\geq n$ and the chain stabilizes as desired.
***