#### $\lem$ – Transcendence Basis Well-Defined 1
Let $\{x_1,\dots,x_m\}$ and $\{y_1,\dots,y_n\}$ be two [[Transcendence Basis|transcendence bases]] for $L$ over $K$. Then, there is some $i$ such that $\{x_i,y_2,\dots,y_n\}$ is a transcendence basis.

##### *Proof.*
Since $L$ is algebraic over $K(y_1,\dots,y_n)$, for each $i$ there is some $p_i(t)\in K(y_1,\dots,y_n)[t]$ such that $p_i(x_i)=0$. We can clear denominators to assume without loss of generality that $p_i(x_i)\in K[y_1,\dots,y_n][t]$. 

We claim that there is some $i$ such that $p_i(t) \notin K[y_2,\dots,y_n][t]$. If not, then $$p_i(t) \in K[y_2,\dots,y_n][t]$$for all $i$, and thus that each $x_i$ is algebraic over $K(y_2,\dots,y_n)$. Thus, $K(x_1,\dots,x_m)$ is algebraic over $K(y_2,\dots,y_n)$, and since $L$ is algebraic over $K(x_1,\dots,x_m)$, $y$ is algebraic over $K(y_2,\dots,y_n)$, which contradicts that $\{y_1,\dots,y_n\}$ is a transcendence basis. This shows the claim.

Now, we claim that for such $i$, $\{x_i,y_2,\dots,y_n\}$ is a transcendence basis. Thinking of the equation $p_i(x_i)=0$ as a polynomial expression in $K[x_i,y_2,\dots,y_n][y_1]$, $y_1$ is algebraic over $K(x_i,y_2,\dots,y_n)$, hence $K(y_1,\dots,y_n)$ is algebraic over $K(x_i,y_2,\dots,y_n)$, and $L$ as well.

If $\{x_i,y_2,\dots,y_n\}$ were algebraically dependent, then there is some polynomial equation $p(x_i,y_2,\dots,y_n)=0$. This equation must involve $x_i$, since $y_2,\dots,y_n$ are algebraically independent. We would then have $K(x_i,y_2,\dots,y_n)$ is algebraic over $K(y_2,\dots,y_n)$. But since  $y_1$ is algebraic over $K(x_i,y_2,\dots,y_n)$, we would have that $K(y_1,\dots,y_n)$ is algebraic over $K(y_2,\dots,y_n)$, which would contradict that $y_1,\dots,y_n$ is a transcendence basis.