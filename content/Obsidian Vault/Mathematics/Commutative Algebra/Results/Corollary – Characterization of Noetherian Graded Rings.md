#### $\cor$ – Characterization of Noetherian Graded Rings
An $\N$-[[Graded Ring|graded]] ring $R$ is [[Noetherian Ring|noetherian]] if and only if $R_0$ is noetherian and $R$ is [[Algebra Finite|algebra-finite]] over $R_0$.

##### *Proof.*
If $R_0$ is noetherian and $R$ is algebra-finite over $R_0$, then $R$ is noetherian by the \hyperref[hilbert basis]{Hilbert Basis Theorem}. On the other hand, if $R$ is noetherian then any quotient of $R$ is also noetherian, by \Cref{quotient noetherian}, and in particular $R_0 \cong R/R_+$ is noetherian. Moreover, $R_+$ is generated as an ideal by finitely many homogeneous elements by noetherianity; by \Cref{graded fg alg}, we get a finite algebra generating set for $R$ over $R_0$.