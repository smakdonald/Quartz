#### $\thm$ – Bézout’s Identity (Gaussian)
Let $\a, \beta \in\Z[i]$, not both zero, and let $\g$ be a $\gcd$ of $\a$ and $\beta$. Then there exist 
$\mu, \nu \in\Z[i]$ such that $\a \mu + \beta \nu = \g$.

##### *Proof.*
Let S = {\g = \mu \a + \nu\beta = 0 : \mu, \nu \in\Z[i]}. The set N (S) = {N (\g ) : \g \in S} is 
a non-empty subset of N, and by the Well-Ordering Principle there exists a smallest 
element d \in\N (S). Let \delta be any element of S with N (\delta ) = d. By definition of S, 
we have \delta = \a σ + \beta \tau for some σ, \tau \in\Z[i]. By the Division Algorithm, there exist 
Gaussian integers \chi and \rho, with N (\rho ) < N (\delta ), such that \a = \chi \delta + \rho, and so 
\rho = \a - \chi \delta = \a - \chi (\a σ + \beta \tau ) = \a (1 - \chi σ) + \beta (-\chi \tau ). 
This shows that \rho \in S if N (\rho ) > 0, which would contradict the fact that \delta had 
minimal norm (since N (\rho ) < N (\delta )). It follows that N (\rho ) = 0, so \rho = 0, and thus 
\delta | \a. An analogous argument proves that \delta | \beta, and so \delta | \g as well (recalling that 
\g is the given \gcd of \a and \beta we seek to write as a linear combination of \a and \beta ). 
Write \g = \varphi\delta. We get 
\g = \varphi\delta = \varphi(\a σ + \beta \tau ) = \a (\varphiσ) + \beta (\varphi\tau ), 
as desired.