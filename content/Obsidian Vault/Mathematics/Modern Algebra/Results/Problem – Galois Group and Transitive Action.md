### Problem 5 – Galois Group and Transitive Action
Let $E/F$ be a [[Degree of Field Extension|finite]] [[Galois Extension|Galois extension]] and let $G$ be the [[Galois Extension|Galois group]] of $E/F$.  
Suppose that $E = F (\a)$ and let $f(x)$ be the [[Minimum Polynomial|minimal polynomial]] of $\a$ over $F$ . Prove that
$$f(x) =\prod_{\s\in G} (x-\s(\a)).$$
###### *Proof*.
Let $E/F$ be a finite Galois extension and let $G$ be the Galois group of $E/F$. Suppose that $E = F (\a)$ and let $f(x)$ be the minimal polynomial of $\a$ over $F$. Thus $G$ acts on the roots of $f$ faithfully. Additionally, as $f$ is the minimal polynomial of $\a$ it is irreducible, making the action transitive as well. 

As $E$ is Galois over $F$ we know that $f$ splits into linear factors, each of the form $x-\b$, where $\b$ is a root of $f$. As our action is transitive, for every root $\b$ there exists a $\s\in G$ such that $\s\cdot\a=b$, or $\s(\a)=\b$. 
***
#qual