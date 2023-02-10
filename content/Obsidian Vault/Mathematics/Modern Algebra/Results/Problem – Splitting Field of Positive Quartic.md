### Problem 7 – Splitting Field of Positive Quartic
Let $E$ be the [[Splitting Field|splitting field]] of $x^4 + 5$ over $\Q$.
(a) Prove, by adding two appropriate roots of $x^4 + 5$ or otherwise, that there exists $\Q\subseteq F\subseteq E$ such that $F \sse \R$ and $[F : \Q] = 4$[^1].
(b) Determine, with justification, $[E : \Q]$.

##### *Proof*.
Let $E$ be the splitting field of $f(x)=x^4 + 5$ over $\Q$.

###### Part (a)
First, we note that the roots of $f$ are the following:
$\a_1=\sqrt[4]5e^{\pi i/4}=\sqrt[4]5 (\cos(\frac{\pi}{4}))+i\sin(\frac{\pi}{4}))=\sqrt[4]5(\frac{\sqrt 2}{2}+i\frac{\sqrt 2}{2})=\frac{\sqrt 2}{2}\sqrt[4]5(1+i)=\frac{\sqrt[4]{20}}{2}(1+i),$
$\a_2=\sqrt[4]5e^{3\pi i/4}=\sqrt[4]5 (\cos(\frac{3\pi}{4}))+i\sin(\frac{3\pi}{4}))=\sqrt[4]5(\frac{-\sqrt 2}{2}+i\frac{\sqrt 2}{2})=\frac{\sqrt 2}{2}\sqrt[4]5(-1+i)=\frac{\sqrt[4]{20}}{2}(-1+i),$
$\a_3=\sqrt[4]5e^{5\pi i/4}=\sqrt[4]5 (\cos(\frac{5\pi}{4}))+i\sin(\frac{5\pi}{4}))=\sqrt[4]5(\frac{-\sqrt 2}{2}+i\frac{-\sqrt 2}{2})=\frac{\sqrt 2}{2}\sqrt[4]5(-1-i)=\frac{\sqrt[4]{20}}{2}(-1-i),$ and
$\a_4=\sqrt[4]5e^{7\pi i/4}=\sqrt[4]5 (\cos(\frac{7\pi}{4}))+i\sin(\frac{7\pi}{4}))=\sqrt[4]5(\frac{\sqrt 2}{2}+i\frac{-\sqrt 2}{2})=\frac{\sqrt 2}{2}\sqrt[4]5(1-i)=\frac{\sqrt[4]{20}}{2}(1-i).$
First we examine $F=\Q(\sqrt[4]{20})$. Notice that $\sqrt[4]{20}$ is a root of the polynomial $x^4-20$, which is [[Irreducible|irreducible]] in $\Q[x]$ using [[Theorem – Eisenstein's Criterion|Eisenstein's Criterion]] with $p=5$. Thus $x^4-20$ is monic and irreducible, making it the [[Minimum Polynomial|minimal polynomial]] of $\sqrt[4]{20}$. Thus $[F:\Q]=4$. Notice that $\a_1+\a_4=\frac{\sqrt[4]{20}}{2}(1+i+1-i)=\sqrt[4]{20}$, so $\sqrt[4]{20}\in E$. Thus there exists $\Q\subseteq F\subseteq E$ such that $F \sse \R$ and $[F : \Q] = 4$.
***
###### Part (b)
Now let $K=F(i)$. Notice that $i$ is a root of the polynomial $x^2+1$, which is irreducible in $F[x]$ as $F\subseteq\R$ and $i\not\in\R$.  Thus $x^2+1$ is monic and irreducible, making it the minimal polynomial of $i$ Thus $[K:F]=2$ and $[K:\Q]=8$ by the [[Proposition – The Degree Formula|Degree Formula]]. 

Notice that $\a_1+\a_4=\frac{\sqrt[4]{20}}{2}(1+i+1-i)=\sqrt[4]{20}$, so $\sqrt[4]{20}\in E$. Thus so is $\frac{1}{\sqrt[4]{20}}$, and so we see that $i=\a_1\cdot\frac{1}{\sqrt[4]{20}}-1$, and thus that $i\in E$ as well, making $K\subseteq E$. As seen in Part (a), each root can be expressed in terms of $i$ and $\sqrt[4]{20}$, and so $E\subseteq K$ as well. Hence $K=E$ and we have $[E : \Q]=[K:\Q]=8$.
***
#qual

[^1]: Notation: [[Degree of Field Extension]]