#### $\thm$ – Second Isomorphism Theorem
Let $G$ be a [[Group|group]], $H \leq G$[^1] and $N \norm G$[^2]. Then $HN \leq G$[^3], $N \cap H \norm H$, $N \norm HN$ and there is an [[Isomorphism|isomorphism]]$$\frac{H}{N \cap H} \xra{\cong} \frac{HN}{N}$$given by[^4]
$$h \cdot (N \cap H) \mapsto hN.$$

##### *Proof.* 
The first two assertions are left as exercises. #fix As $N \nsg G$ we have $N \nsg HN$. Define a [[Homomorphism|homomorphism]] $f: H \to \frac{HN}{N}$ by $f(h) = hN$. This is a homomorphism since it is the composition $$f:H \hookrightarrow HN \xra{\can} \frac{HN}{N}$$of homomorphisms. The function $f$ is onto since for all $h,n$ we have $hnN = hN = f(h)$. The [[Kernel|kernel]] of $f$ is $\ker(f)=\{h \mid hN = N\} = H \cap N$. The result thus follows from the [[Theorem – First Isomorphism Theorem|first isomorphism theorem]].
***

[^1]: See: [[Subgroup]]
[^2]: See: [[Normal Subgroup]]
[^3]: See: [[HK]]
[^4]: See: [[Quotient Group]], [[Coset]] for notation in equations.

#### $\thm$ – Second Isomorphism Theorem for Rings
Let $S$ be a subring and let $I$ be an ideal of $R$. Then $S + I = \{s + i \mid s \in S, i \in I\}$ is a subring of $R$, $S \cap I$ is an ideal of $S$, and $$\frac{S+I}{I}\cong \frac{S}{S\cap I}.$$

###### *Proof.* 
***