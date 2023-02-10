### Problem 9 – Primitive Sixth Root of Unity
Consider $f(x) = x^6 + 3 \in \Q[x]$.
(a) Let $a$ be a root of $f(x)$ and prove $\Q(a)$ is a [[Galois Extension|Galois field extension]] of $\Q$. (Hint: First show $\frac{a^3+1}2$ is primitive $6$-th root of unity.)
(b) Find the [[Galois Extension|Galois group]] $\Gal(\Q(a)/\Q)$.

##### *Proof.*
Consider $f(x) = x^6 + 3 \in \Q[x]$.
###### Part (a) 
Let $a$ be a root of $f(x)$. Note that $(\frac{a^3+1}{2})^2=\frac{a^3-1}{2}$, and so $$(\frac{a^3+1}{2})^6=((\frac{a^3+1}{2})^2)^3=(\frac{a^3-1}{2})^3=1,$$so yay! It's primitive. Using one $6$th primitive root we can obtain all the others, specifically $e^{2\pi i/6}$. So we multiply each root by this to get all the others. So we have our splitting field. 
***
###### Part (b) 
Since $\Q(a)$ is Galois, we see that $[\Q(a):\Q]=6$. So $\Gal(\Q(a)/\Q)$ is either $S_3$ or $\Z/6.$ 
The roots of $f$ are $\alpha_i=\sqrt[6]{3}e^{{(\pi i/6)}^{2i-1}}$ for $1\leq i\leq 6$. 

By the Porism there exists a $\sigma\in\Gal(\Q(a)/\Q)$ such that $\sigma(\alpha_1)=\alpha_2$. Let $\zeta=e^{\pi i/3}$, and note that $\alpha_i=\alpha_{i-1}\zeta$. Additionally, note that $\frac{\alpha_i^3+1}{2}=\zeta$ when $i=1,3,5$ and $\frac{\alpha_i^3+1}{2}=\zeta^5$ when $i=2,4,6$. 

Observe then that $$\sigma(\alpha_2)=\sigma(\alpha_1)\sigma(\zeta)=\alpha_2\frac{\sigma(\alpha_1)^3+1}{2}=\alpha_2\zeta^5=\alpha_1.$$Similarly, we see that $\sigma(\alpha_3)=\alpha_6$ and $\sigma(\alpha_4)=\alpha_5$. Thus $\sigma$ corresponds to the permutation $(12)(36)(45)$.

Using the Porism again we see there exists a $\tau\in\Gal(\Q(a)/\Q)$ such that $\tau(\alpha_2)=\alpha_3$. Using a similar process as above we see that $\tau$ corresponds to $(14)(23)(46)$. However, observe that $\sigma\tau=(153)(264)$, while $\tau\sigma=(135)(246)$. Thus these elements do not commute, so we cannot be in $\Z/6$. Thus $\Gal(\Q(a)/\Q)\cong S_3$.
#qual