#### $\defn$ – Field Extension
A *field extension* is an [[Inclusion Map|inclusion]] of one [[Field|field]] $F$ into a larger field $L$, making $F$ into a subfield of $L$. We will write either $F \subseteq L$ or $L/F$ to signify that $L$ is a field extension of $F$.
***
#### $\defn$ – Elemental Field Extension
Given a [[Field|field]] [[Field Extension|extension]] $F \subseteq L$ and an element $\a \in L$, set $$F[\a] = \{f(\a) \mid f(x) \in F[x]\}.$$Then $F[\a]$ is a [[Subring|subring]] of $L$ and in fact it is the smallest subring of $L$ that contains $F$ and $\a.$
We define $F(\a)$ to be the [[Field of Fractions|field of fractions]] of $F[\a]$; that is,
$$F(\a) = \left\{\frac{f(\a)}{g(\a)} \mid f(x), g(x) \in F[x] \text{ such that $g(\a) \ne 0$} \right\}.$$
So, $F(\a)$ is a subfield of $L$ and it is the smallest subfield of $L$ that contains $F$ and $\a$.
***
#### $\defn$ – Generated Subfield
If $F \subseteq L$ is a [[Ring|field]] [[Field Extension|extension]] and $A$ is any subset of $L$, we write $F(A)$ for the smallest subfield of $L$ that contains all of $F$ and $A$ and it is called the *subfield generated* by $A$ over $F$. Since the intersection of any two subfields of $L$ is again a subfield, $F(A)$ exists and is
$$
F(A) = \bigcap_{\text{$E$ is a subfield of $L$ such that $E \supseteq F \cup A$}} E.
$$
where $E$ 
Nearly always $A$ will be a finite set, $A = \{a_1, \dots, a_n\}$, and we write $F(a_1, \dots, a_n)$ for $F(A)$.

In this case, we have 
$$
F(a_1, \dots, a_n) = \left\{ \frac{p(a_1, \dots, a_n)}{q(a_1, \dots, a_n)} \mid p, q \in F[x_1, \dots, x_n], q(a_1, \dots, a_n) \ne 0\right\}.
$$
***