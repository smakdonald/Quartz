#### $\thm$ – Finding Groups with Semidirect Products
If $H$ and $K$ are [[Group|groups]] and $\rho:K\to \Aut(H)$[^1] is a [[Homomorphism|homomorphism]], then setting: 
1. $H \sdp_\rho K$[^2] is a group
2. $H\cong H':=\{(h,e)\mid h\in H\}\norm H \sdp_\rho K$[^3] and $K\cong K':=\{(e,k)\mid k\in K\}\leq H \sdp_\rho K$
3. $(H \sdp_\rho K )/ H' \cong K$[^4].

###### *Proof.* 
(1.) The proof is straightforward but a bit messy. For associativity, note that
$$\begin{align*}
(y_1,x_1) \left( (y_2, x_2) (y_3, x_3) \right)
&=(y_1,x_1) (y_2\rho(x_2)(y_3), x_2x_3)
=
(y_1\rho(x_1)\left(y_2\rho(x_2)(y_3)\right), x_1x_2x_3)\\
&=
(y_1\rho(x_1)(y_2)(\rho(x_1)\circ \rho(x_2))(y_3), x_1x_2x_3)\\
&=
(y_1\rho(x_1)(y_2)\rho(x_1x_2)(y_3), x_1x_2x_3)\\
\end{align*}$$
On the other hand
$$\begin{align*}
\left( (y_1,x_1) (y_2, x_2) \right) (y_3, x_3) 
& = (y_1 \rho(x_1)(y_2), x_1 x_2)  (y_3, x_3) 
= (y_1 \rho(x_1)(y_2)\rho(x_1x_2)(y_3), x_1 x_2 x_3).
\end{align*}$$
This gives associativity.

The fact that $(e,e)$ is a two-sided identity follows from the fact that $\rho(e)(y) = \id_H(y)=y$.

Finally
$$\begin{align*}
(y,x) (\rho(x^{-1})(y^{-1}) ,x^{-1}) &= (y \rho(x)\left(\rho(x^{-1})(y^{-1}) \right), e)
= (y (\rho(x)\circ\rho(x^{-1}))(y^{-1}), e) 
\\ &= (y \rho(e)(y^{-1}), e) = (yy^{-1},e)=(e,e),
\end{align*}$$
and similarly
$$
(\rho(x^{-1})(y^{-1}) ,x^{-1})  (y,x) = (e,e).
$$

(2.) Define a function
$$
i: H \to H \sdp_\rho K
$$
as $i(y) = (y, e)$. Then $i$ is a  homomorphism, since
$$
i(y_1) i(y_2) = (y_1,e)(y_2,e) = (y_1\rho(e)(y_2) , ee) = (y_1 y_2, e) = i(y_1y_2).
$$
The map is clearly injective and hence its image is isomorphic to $H$. 
In fact, the image is normal since the second component of
$$
(y,x) (y_2, e) (\rho(x^{-1})(y^{-1}), x^{-1})
$$
is clearly $e$. 
Let us write this image as
$$
H' := \{(y,e) \mid y \in H\} \nsg  H \sdp_\rho K.
$$


The function
$$
j: K \to H \sdp_\rho K
$$
defined by $j(x) = (e,x)$ is also an injective homomorphism and thus its image 
$$
K' := \{(e,x) \mid x \in H \} \leq H \sdp_\rho K
$$
is isomorphic to $K$. $K'$ is typically {\em not} normal, however.
Finally, it is easy to see that $H'K'= H \sdp_\rho K$ and $H' \cap K' = \{e\}$. Putting this all together we have

$H' \nsg  H \sdp_\rho K$, 
$K' \leq H \sdp_\rho K$,
$H' K' = H \sdp_\rho K$, and 
$H'\cap K' = \{e\}$. 

(3.) Consider the projection onto the second factor $\pi_2:H \sdp_\rho K \to  K$ given by $\pi_2(y,x)=x$.
This is a group homomorphism since the second component of $(y_1,x_1)(y_2,x_2)$ is $x_1x_2$ and is surjective by definition. Now $$\ker(\pi_2)=\{(y,e_K)\mid y\in H\}=H'\cong H.$$
By the first isomorphism theorem we conclude that $(H \sdp_\rho K )/ H' \cong K$.
***

[^1]: See: [[Automorphism]]
[^2]: See: [[External Semidirect Product]]
[^3]: See: [[Isomorphism]], [[Normal Subgroup]]
[^4]: See: [[Quotient Group]]