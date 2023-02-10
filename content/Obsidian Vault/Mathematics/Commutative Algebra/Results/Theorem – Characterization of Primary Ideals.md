#### $\thm$ – Characterization of Primary Ideals
If $R$ is [[Noetherian Ring|noetherian]], the following are equivalent:
(a) $Q$ is [[Primary Ideal|primary]].
(b) Every [[Zero-Divisor|zerodivisor]] in $R/Q$ is [[Nilpotent|nilpotent]] on $R/Q$.
(c)  $\Ass(R/Q)$[^1] is a singleton.
(d)  $Q$ has exactly one [[Minimal Prime|minimal prime]], and no [[Embedded Prime|embedded primes]].
(e) $\sqrt{Q} = P$[^2] is [[Prime Ideal|prime]] and for all $r, w \in R$ with $w \notin P$, $rw \in Q \Rightarrow r \in Q$.
(f) $\sqrt{Q}= P$ is prime, and $Q R_{P} \cap R = Q$[^3].

##### *Proof.*
$(1) \iff (2)$: Saying $y$ is a zerodivisor modulo $Q$ if there is some $x\notin Q$ with $xy\in Q$. So the condition that every zerodivisor on $R/Q$ must be nilpotent is equivalent to$$\exists x \notin Q : xy \in Q \implies y^n \in Q.$$This is exactly the condition that $Q$ is a primary ideal.

$(2) \iff (3)$: First, note that the associated primes of $R/Q$ are the associated primes of the ideal $Q$, while the minimal primes of $R/Q$ are the minimal primes of $Q$. By \Cref{zerodivisors associated primes}, $$\bigcup_{P \in \Ass(Q)} P \, = \, \mathcal{Z}(R/Q).$$By \Cref{min contained in ass}, every minimal prime of $Q$ is associated to $Q$, so$$\bigcap_{P \in \Min(Q)} P = \bigcap_{P \in \Ass(Q)} P.$$Finally, every nilpotent element is always a zerodivisor. Putting all these together, we always have the following:$$\bigcup_{P \in \Ass(Q)} P \, = \, \mathcal{Z}(R/Q) \, \supseteq  \{ r \in R \mid r + Q \in \mathcal{N}(R/Q) \} \, = \bigcap_{P \in \Min(Q)} P = \bigcap_{P \in \Ass(Q)} P.$$	On the one hand, (2) says that the set of zerodivisors on $R/Q$ coincides with the elements in the nilradical of $R/Q$; thus (2) is the statement that we have equality throughout. So (2) holds if and only if$$\bigcup_{P \in \Ass(Q)} P \, = \bigcap_{P \in \Ass(Q)} P.$$The rest of the proof is elementary set theory: the intersection and union of a collection of sets agree if and only if there is only one set. More precisely, we have equality above if and only if there is only one associated prime.

$(3) \iff (4)$ is clear, given that every ideal has a minimal prime and minimal primes are always associated, so having a single associated prime means having only one minimal prime and no embedded primes.

$(1) \iff (5)$: Given the observation that the radical of a primary ideal is prime, this is just a rewording of the definition.

$(5) \iff (6)$: By \Cref{localization ideals}, we have the following characterization:$$Q R_P \cap R = \lbrace r \in R \mid sr \in Q \textrm{ for some } s \notin P \rbrace.$$Thus the second condition in $(5)$ is equivalent to $Q R_Q \cap R = Q$.

[^1]: Notation: [[Associated Prime]]
[^2]: Notation: [[Radical Ideal]]
[^3]: Notation: [[Contraction]]