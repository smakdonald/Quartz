### Problem 1 – Subgroup of Squares and Cosets
Let $G$ be a [[Group|group]] (not necessarily [[Order|finite]]) and $H$ a nonempty subset of $G$ that is [[Multiplicatively Closed Set|closed under multiplication]]. Suppose that for all $g\in G$ we have $g^2\in H$. Prove the following:
(a) $H$ is a [[Subgroup|subgroup]] of $G$
(b) $H$ is [[Normal Subgroup|normal]]
(c) $G/H$ (See: [[Coset]]) is [[Abelian Group|abelian]].

##### *Proof.*
Let $G$ be a group, $H$ a multiplicatively closed subset of $G$, and suppose that $g^2\in H$ for all $g\in G$. 

###### Part (a)
First, notice that $e^2=e\in H$. Let $x\in H$, and consider $x\inv$. Notice that $(x{\inv})^2=x^{-2}\in H$. As $H$ is multiplicatively closed, we see that $xx^{-2}=x\inv\in H$. Thus $H$ is a subgroup of $G$ by the [[Lemma – Subgroup Tests|subgroup test]]. 
***
###### Part (b)
Let $g\in G$, $h\in H$, and consider $gh$. Notice that $(gh)^2=ghgh\in H$. Multiplying by $h\inv$ on the right we see $ghg\in H$, as it is multiplicatively closed and $h\inv\in H$. We rewrite $ghg=ghggg\inv=ghg\inv g^2$, given that elements always commute with their inverses. As $g^2\in H$, we see that $ghg\inv\in H$ as well. Thus $H$ is normal in $G$.
***
###### Part (c)
Let $x,y\in G/H$. As $g^2\in H$ for every $g\in G$, every element $G/H$ has order $2$.  Thus $xyxy=e$ and so $xy=(xy)\inv=yx$, making the group abelian.  
***
#qual