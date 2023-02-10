#### $\prop$ – Injective iff Trivial Kernel
A [[Group|group]] [[Homomorphism|homomorphism]] $f: G \to H$ is one-to-one if and only if $\ker(f) = \{e_G\}$[^1].

###### *Proof.* 
$(\Rightarrow)$ As $e_G \in \ker(f)$ for all homomorphisms $f$, we have $\{e\}\sse\ker(f)$.
$(\Leftarrow)$ If $\ker(f) = \{e_G\}$ and $f(h) = f(h')$ then $$f(h^{-1}h') = f(h)^{-1}f(h') = e_H$$ placing $h\inv h'\in\ker(f)=\{e\}$. Thus $h^{-1}h' = e_G$ which implies $h = h'$[^2].
***

[^1]: Notation: $\ker(f)$ is the [[Kernel|kernel]] of $f$.
[^2]: This is because [[Proposition – Unique Inverse|inverses are unique]] in groups. Since $h\inv$ is the inverse of both $h$ and $h'$, we must have $h=h'$.