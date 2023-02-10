#### $\cor$ – Ass Direct Sum
Let $A$ and $B$ be $R$-modules. Then $\Ass(A \oplus B) = \Ass(A) \cup \Ass(B)$[^1].

##### *Proof.*
Apply \Cref{ass ses} to the short exact sequence $$\begin{CD}
0@>>>A@>>>A\oplus B@>>>B@>>>0
\end{CD}$$We obtain $\Ass(A) \subseteq \Ass(A \oplus B) \subseteq \Ass(A) \cup \Ass(B)$. Repeat with $$\begin{CD}
0@>>>B@>>>A\oplus B@>>>A@>>>0
\end{CD}$$to conclude that $\Ass(B) \subseteq \Ass(A \oplus B)$. So we have shown both $\Ass(A) \subseteq \Ass(A \oplus B)$ and $\Ass(B) \subseteq \Ass(A \oplus B)$, so $\Ass(A) \cup \Ass(B) \subseteq \Ass(A \oplus B)$. Since we have also already shown $\Ass(A \oplus B) \subseteq \Ass(A) \cup \Ass(B)$, we must have $\Ass(A \oplus B) = \Ass(A) \cup \Ass(B)$.

[^1]: Notation: For $\Ass$, see: [[Associated Prime]]. For $\oplus$, see: [[Direct Product, Sum|Direct Sum]]