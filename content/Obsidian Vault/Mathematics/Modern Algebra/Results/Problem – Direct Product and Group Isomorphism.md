### Problem 1 – Direct Product and Group Isomorphism
Let $G$ be a (not necessarily finite) [[Group|group]] and $H$ and $K$ [[Normal Subgroup|normal]] [[Subgroup|subgroups]]  
such that $G = HK$[^1]. Prove that $G/(H\cap K)\cong G/H \times G/K.$[^2] 

##### *Proof.*
Let $f:G\to G/H\times G/K$ defined such that $f(g)=(gH, gK)$. Let $x,y\in G$. Then $$f(xy)=(xyH,xyK)=(xHyH,xKyK)=(xH,yH)\cdot(xKyK)=f(x)f(y),$$ showing $f$ is a [[Homomorphism|homomorphism]].

Let $(xH,yK)\in G/H\times G/K$. As $x,y\in G=HK$, we have $x=hk$ and $y=h'k'$ with $h,h'\in H$ and $k,k'\in K$. As $k'\in K$ and $h\in H$ we see $(xH,yK)=(kH,h'K)$. 

Consider $g=kh'\in G$ and $$f(g)=f(kh')=(kh'H,kh'K)=(kH,h'K)=(xH,yK),$$making $f$ surjective as well. 

Let $g\in H\cap K$. Then $f(g)=(gH,gK)=(H,K)$, and so $g\in\Ker(f)$. (See: [[Kernel]])
Let $g\in\Ker(f)$. Then $f(g)=(H,K)$, so $gH=H$ and $gK=K$, placing $g\in H\cap K$. Thus, by the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]], we have $G/(H\cap K)\cong G/H \times G/K.$
***
#qual

[^1]: Notation: [[HK]]
[^2]: Notation: [[Quotient Group]], [[Isomorphism]], [[Direct Product, Sum]]