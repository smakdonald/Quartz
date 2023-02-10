#### $\thm$ – Fraction Rings are Actually Rings
If $R$ is a [[Commutative Ring|commutative]] [[Ring|ring]] and $S$ is a [[Multiplicatively Closed Set|multiplicatively closed]] subset of non-[[Zero-Divisor|zerodivisors]], the rules given in the above definition for $+$ and $\cdot$ make $S^{-1} R$ into a commutative ring. Moreover, the function $R\to S^{-1}R$ sending $r$ to $\frac{r}{1}$ is an injective ring [[Homomorphism|homomorphism]].

###### *Proof.* 
There is a lot of small things to check and we'll just do a few. Right off the bat we need to be sure the given equivalence relation really is one. The reflexive
and symmetric properties are clear. But the proof of transitivity illustrates a key point: Say $\frac{r}{s} \sim \frac{r'}{s'} \sim \frac{r''}{s''}$. Then $rs'= r's$ and $r's'' = r''s'$. We need to deduce that $rs'' = r''s$. The given equations imply $rs's'' = r'ss'' = r''ss'$ and {\em since $s'$ is a nonzerodivisor}
we conclude $rs'' = r''s$. This is in fact the only time that the fact that $S$ consists of nonzerodivisors is used.



We also need to be sure  our rules for $+$ and $\cdot$ make sense and are independent of representation. They "make sense'' since we assume $S$ is closed under $\cdot$. To show $+$ is independent of representations, say $\frac{r}{s} \sim \frac{r''}{s''}$, so that $rs'' = r''s$. Then
$$
\frac{r}{s} + \frac{r'}{s'} := \frac{rs' + r's}{ss'}
$$
and
$$
\frac{r''}{s''} + \frac{r'}{s'} := \frac{r''s' + r's''}{s''s'}
$$
and so we need to show $(rs' + r's)(s''s') \sim (r''s' + r's'')(ss')$. This is clear upon expaning out both sides and using $rs'' = r''s$. In a similar way one
shows $\cdot$ is well-defined.

From now on we just write $=$ instead of $\sim$ when dealing with fractions.

The associative and distributive axioms involve a straightfoward but tedious check, and we skip them entirely.
The fact that $+$ and $\cdot$ are commutative is clear from their definitions.
$S^{-1}R$ is a group under addition since
it has a  $0$ element, namely $\frac{0}{1}$, and
$\frac{r}{s} +
\frac{-r}{s} = \frac{rs - rs}{s^2} = \frac{0}{s^2} = \frac{0}{1}$, with the last equality holding since $0 \cdot 1 = s^2 \cdot 0$.
The $1$
element is $\frac{1}{1}$. (Note that we have used that $1 \in S$ a couple times here --- indeed, without this assumption $S$ could be empty and then $S^{-1}R$
would be the empty set.)

The fact that $r \mapsto \frac{r}{1}$ is a ring homomorphism is straightforward to check. Its injective since $\frac{r}{1} = \frac{0}{1}$ implies $r = 0$.
***