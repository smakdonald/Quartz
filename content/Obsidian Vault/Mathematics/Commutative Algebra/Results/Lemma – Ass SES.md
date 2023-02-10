#### $\lem$ – Ass SES
If $$\begin{CD}
0@>>>L@>>>M@>>>N@>>>0
\end{CD}$$is an [[Exact Sequence|exact sequence]] of $R$-modules, then $\Ass(L) \subseteq \Ass(M) \subseteq \Ass(L) \cup \Ass(N)$[^1].

##### *Proof.*
If $R/P$ includes in $L$, then composition with the inclusion $L\hookrightarrow M$ gives an inclusion $R/P \hookrightarrow M$. Therefore, $\Ass(L) \subseteq \Ass(M)$. 

Now let $P \in \Ass(M)$, and let $m \in M$ be such that $P=\ann(m)$. First, note that $P \subseteq \ann(rm)$ for all $r \in R$.

Thinking of $L$ as a submodule of $M$, suppose that there exists $r \notin P$ such that $rm \in L$. Then $$s(rm) = 0 \Longleftrightarrow (sr)m = 0 \implies sr \in P \implies s \in P.$$So $P = \ann(rm)$, and thus $P \in \Ass(L)$. 

If $rm \notin L$ for all $r \notin P$, let $n$ be the image of $m$ in $N$. Thinking of $N$ as $M/L$, if $rn = 0$, then we must have $rm \in L$, and by assumption this implies $r \in P$. Since $P = \ann(m) \subseteq \ann(n)$, we conclude that $P = \ann(n)$. Therefore, $P \in \Ass(N)$.

[^1]: Notation: [[Associated Prime]]