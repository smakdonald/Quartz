#### $\thm$ – Fundamental Theorem of Gaussian Arithmetic
Every non-zero Gaussian integer can be written in the form $\a = \epsilon\pi_{1} \cdots \pi_{k}$, where $\epsilon$ is a unit, $k \geq 0$, and each $\pi_{j}$ a Gaussian prime. Moreover, this form is unique up to reordering and associates.

##### *Proof.*
(sketch) Recall that the proof of the Fundamental Theorem of Arithmetic in 
Z has two parts: an existence proof and a uniqueness proof. As was the case in Z we 
can use strong induction to prove the existence of a prime factorization into Gaussian 
primes. This time, rather than inducting on the natural number a, we induct on N (\a ). 
The crux of the uniqueness proof in Z was the Prime Divisor Property, and it 
is again in \Z[i]. Suppose we had two distinct factorizations of \a as the product of 
Gaussian primes: 
ε\pi1 \cdots \pik = ε \tau 1 \cdots \tau . 
Canceling any like or associate factors from both sides, what remains is an equality 
between two products 
\pi1\pi2 \cdots \pis = \tau 1\tau 2 \cdots \tau t. 
Let \pi j be a prime appearing in the product on the left. Then \pi j | \tau 1\tau 2 \cdots \tau t and 
so by Lemma 5.5.8, \pi j | \tau k for some 1 \leq k \leq , which implies that \pi j and \tau k 
are associates. This contradicts the statement that \pi j and \tau k are primes that remain 
after canceling all like or associate factors appearing in both factorizations. Thus, 
the original factorizations must not have been distinct up to associates.