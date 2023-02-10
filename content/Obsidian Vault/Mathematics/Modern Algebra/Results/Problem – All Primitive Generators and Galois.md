### Problem 4 – All Primitive Generators and Galois
Let $L$ be the [[Splitting Field|splitting field]] over $\Q$ of the polynomial $x^3-7$.
(a) Find all [[Intermediate Field|intermediate fields]] $E$ with $\Q \sse E \sse L$ (including possibly $L$ and $\Q$) such that $E$ is Galois over $\Q$.
(b) For each [[Field|field]] $E$ you found in (a), find with justification a primitive generator (i.e., find $\a \in E$ so that $E = \Q(\a))$.

##### *Proof.*
Let $L$ be the splitting field over $\Q$ of the polynomial $f(x)=x^3-7$

###### Part (a) 
First, notice that $f$ is irreducible in $\Q[x]$ by Eisenstein's Criterion $(p=7)$. Let $\z$ denote a primitive third root of unity. The roots of $f$ are the following:
1. $\a_1=\sqrt[3]{7}\z$,
2. $\a_2=\sqrt[3]{7}\z^2$, and 
3. $\a_3=\sqrt[3]{7}\z^3=\sqrt[3]{7}$.
As $f$ is irreducible and monic we see that it is the minimum polynomial of $\a_3$ over $\Q$. Let $E_1=\Q(\a_3)$ and notice $[E_1:\Q]=3$. 

Recall that $G=\Gal(L/\Q)$ is isomorphic to a subgroup of $S_3$. As $E_1\sse \R$ and $\a_1\not\in\R$, we see another extension is needed, and that extension will have at least degree $2$. Thus, due to size constraints, we see $G\cong S_3$. 

By the FTGT each Galois intermediate extension between $\Q$ and $L$ corresponds to a normal subgroup of $G$, which are the normal subgroups of $S_3$. 

The elements of $S_3$ are the following:
1. $(1)$
2. $(12)$
3. $(13)$
4. $(23)$
5. $(123)$
6. $(132)$
The subgroup $F=\langle(123)\rangle=\{(123),(132)\}$ has index $2$ in $G$ and is thus normal. None of the order $2$ subgroups are normal in $S_3$, so $F$ is the only strictly intermediate extension. 

Recall $[E_1:\Q]=3$, meaning $|\Gal(L/E_1)|=3$, so $E$ corresponds to a subgroup of order $2$ in $G$, so its not Galois unfortunately. However, $E_2=\Q(\z)$ is a degree $2$ extension that is an intermediate field, as $\z$ is a root of the irreducible polynomial $x^2+x+1$. 

With all this in mind, notice:
- $\Q$ is a splitting field of $\Q$, and has the primitive generator by $1$. 
- $E_2$ is our only strictly intermediate field, and has the primitive generator $\z$
- Finally, $L$ is Galois over $\Q$, and has the primitive generator $\z+\sqrt[3]{7}$. 
***
###### Part (b) 
***
#qual