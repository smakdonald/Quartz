### Problem 8 – Algebraic but not Finite Extension
(a) Show that any [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] $K/F$ is [[Algebraic Extension|algebraic]].
(b) Let $\overline{\Q}$ denote the [[Subring|subfield]] of $\C$ consisting of all the complex numbers which are [[Algebraic Element|algebraic]] over $\Q$. (You may use that $\overline{\Q}$ is a field without proof.) Show that $\overline{\Q}/\Q$ is an algebraic extension, but not a finite extension.

##### *Proof*.
###### Part (a) 
Let $K/F$ be a finite extension of fields. Let $\a\in L$. By the [[Proposition – The Degree Formula|Degree Formula]] we have $[K:F(a)]=[K:F(\a)][F(\a):F]$[^1]. Thus $[F(\a):F]$ is finite, making $\a$ algebraic over $F$.
***
###### Part (b)
Notice that $\a_n\sqrt[n]2\in\overline{\Q}$ for all $n\in\N$ and that $\a_n$ is a root of the polynomial $x^n-2$, which is [[Irreducible|irreducible]] in $\Q[x]$ by [[Theorem – Eisenstein's Criterion|Eisenstein's Criterion]] ($p=2$). Thus $[\Q(\a_n):\Q]=n$. As $\a_n$ must be added to $\Q$ for all $n$, we see that this extension is not finite. 
***
#qual

[^1]: See: [[Degree of Field Extension]]