#### $\lem$ – Ring Homomorphism Properties
If $f: R \to S$ is a [[Ring|ring]] [[Homomorphism|homomorphism]], then
1. $f(0_R) = 0_S$ and $f(-x)=-f(x)$. 
2. if $R$, $S$ are [[Unital Ring|unital]] then $f(1_R)$ can be either $0_S, 1_S$ or a [[Zero-Divisor|zero divisor.]] 
3. If $f(1_R)=1_S$ and $u\in R^\times$[^1] then $f(u^{-1})=f(u)^{-1}$.

###### *Proof.* 
(2) Since $1_R1_R=1_R$ we have $f(1_R)f(1_R)=f(1_R)$, thus $$f(1_R)(f(1_R)-1_S)=0_S.$$ Now either $f(1_R)=0_S$ or $f(1_R)-1_S=0_S$ (which yields $f(1_R)=1_S$) or both of these are nonzero and then they are complementary zero divisors (in particular, $f(1_R)$ is a zero divisor).
***

[^1]: See: [[Group of Units]]