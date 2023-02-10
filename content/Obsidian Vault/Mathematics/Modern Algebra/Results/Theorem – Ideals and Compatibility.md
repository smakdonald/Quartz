#### $\thm$ – Ideals and Compatibility
Let $I$ be a [[Subring|subring]] of a [[Ring|ring]] $R$. The following are equivalent: 
1. $I$ is an [[Ideal|ideal]] of $R$. 
2. The equivalence relation $\sim_I$ defined by $s\sim_It$ if and only if $s-t\in I$ is [[Compatible with Addition & Multiplication|compatible with addition and multiplication]]. 
3. The [[Quotient Group|quotient group]] $R/I$ (under addition) is a ring with multiplication $$(r+I)(s+I) = rs+I$$ and the quotient map $\pi R\to R/I, \pi(r)=r+I$ is a ring [[Homomorphism|homomorphism]] with $\ker(\pi)=I$[^1].

###### *Proof.* 
$1.\Rightarrow 2.$ If $s\sim_It$ then $s-t\in I$, so for any $r\in R$ we have $r(s-t)\in I$ and $(s-t)r\in I$, otherwise written as $rs\sim_I rt$ and $sr\sim_I tr$. Also,  $s\sim_It$ implies $s+r\sim_I t+r$ as $s-t=(s+r)-(t+r)\in I$.
 
$2.\Rightarrow 3.$ The main point is the well-definedness of the operations:
Since the ideal $I$ is a normal subgroup of $(R,+)$ the set of cosets $R/I$ is a group under addition. The remaining point is the well definedness of the multiplication. If $r\sim_I r'$ and $s\sim_I s'$ we deduce by compatibility with multiplication that
 $$\begin{eqnarray*}
  r\sim_I r' \Rightarrow rs\sim_I r's\\
   s\sim_I s' \Rightarrow r's\sim_I r's'
 \end{eqnarray*} $$
which by transitivity implies $rs\sim_Ir's'$. By definition of the relation $\sim_I$ this gives $rs-r's'\in I$, which by way of our criteria for coset equality from Lemma \ref{lem:cosets} (translated into additive notation) allows to conclude $rs+I= r's'+I$. The ring axioms which involve multiplication are left to check as an exercise.
 
The quotient map is known to be an additive group homomorphism with $\ker(\pi)=I$ by Lemma \ref{lem:quotientmap}. From the definition for multiplication in $R/I$ we have $$\pi(rs)=rs+I=(r+I)(s+I)=\pi(r)\pi(s)$$which allows to conclude that $\pi$ is a ring homomorphism.
 
$3.\Rightarrow 1.$ Since $(R/I, +)$ is a group we know that $I$ is a (normal) subgroup of $(R,+)$. Furthermore, if $a\in I$ and $r\in R$ then $a+I=0+I$ and by the well-definedness of multiplication we have $ra+I=r0+I=0+I$, so $ra\in I$ and $ar+I=0r+I=0+I$, so $ar\in I$.
***

[^1]: See: [[Kernel]]