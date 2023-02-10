### Problem 3 – Order 225, Element of Order 25
Let $G$ be a [[Group|group]] of [[Order|order]] $175 = 3^2\cdot 5^2$ and suppose $G$ contains an element of order $25$. Prove that $G$ is [[Abelian Group|abelian]].

###### *Proof*
First, note that $3^2\cdot 5^2=225$, not $175$. You hate to see it.
Anyway, let $x$ be an element of order $25$ and consider $H=\langle x\rangle$, a cyclic subgroup of order $25$. The possible number of Sylow $5$-subgroups of $G$ is exactly $1$, making $H$ this subgroup and thus normal in $G$. Let $K$ be a Sylow $3$ subgroup, it intersects $H$ trivially and thus $G\cong H\sdp_{\rho}K$, where $\rho:K\to\Aut(H)$. The order of $\Aut(H)$ is $20$, which is relatively prime to $|K|$, making $\rho$ trivial and $G=H\times K$ and thus abelian. 
***
#qual