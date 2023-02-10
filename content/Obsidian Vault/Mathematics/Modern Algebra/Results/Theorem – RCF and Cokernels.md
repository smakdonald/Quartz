#### $\thm$ – RCF and Cokernels
Let $F$ be a [[Field|field]] and let $A \in \Mat_{n \times n}(F)$. The matrix  $xI_n - A \in \Mat_{n \times n}(F[x])$ presents the $F[x]$-[[Module|module]] $F^n_A$[^1]; that is, there is an [[Isomorphism|isomorphism]] of $F[x]$-modules 
$$
F^n_A \cong \coker(xI_n -A) = F[x]^n/\im(xI_n - A).
$$

###### *Proof.* 
For this proof it is useful to identity $F[x]^n$ with $F^n[x]$ where the latter refers to all expressions of the form $\sum_i v_i x^i = v_0 + v_1 x + \cdots + v_m x^m$ with $v_i \in F^n$. For instance, (when $n = 2$) we identify $\vectwo{x^2 -3x + 1}{x^7 +x + 5}$ with $\vectwo{1}{5} + \vectwo{-3}{1} x + \vectwo{1}{0} x^2 + \vectwo{0}{1} x^7$. Using this identification we define $$\phi:  F[x]^n = F^n[x] \to F^n_A$$by $\phi(\sum_i v_i x^i) = \sum_i A^i v_i$. Then $\phi$ is a $F[x]$-module homomorphism --- I leave it to you to verify this. $\phi$ is onto since, e.g., for any $v \in F^n$ we have $\phi(vx^0) = v$. 

We have $$\phi((xI_n - A) \cdot \sum_i v_i x^i) = \phi(\sum_i v_i x^{i+1} - \sum_i (Av_i) x^i) = \sum_i A^{i+1}(v_i) - \sum_i A^i(Av_i) = 0$$and hence $\ker(\phi) \supseteq \im(xI_n - A)$. By the $0$-th isomorphism theorem, there is an induced $F[x]$-module homomorphism $$\ov{\phi}: \frac{F^n[x]}{\im(xI_n - A)}  \onto F^n_A$$induced by $\phi$, and it is onto since $\phi$ is onto. It remains to show this map is one-to-one. 

Since $\overline{\phi}$ is $F[x]$-linear it is certainly $F$-linear. Since $\dim_F(F^n_A) = n$, to prove $\overline{\phi}$ is one-to-one,
it suffices to prove $\dim_F \frac{F^n[x]}{\im(xI_n - A)} \leq n$ (by Rank-Nullity). I claim the images of the standard basis $e_1, \dots, e_n$ in  $\frac{F^n[x]}{\im(xI_n - A)}$ span it as an $F$-vector space. To see this, note that $x^je_i$, for $1 \leq i \leq n$, $j \geq 0$ span $F^n[x]$ as an $F$-vector space, and hence they span the quotient.
It thus suffices to show $\overline{x^j e_i}$ lies in the span of $\overline{e_1}, \dots, \overline{e_n}$ in $\frac{F^n[x]}{\im(xI_n - A)}$ for all $i$ and $j$.  
We have $x^{j-1} \cdot (A - x) e_i \in \im(xI_n - A)$ and thus $$\overline{x^j e_i} = \overline{x^{j-1} Ae_i}$$and by repeating this argument we have $$\overline{x^j e_i} =\overline{x^{j-1} Ae_i} = \overline{x^{j-2} A^2e_i} = \cdots =\overline{A^je_i} \in \Span_F(e_1, \dots, e_n).$$
***

[^1]: See: [[Polynomial Ring]]