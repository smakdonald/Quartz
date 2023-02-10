#### $\lem$ – Transcendence Basis Well-Defined 2
If $\{x_1,\dots,x_m\}$ and $\{y_1,\dots,y_n\}$ are two [[Transcendence Basis|transcendence bases]] for $L$ over $K$, then $m=n$.

##### *Proof.*
Say that $m\leqslant n$.  If the intersection has $s<m$ elements, then without loss of generality $y_1\notin \{x_1,\dots,x_m\}$. Then, for some $i$,  $\{x_i, y_2\dots,y_n\}$ is a transcendence basis, and $\{x_1,\dots,x_m\} \cap \{x_i, y_2\dots,y_n\}$ has $s+1$ elements. Replacing $\{y_1,\dots,y_n\}$ with  $\{x_i, y_2\dots,y_n\}$ and repeating this process, we obtain a transcendence basis with $n$ elements such that $\{x_1,\dots,x_m\} \subseteq \{y_1,\dots,y_n\}$. But we must then have that these two transcendence bases are equal, so $m=n$.