#### $\lem$ – Every Prime Contains Minimal Prime
Let $R$ be a ring, and $I$ an ideal. Every [[Prime Ideal|prime]] $P$ that contains $I$ contains a [[Minimal Prime|minimal prime]] of $I$.

##### *Proof.*
Fix an ideal $I$ and a prime $P \supseteq I$, and consider the set$$S = \lbrace Q \in V(I) \mid P \supseteq Q \rbrace,$$which is partially ordered with $\supseteq$. On the one hand, $P \in S$, so $S$ is nonempty. On the other hand, given any chain $\{ Q_i \}_i$ in $S$, $Q :=  \bigcap_i Q_i$ is a prime ideal in $R$ (exercise!). Moreover, $Q$ contains $I$, since every $Q_i$ contain $I$, and $Q$ is contained in $P$, since every $P_i \subseteq Q$. Therefore, $Q \in S$, and Zorn's Lemma applies to $S$. By \hyperref[Zorn's Lemma]{Zorn's lemma}, $S$ contains a maximal element for $\supseteq$, say $Q$. 

Notice that $Q$ is equivalently a minimal element for $\subseteq$. Now if $Q'$ is a prime ideal with $I \subseteq Q' \subseteq Q$, then $Q' \subseteq Q \subseteq P$, and thus $Q' \in S$. Therefore, we must have $Q' = Q$, by maximality of $Q$ with respect to $\supseteq$. We conclude that $Q$ is a minimal prime of $I$, and by definition $Q$ is contained in $P$.