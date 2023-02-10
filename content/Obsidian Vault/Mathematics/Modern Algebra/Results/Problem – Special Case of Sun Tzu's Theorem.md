### Problem 4 – Special Case of Sun Tzu's Theorem
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] with [[Unital Ring|identity]], and assume $1\neq0$. Let $I$ and $J$ be [[Ideal|ideals]] such that $I + J = R$.

(a) Prove $IJ = I\cap J$.  
(b) Prove the following special case of the [[Theorem – Sunzi's Remainder Theorem|Sun Tzu's Theorem]]: There is an [[Isomorphism|isomorphism]] of rings of the form $R/(I \cap J)\cong R/I \times R/J$.  

##### *Proof.*
Let $R$ be a commutative ring with identity, and assume $1\neq0$. Let $I$ and $J$ be ideals such that $I + J = R$.

###### Part (a)
First, note that both $IJ$ and $I\cap J$ are ideals (See: [[Modern Algebra#Proposition – $I+J, I cap J, IJ, bigcap_{ a in J} I_ a$ all Ideals|Proposition]]).

Let $x\in IJ$. Thus $x=\sum a_ib_j$, where each $a_i\in I$ and $b_j\in J$. As $I$ and $J$ are both ideals, each term in this sum is contained both in $I$ and $J$. Thus, by absorption, $x\in I\cap J$. Hence $IJ\subseteq I\cap J$.

Let $x\in I\cap J$. Thus $x\in I$ and $x\in J$. Note that as $I+J=R$, there exists some $a\in I$ and $b\in J$ such that $a+b=1$. So $x=x1=xa+xb$. As $x\in I\cap J$ we see that $x=ax+xb$, with $a,x\in I$ and $b,x\in J$. Thus $x\in IJ$, yielding $IJ=I\cap J$.
***
###### Part (b)

Let $f:R\to R/I\times R/J$  be defined by $f(x)=(x+I,x+J)$.

Notice that if $x\in I\cap J$, we have $f(x)=(I,J)$, and so $x\in\Ker(f)$. (See: [[Kernel]])
Let $x\in\Ker(f)$. Thus $x+I=I$ and $x+J=J$, and so $x\in I$ and $x\in J$. Hence $x\in I\cap J$, and so $\Ker(f)=I\cap J$.

Observe $$f(x+y)=((x+y)+I,(x+y)+J)=((x+I)+(y+I),(x+J)+(y+J))=((x+I),(x+J))+(y+I),(y+J))=f(x)+f(y),$$ making $f$ a [[Homomorphism|homomorphism]] of rings. 

Let $(a+I,b+J)\in R/I\times R/J$. As $R=I+J$, we can write $a$ and $b$ as $a_i+a_j$ and $b_i+b_j$. However, as $a_i\in I$ and $b_j\in J$, we have $(a+I,b+J)=(a_j+I, b_i+J)$. 

Consider the element $x=(a_j+b_i)\in R$, and observe $$f(x)=f(a_j+b_i)=(a_j+b_i+I, b_i+a_j+J).$$However, as $b_i\in I$ and $a_j\in J$, we see $$(a_j+b_i+I, b_i+a_j+J)=(a_j+I,b_i+J)=(a+I,b+J).$$
Thus $f$ is a surjective homomorphism. Hence, by the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]], we see $R/(I \cap J)\cong R/I \times R/J$.
***

### Problem 4 – Special Case of Sun Tzu's Theorem
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] with [[Unital Ring|identity]], and assume $1\neq0$. Let $I$ and $J$ be [[Ideal|ideals]] such that $I + J = R$.

(a) Prove $IJ = I\cap J$.  
(b) Prove the following special case of the [[Theorem – Sunzi's Remainder Theorem|Sun Tzu's Theorem]]: There  
is an [[Isomorphism|isomorphism]] of rings of the form $R/(I \cap J)\cong R/I \times R/J$.  

##### *Proof.*
Let $R$ be a commutative ring with identity, and assume $1\neq0$. Let $I$ and $J$ be ideals such that $I + J = R$.

###### Part (a)
First, note that both $IJ$ and $I\cap J$ are ideals (See: [[Proposition – Combinations of Ideals|Result]]).

Let $x\in IJ$. Thus $x=\sum a_ib_j$, where each $a_i\in I$ and $b_j\in J$. As $I$ and $J$ are both ideals, each term in this sum is contained both in $I$ and $J$. Thus, by absorption, $x\in I\cap J$. Hence $IJ\subseteq I\cap J$.

Let $x\in I\cap J$. Thus $x\in I$ and $x\in J$. Note that as $I+J=R$, there exists some $a\in I$ and $b\in J$ such that $a+b=1$. So $x=x1=xa+xb$. As $x\in I\cap J$ we see that $x=ax+xb$, with $a,x\in I$ and $b,x\in J$. Thus $x\in IJ$, yielding $IJ=I\cap J$.
***
###### Part (b)

Let $f:R\to R/I\times R/J$  be defined by $f(x)=(x+I,x+J)$.

Notice that if $x\in I\cap J$, we have $f(x)=(I,J)$, and so $x\in\Ker(f)$. (See: [[Kernel]])
Let $x\in\Ker(f)$. Thus $x+I=I$ and $x+J=J$, and so $x\in I$ and $x\in J$. Hence $x\in I\cap J$, and so $\Ker(f)=I\cap J$.

Observe $$f(x+y)=((x+y)+I,(x+y)+J)=((x+I)+(y+I),(x+J)+(y+J))=((x+I),(x+J))+(y+I),(y+J))=f(x)+f(y),$$ making $f$ a [[Homomorphism|homomorphism]] of rings. 

Let $(a+I,b+J)\in R/I\times R/J$. As $R=I+J$, we can write $a$ and $b$ as $a_i+a_j$ and $b_i+b_j$. However, as $a_i\in I$ and $b_j\in J$, we have $(a+I,b+J)=(a_j+I, b_i+J)$. 

Consider the element $x=(a_j+b_i)\in R$, and observe $$f(x)=f(a_j+b_i)=(a_j+b_i+I, b_i+a_j+J).$$However, as $b_i\in I$ and $a_j\in J$, we see $$(a_j+b_i+I, b_i+a_j+J)=(a_j+I,b_i+J)=(a+I,b+J).$$
Thus $f$ is a surjective homomorphism. Hence, by the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]], we see $R/(I \cap J)\cong R/I \times R/J$.
***
#qual