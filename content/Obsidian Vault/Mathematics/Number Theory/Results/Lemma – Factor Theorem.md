#### $\lem$ – Factor Theorem
Let $R$ be an [[Integral Domain|integral domain]]. Every non-zero polynomial $f \in R[x]$[^1] of [[Polynomial Degree|degree]] $d$ has at most $d$ roots in $R$.

##### *Proof.*
We proceed by induction on $d$, beginning with the $d = 0$ case , where $f$ is  
constant (and non-zero) so has no roots. Now fix $d > 0$ and suppose for the sake of induction we know that all polynomials of degree $d - 1$ have at most $d - 1$ roots.  
Let $f = a d x d + \cdots  + a1 x + a0$ be a polynomial of degree $d$ and let $r$ be a root of  
$f$ (if no root exists, we are done). Then $f (r ) = 0$, and we observe that  
$$f (x) = f (x) - f (r ) = a d (x d - r d ) + a d-1(x d-1 - r d-1) + \cdots  + a1(x - r ).$$  
Combined with the polynomial identity  
$$x k - r k = (x - r )(x k-1 + x k-2r + \cdots  + xr k-2 + r k-1)$$,  
we see that we can extract a factor of $x - r$ from each summand and thus conclude  
that $f (x) = (x - r )g(x)$ for some $g \in\R[x]$ (which we could write down explicitly if we wanted to). By the  
previous lemma, $g$ has degree $d - 1$, so by the induction hypothesis it has at most $d - 1$ roots. Between these $d - 1$ roots and our initial root $r$, we see that $f$ has at  
most $d$ roots since $f (x)$ can only be zero if $x - r = 0$ or $g(x) = 0$.

[^1]: Notation: [[Polynomial Ring]]