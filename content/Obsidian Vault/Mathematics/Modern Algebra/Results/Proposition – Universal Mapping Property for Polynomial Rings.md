#### $\prop$ – Universal Mapping Property for Polynomial Rings
Let $R$ and $S$ be [[Commutative Ring|commutative]] [[Ring|rings]], $\phi: R \to S$ is a ring [[Homomorphism|homomorphism]] and $s_1, \dots, s_n$ arbitrary elements of $S$. Then there exists a unique ring homomorphism[^1]
$$\tilde{\phi}: R[x_1, \dots, x_n] \to S$$
such that $\tilde{\phi}|_R = \phi$ and $\tilde{\phi}(x_i) = s_i$ for all $i$, namely 
$$\tilde{\phi}\left(\sum_{e_1, \dots, e_n \geq 0} r_{e_1, \dots, e_n} x_1^{e_1} \cdots x_n^{e_n}\right) =
\sum_{e_1, \dots, e_n \geq 0} \phi(r_{e_1, \dots, e_n}) s_1^{e_1} \cdots s_n^{e_n}$$

###### *Proof.* 
Let's observe first that if such a map exists it is unique. For if $\tilde\phi: R[x_1, \dots, x_n] \to S$ is a ring map extending $\phi$ and sending $x_i$ to $s_i$.  Then
$$\begin{align*}
\tilde\phi(\sum_{e_1, \dots, e_n \geq 0} r_{e_1, \dots, e_n} x_1^{e_1} \cdots x_n^{e_n}) &=
\sum_{e_1, \dots, e_n \geq 0} \phi(r_{e_1, \dots, e_n}) \phi(x_1)^{e_1} \cdots \phi(x_n)^{e_n}) \\
&=
\sum_{e_1, \dots, e_n \geq 0} \phi(r_{e_1, \dots, e_n}) s_1^{e_1} \cdots s_n^{e_n},
\end{align*}$$
using that $\tilde\phi$ preserves $+$ and $\cdot$.

For existence, let's assume $n = 1$ at first. Given $\phi: R \to S$ and $s \in S$,
define
$$
\tilde{\phi}: R[x] \to S
$$
by
$$
\tilde{\phi}(\sum_i r_i x^i) = \sum_i \phi(r_i) s^i.
$$
It is elementary (but tedious) to check $\tilde{\phi}$ really is a ring homomorphism. The fact that it restricts to $\phi$ is clear, however.


For the general case, we proceed by induction on the number of variables $n$. The induction hypothesis shows that there is a ring homomorphism
$$
\psi: R[x_1, \dots, x_{n-1}] \to S
$$
such that $\psi|_R = \phi$ and $\psi(x_i) = s_i$, $i = 1, \dots, n-1$.  Applying the $n=1$ case to $\psi$ gives
$$
\tilde{\psi}: (R[x_1, \dots, x_{n-1}])[x_n] \to S
$$
with $\tilde\psi|_{R[x_1, \dots, x_{n-1}]} = \psi$ and $\tilde{\psi}(x_n) = s_n$. Setting $\tilde\phi=\tilde\psi$  gives a map $\tilde{\phi}$ with the needed properties.
***

[^1]: See: [[Polynomial Ring]]