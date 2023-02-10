### Problem 4 – Prime Degree and Splitting Field
Let $F$ be a [[Field|field]] of [[Ring Characteristic|characteristic]] $p > 0$, $a \in F$ , and  consider the polynomial $f(x)=x^p -x-a \in F[x]$[^1].

(a) Prove that $f(x)$ is either irreducible over $F$ or it splits into distinct linear factors over $F$. (*Hint*: If $\alpha$ is a root of $f(x)$,  consider $\alpha + j$ for $j \in \Z/p$.)
(b) Suppose $f(x)$ is irreducible over $F$ and let $L$ be a splitting field of $f$ over $F$. Prove that the Galois group of $L$ over $F$ is cyclic.

##### *Proof.*
Let $F$ be a field of characteristic $p > 0$, $a \in F$ , and  consider the polynomial $f(x)=x^p -x-a \in F[x]$.

###### Part (a) 
Suppose $f$ has a root, $\alpha$, in $F$. Then $\alpha^p-\alpha-a=0$. Consider $\alpha+j$ for some $j\in\Z/p$, and observe $(\alpha+j)^p-(\alpha+j)-a$. By The Freshman's Dream, we have $\alpha^p+j^p-\alpha-j-a$, but as $\alpha^p-\alpha-a=0$, we really have $j^p-j$. By Fermat's Little Theorem, $p|j^p-j$, and thus $f(\alpha+j)=0$. Thus we have found $p$ roots of $f$, and thus $f$ splits into linear factors. 

Suppose then that no root of $f$ exists in $F$. Let $L$ be a splitting field of $f$ over $F$, and note that from the above paragraph we have $L=F(\alpha)$. As $f'(x)=1$, we see $\gcd(f,f')=1$, and thus $f$ is separable. Hence $F(\alpha)$ is a Galois extension. Thus there exists a $\sigma\in\Gal(L/F)$ such that $\sigma(\alpha)\neq\alpha$. So $\sigma(\alpha)=\alpha+j$ for some $j\in\Z/p$. Notice $\sigma(\alpha+j)=\sigma(\alpha)+j=\alpha+2j$. As $p$ is prime, we see that $|j|=p$, and thus we need to apply $\sigma$ to $\alpha$ $p$ times in order to get back to $\alpha$. Thus $\sigma(\alpha)^p=\alpha$, so $|\sigma|=p$. Thus $|\Gal(L/F)|=p$. Thus the minimum polynomial of $\alpha$ must have degree $p$. As $\alpha$ is a root of $f$ and $f$ is monic, it must be the minimal polynomial and is thus irreducible.
***
###### Part (b) 
Suppose $f(x)$ is irreducible over $F$ and let $L$ be a splitting field of $f$ over $F$. Let $\alpha$ be a root of $f.$ Consider $F(\alpha)$. By part (a), $F(\alpha)$ contains all the roots of $f$, hence $L=F(\alpha)$. As $f$ is monic and irreducible, it is the minimum polynomial of $f$, and thus $[L:F]=p$. Hence $|\Gal(L/F)|=p$. All groups of prime order are cyclic, completing the proof.
***
#qual

[^1]: Notation: [[Polynomial Ring]]