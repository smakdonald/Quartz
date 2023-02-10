### Problem 9 – Primitive Sixth Root of Unity (2)
Let $p = x^6 + 3 \in \Q[x]$, and let $L$ be its [[Splitting Field|splitting field]] over $\Q$. Prove that if $\a$ is a root of $p$ then $L = \Q(\a)$. Hence (or otherwise) determine $[L : Q]$. (Hint: Consider the value of  $\a_3$.)

###### *Proof*.
Let $p = x^6 + 3 \in \Q[x]$, and let $L$ be its splitting field over $\Q$ and suppose $\a$ is a root of $p$. Note that $(\frac{\a^3+1}{2})^2=\frac{\a^3-1}{2}$, and so $$\left(\frac{\a^3+1}{2}\right)^6=\left(\left(\frac{\a^3+1}{2}\right)^2\right)^3=\left(\frac{\a^3-1}{2}\right)^3=1,$$making $\a$ a primitive sixth root of unity. By squaring primitive sixth roots of unity over and over we get all of the other sixth roots of unity as well, and so $e^{2\pi i/6}\in L$. Thus we have all the roots of $p$, and so $L=\Q(a)$ and $[L:\Q]=6$.
#qual