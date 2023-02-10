#### $\lem$ – Making a Pure-Power Leading Term (Graded Version)
Let $k$ be an infinite field, and let $R=k[x_1,\dots,x_n]$[^1] be standard [[Graded Ring|graded]], meaning $\deg(x_i)=1$. Let $f\in R$ be a [[Homogeneous Element|homogeneous]] polynomial of [[Polynomial Degree|degree]] $N$ #eltypo . There is a degree-preserving $k$-[[Algebra|algebra]] automorphism of $R$ given by $\phi(x_i) = x_i + a_i x_n$ for $i<n$ and $\phi(x_n)=x_n$ that maps $f$ to a polynomial that viewed as a polynomial in $x_n$ with coefficients in $k[x_1,\dots,x_{n-1}]$, has leading term $a x_n^N$ for some (nonzero) $a\in k$.

##### *Proof.*
Given \Cref{lemma leading term noether normalization}, we just need to show that the $x^N$ coefficient of $\phi(f)$ is nonzero for some choice of $a_i$. One can check that the coefficient of the $x^N$ term is $f(-a_1,\dots,-a_{n-1},1)$. But $f(-a_1,\dots,-a_{n-1},1)$, when thought of as a polynomial in the $a_i$, is identically zero, then $f$ must be the zero polynomial.

[^1]: Notation: [[Polynomial Ring]]