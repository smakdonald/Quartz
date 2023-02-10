#### $\cor$ – Module Powers are Noetherian
A module $M$ is [[Noetherian Module|noetherian]] if and only if $M^n$ is noetherian for some $n$. In particular, if $R$ is a [[Noetherian Ring|noetherian ring]] then $R^n$ is a noetherian module.

##### *Proof.*
We will do induction on $n$. The case $n=1$ is a tautology. For $n>1$, consider the short exact sequence
$$\begin{CD}
0@>>>M^{n-1}@>>>M^{n}@>g>>M@>>>0
\end{CD}$$
Lemma \ref{lem:Noethses} and the inductive hypothesis give the desired conclusion.