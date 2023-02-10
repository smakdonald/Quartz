### Problem 1 – Characteristic Subgroup and Normality
Let $G$ be a [[Group|group]]. A [[Subgroup|subgroup]] $H$ of $G$ is called a *characteristic subgroup* of $G$ if $\a(H)=H$ for every [[Automorphism|automorphism]] $\a$ of $G$. Show that if $H$ is a characteristic subgroup of $N$ and $N$ is a [[Normal Subgroup|normal subgroup]] of $G$, then $H$ is a normal subgroup of $G$.

##### *Proof.*
Let $G$ be a group, $N$ is a normal subgroup of $G$, and $H$ a characteristic subgroup of $N$. 
Let $g\in G$ and consider the automorphism $a_g:G\to G$ given by $a_g(g')=gg'g^{-1}$. 

Let $n\in N$ and notice $a_g(n)=gng\inv\in N$, as $N\nsg G$. Thus $a_g:N\to N$ is well defined. Let $n\in N$. As $gNg\inv=N$, we can write $n=gn'g\inv$ for some $n'\in N$. Then $a_g(n')=gn'g\inv=n$, making $a_g$ surjective. As $|N|=|N|$ we see that $a_g$ is a bijection. The homomorphism piece we get for free from $G$, making $a_g\in\Aut(N)$. 

Let $h\in H$. As $H$ is a characteristic subgroup of $N$, we see that $a_g(h)=ghg\inv=h$ for all $h\in H$ and for all $g\in G$. Thus $H$ is normal in $G$. 
***
#qual