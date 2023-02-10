### Problem 4 – Positive Quartic and Basis
Let $E$ be the [[Splitting Field|splitting field]] of $x^4 + 7 \in \Q[x].$
(a) Prove that $\sqrt[4]{28}\in E$.
(b) Find a [[Basis and Free Module|basis]] for $E$ as a $\Q$-[[Vector Space|vector space]].

##### *Proof.*
Let $E$ be the splitting field of $f(x)=x^4 + 7 \in \Q[x].$
###### Part (a) 
The roots of $f$ are the following:
1. $\a_{1}=\sqrt[4]{7}e^{\frac{\pi i}{4}}=\sqrt[4]{7}(\cos(\frac{\pi}{4})+i\sin(\frac{\pi}{4}))=\sqrt[4]{7}\cdot \frac{\sqrt{2}}{2}(1+i)=\frac{\sqrt[4]{28}}{2}(1+i)$
2. $\a_{2}=\sqrt[4]{7}e^{\frac{3\pi i}{4}}=\sqrt[4]{7}(\cos(\frac{3\pi}{4})+i\sin(\frac{3\pi}{4}))=\sqrt[4]{7}\cdot \frac{\sqrt{2}}{2}(-1+i)=\frac{\sqrt[4]{28}}{2}(-1+i)$
3. $\a_{3}=\sqrt[4]{7}e^{\frac{5\pi i}{4}}=\sqrt[4]{7}(\cos(\frac{5\pi}{4})+i\sin(\frac{5\pi}{4}))=\sqrt[4]{7}\cdot \frac{\sqrt{2}}{2}(-1-i)=\frac{\sqrt[4]{28}}{2}(-1-i)$
4. $\a_{4}=\sqrt[4]{7}e^{\frac{7\pi i}{4}}=\sqrt[4]{7}(\cos(\frac{7\pi}{2})+i\sin(\frac{7\pi}{2}))=\sqrt[4]{7}\cdot \frac{\sqrt{2}}{2}(1-i)=\frac{\sqrt[4]{28}}{2}(1-i)$
Notice that $\a_1+\a_4=\sqrt[4]{28}$, and thus $\sqrt[4]{28}\in E$.
***
###### Part (b) 
The polynomial $g(x)=x^4-28$ is irreducible in $\Q[x]$ by Eisenstein's Criterion ($p=7$). Thus it is the minimal polynomial of $\sqrt[4]{28}$, and so $F=\Q(\sqrt[4]{28})$ is a field extension of $\Q$ of degree $4$. After adjoining $i$ as well we see that $E$ is an extension of degree $8$. Thus a basis of $E$ as a $\Q$-vector space is the following: $$\{1,\sqrt[4]{28},\sqrt[4]{28}^2,\sqrt[4]{28}^3,i,\sqrt[4]{28}i,\sqrt[4]{28}^2i,\sqrt[4]{28}^3i\}$$
***
#qual