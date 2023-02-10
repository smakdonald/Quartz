#### $\defn$ – Hilbert Symbol
We define the $p$-adic *Hilbert symbol* $(a,b)_p$ for $a,b\in\Q^{\times}$ and $p\leq\infty$
- For $2 < p < \infty$, write $i = v_{p}(a)$ and $j = v_{p}(b)$, so $a = p^{i}u$ and $b = p^{j} v$ with $u, v \in Z^{\times}_{p}$. Then set $$(a,b)_{p}=\leg{(-1)^{ij}u^{j}v_{i}}{p}=\leg{-1}{p}^{ij}\leg up^{j}\leg vp^{i}=(-1)^{\frac{ij(p-1)}{2}}\leg up^{j}\leg vp^{i}$$
- For $p=2$, take $i,j,u,v$ as above, and set $$(a,b)_{2}=(-1)^{e},\text{ where }e=\leg{u-1}{2}\cdot\leg{v-1}{2}+\leg{j(u^{2}-1)}{8}+\leg{i(v^{2}-1)}{8}$$
- For $p=\infty$, define $$(a,b)_{\infty}=\begin{cases}
+1& \text{ if } a>0 \text{ or } b>0 \\
-1& \text{ if } a<0 \text{ and } b<0
\end{cases}$$