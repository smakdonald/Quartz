#### $\prop$ – Universal Mapping Property of a Cyclic Group
Assume $G = \langle x \rangle$[^1] and let $H$ be any [[Group|group]]. If $|x| = n < \infty$[^2], then for each $y \in H$ such that $y^n = e$, 
there is a unique group [[Homomorphism|homomorphism]] $$f: G \to H$$such that $f(x) = y$. 
If $|x| = \infty$, then for each $y \in H$, there is a unique group homomorphism $$f: G \to H$$such that $f(x) = y$. 
In both cases this unique group homomorphism is given by $f(x^i)=y^i$ for any $i$.

###### *Proof.* 
Recall that either $G = \{e,x,x^2, \dots, x^{n-1}\}$ (with no repetitions) if $|x| = n$ or $G = \{ \cdots, x^{-2}, x^{-1}, e, x, x^e, \dots \}$ (with no repetitions) if $|x| = \infty$.[^3]  

First, uniqueness. Suppose $f:G\to H$ is a group homomorphism, and consider $f(x^i)$ for some $i$.
- if $i=0$ then $f(x^0)=f(e_G)=e_H=y^0$
- if $i>0$ then $f(x^i)=f(\underbrace{x\cdots x}_{i \text{ times}})=\underbrace{f(x)\cdots f(x)}_{i \text{ times}})=y^i$
- if $i<0$ then $$f(x^i)=f\left((x^{-i})^{-1}\right)=f\left((x^{-i})\right)^{-1}=(y^{-i})^{-1}=y^i,$$using the formula above for $-i>0$.

Now, existence. Define $f(x^i) = y^i$ for all relevant $i$ (i.e., in the first case, for $0 \leq i \leq n-1$ and in the second for all $i \in\Z$). 

To see that $f$ is well defined, suppose $x^i=x^j$ for some $i,j\in \Z$. Then, since $x^{i-j}=e_G$, using this [[Lemma – $x^m = e to x big m$.|lemma]] or the definition for order we have
$$\begin{cases}
n\mid i-j & \text{ if } |x|=n\\
i-j=0 & \text{ if } |x|=\infty\\
\end{cases}
\Rightarrow
\begin{cases}
y^ {i-j}=y^{nk} & \text{ if } |x|=n\\
y^{i-j}=y^0 & \text{ if } |x|=\infty\\
\end{cases}
\Rightarrow y^ {i-j}=e_H
\Rightarrow y^ i=y^j.
$$
Thus, if $x^i=x^j$ then $f(x^i)=y^i=y^j=f(x^j)$.

As $$f(x^ix^j)=f(x^{i+j})=y^{i+j}=y^iy^j=f(x^i)f(x^j)$$for all $x$, we see that $f$ is indeed a homomorphism.
***

[^1]: Notation: $\langle x \rangle$ is the [[Cyclic|cyclic]] [[Subgroup|subgroup]] of $G$ [[Generator|generated]] by $x$.
[^2]: Notation: $|x|$ denotes the [[Order|order]] of the element $x\in G$
[^3]: This comes from the proof of this [[Theorem – Divisors and Subgroups of Cyclic Group|theorem]].