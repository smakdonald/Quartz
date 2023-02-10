### Problem 5 – Eigenvalues and Linear Maps
Suppose that $T : V\to V$ is a [[Linear Transformation|linear map]], where $V$ is a [[Dim (Vector Space)|finite dimensional]] $\C$-[[Vector Space|vector space]]. Fix a polynomial $p\in \C[x]$[^1].

(a) Prove that if $\lambda$ is an eigenvalue of $T$ then $p(\lambda)$ is an eigenvalue of $p(T)$.
(b) Prove conversely that if $\mu$ is an eigenvalue of $p(T)$ then there exists an eigenvalue $\l$ of $T$ such that $\mu = p(\l)$.

##### *Proof*.

###### Part (a)
Let $\l$ be an eigenvalue of $T$. Thus there exists some $v$ such that $Tv=\l v$. 
Notice that $p(T)v=a_nT^nv+\dots+a_0Iv=0$ and $p(\l)=a_n\l^n+\dots+a_0$. 
Then $$\begin{align}(p(T)-p(\l I))v&=p(T)v-p(\l I)v\\&=(a_nT^nv+\dots+a_0Iv)-(a_n\l^nv+\dots+a_0v)\\&=a_n(T^n-\l^n)v+\dots a_0(I-I)v\\&=0,\end{align}$$making $p(\l)$ an eigenvalue of $p(T)$. 
***
###### Part (b) 
First note that if $T$ is a scalar of the identity matrix then its only eigenvalue is $0$. 
Let $\mu$ be an eigenvalue of $p(T)$. Thus $(p(T)-\mu I)v=0$ for some $v$. As $\C$ is algebraically closed we can factor the polynomial $p(x)-\mu$ into linear terms:
$$p(x)-\mu=c(x-r_1)\dots(x-r_n)$$for roots $r_i$. Note that $p(r_i)-\mu=0$ for all $r_i$. Observe $$\begin{align}(p(T)-\mu I)v&=p(T)v-(\mu I)v\\&=c(T-r_nI)\dots(T-r_1I)v\\&=0.\end{align}$$Thus one of these terms must be sent to zero. Note that if $T-r_iI=0$ for any $I$ this would make $T$ a scaler of the identity matrix. Thus there exists some $i$ such that $(T-r_iI)v=0$, making $r_i$ an eigenvalue of $T$. Notice that as $p(r_i)-\mu=0$ we have $p(r_i)=\mu$, completing the proof. 
***
#qual

[^1]: Notation: [[Polynomial Ring]]