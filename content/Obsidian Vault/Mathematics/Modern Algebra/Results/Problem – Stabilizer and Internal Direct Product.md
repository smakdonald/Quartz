### Problem 3 – Stabilizer and Internal Direct Product
Let $G$ be a [[Group|group]] that [[Group Action|acts]] on a set $A$, and $H$ a [[Subgroup|subgroup]] of $G$ such that for any $a, b \in A$ there exists a unique $h \in H$ with $ha = b$.

(a) Prove that for every $a \in A, G = HG_a$[^1] and $H \cap Ga = \{1\}$, where $G_a = \{g \in G | ga = a\}.$
(b) Prove that if $H \subseteq Z(G)$[^2] then for every $a \in A$, $G$ is the [[Internal, External Direct Product|internal direct product]] of $H$ and $G_a.$

##### *Proof.*
Let $G$ be a group that acts on a set $A$, and $H$ a subgroup of $G$ such that  
for any $a, b \in A$ there exists a unique $h \in H$ with $ha = b$.

###### Part (a)
Suppose there exists some $h\in H$ such that $h\in G_a$. Then $ha=a$. But $ea=a$ by the definition of group action. As the $h\in G_a$ is unique, we see $h=e$. Thus $H\cap G_a=\{e\}$. 

Let $g\in G$ and $a\in A$. If $g\in H$ then we can write $g=ge$, as $e\in G_a$. Suppose $g\not\in H$ and $ga=b$ for some $b\in A$. There exists an $h\in H$ such that $ha=b$. Then $ha=ga$, so  $h\inv g a=a$, so $h\inv g\in G_a$. Thankfully, we can know write $g=h(h\inv g$), and so $G=HG_a$.  
***
###### Part (b)
If $H\subseteq Z(G)$ then we have $HG_a=G_aH$, which means $HG_a\leq G$. From Part (a) we have a trivial intersection, making $G$ the internal direct product of $H$ and $G_a$. 
***
#qual

[^1]: Notation: [[HK]]
[^2]: Notation: [[Center]]