#### $\prop$ – Characterizations of Symbolic Powers
Let $R$ be [[Noetherian Ring|noetherian]], and $P$ a [[Prime Ideal|prime ideal]] of $R$. 
(a) $P^{(n)}=\{ r\in R \ \mid \ rs\in P^n \textrm{ for some }  s\notin P \}$[^1].
(b) $P^{(n)}$ is the unique smallest $P$-[[Primary Ideal|primary]] ideal containing $P^n$.
(c) $P^{(n)}$ is the $P$-primary component in any minimal [[Primary Decomposition|primary decomposition]] of $P^n$.

##### *Proof.*
The first characterization follows from the definition, and the fact that expanding and contraction to/from a localization is equivalent to saturating with respect to the multiplicative set, which we proved in \Cref{localization ideals}.

We know that $P^{(n)}$ is $P$-primary from one of the characterizations of primary we gave in \Cref{characterization of primary}. Any $P$-primary ideal satisfies $\q R_{P} \cap R = \q$, and if $\q\supseteq P^{n}$, then $P^{(n)} = P^n R_{P} \cap R \subseteq \q R_{P} \cap R = \q$. Thus, $P^{(n)}$ is the unique smallest $P$-primary ideal containing $P^n$.

The last characterization follows from the second uniqueness theorem, \Cref{primary decomposition uniqueness minimal components}.

[^1]: Notation: [[Symbolic Power]]