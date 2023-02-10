### Problem 6 – Strict Inequality of Automorphism Group
Assume $F \sse L$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] and that the [[Ring Characteristic|characteristic]] of $F$ is $p$, where p is a prime. Prove that if there exists an element $\a\in L\setminus F$ such that $\a^p \in F$ , then $|\Aut(L/F )| < [L : F ]$. You may use, without proof, the fact that $|\Aut(K/E)|\leq [K : E]$ for any finite extension of fields $E \sse K.$

##### *Proof*.
Let $F \sse L$ is a finite extension of fields and that the characteristic of $F$ is $p$, where $p$ is a prime, and suppose there exists an element $\a\in L\setminus F$ such that $\a^p \in F$. 

Consider the polynomial $f(x)=x^{p}-\a^p\in F[x]$, and notice that $f'(x)=px^{p-1}=0$, as we are in a field of characteristic $p$. However, this characteristic also yields $x^p-\a^p=(x-\a)^p$. As $F$ is a field we have $F[x]$ as a UFD, and thus as $x-\a$ is irreducible in $F[x]$ it is also prime. Therefore this is the unique factorization of $f$ up to associates. If $f$ was reducible $F$ it would thus have to be divisible into power os $x-\a$, which will never be reducible as $\a\not\in F$. Thus $f$ is irreducible in $F[x]$, making it the minimal polynomial of $\a$. However, if $|\Aut(L/F )|= [L : F ]$ this would make $L$ the splitting field of $f$ over $F$, which it is not, given $\a\not\in F$. Thus $|\Aut(L/F )| < [L : F ]$.
***
#qual