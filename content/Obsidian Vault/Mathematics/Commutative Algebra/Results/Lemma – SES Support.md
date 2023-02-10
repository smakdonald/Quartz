#### $\lem$ – SES Support
Let $R$ be a ring, $L,M,N$ be modules. If $$\begin{CD}
0@>>>L@>>>M@>>>N@>>>0
\end{CD}$$ is exact, then $\Supp(L) \cup \Supp(N) = \Supp(M)$[^1]. 

##### *Proof.*
Localization is exact, by \Cref{localization is exact}, so for any $P$, $$\begin{CD}
0@>>>L_{p}@>>>M_{p}@>>>N_{p}@>>>0
\end{CD}$$is exact. If $P \in \Supp(L) \cup \Supp(N)$, then $L_P$ or $N_P$ is nonzero, so $M_P$ must be nonzero as well. On the other hand, if $P \notin \Supp(L) \cup \Supp(N)$, then $L_P = N_P =0$, so $M_P=0$.

[^1]: Notation: [[Support]]