#### $\cor$ – Ass Finite
If $R$ is a [[Noetherian Ring|noetherian ring]], and $M$ is a finitely generated module, and $$M=M_t \supsetneq M_{t-1} \supsetneq M_{t-2} \supsetneq \cdots \supsetneq  M_1 \supsetneq M_0 = 0$$ is a [[Theorem – Filtration|prime filtration]] of $M$ with $M_i/M_{i-1}\cong R/P_i$, then $$\Ass_R(M)\subseteq \{ P_1, \dots, P_t \}.$$Therefore, $\Ass_R(M)$ is finite. Moreover, if $M$ is [[Graded Module|graded]], then $\Ass_R(M)$ is a finite set of [[Homogeneous Ideal|homogeneous]] [[Prime Ideal|primes]].

##### *Proof.*
For each $i$, we have a short exact sequence
$$\begin{CD}
0@>>>M_{i-1}@>>>M_{i}@>>>M_{i}/M_{i-1}@>>>0
\end{CD}$$
By \Cref{ass ses}, $\Ass(M_i) \subseteq \Ass(M_{{i-1}})\cup \Ass(M_i/M_{i-1}) = \Ass(M_{{i-1}}) \cup \{P_i\}$. Inductively, we have $\Ass(M_i)\subseteq\{P_1,\dots,P_i\}$, and $\Ass_R(M) = \Ass_R(M_t) \subseteq \{ P_1, \dots, P_t \}$. This immediately implies that $\Ass(M)$ is finite. In the graded case, \Cref{filtration} gives us a filtration where all the $P_i$ are homogeneous primes, and those include all the associated primes.