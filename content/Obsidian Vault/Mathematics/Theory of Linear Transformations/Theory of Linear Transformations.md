# Introduction
## Algebra
#### $\defn$ – Step
#### $\defn$ – Step Arithmetic
We consider the set of all steps in the plane, thought of as ordered pairs of real numbers: 
$$\R^2 = \setof{(x, y)}{x, y\in \R}.$$
Given steps $(x, y)$ and $(x',y')$ in $\R^2$ and a number $\l\in \R$ we define
$$\begin{align*}(x, y)+(x',y') &= (x+x',y+y') \\\l\,(x, y) &= (\l\,x, \l\, y).\end{align*}$$
#### $\ex$ – Linear Combination
If $\v=(x, y)$ and $\w=(x',y')$ are  steps in $\R^2$ and $\l,\mu \in \R$ then we say that 
$$\l\v + \mu\w = (\l x+\mu x', \l y+\mu y')$$
is a *linear combination* of $\v$ and $\w$. 
#### $\defn$
More generally if we have $n$ steps $\v_i=(x_i, y_i)$ and $n$ numbers $\l_i$ then we get a linear combination$$\Slv = \l_1\v_1 + \l_2\v_2 + \dots + \l_n\v_{n} = \parens[\Big]{ \sum_{i=1}^n \l_i x_i , \sum_{i=1}^n \l_i y_i }.$$
## Geometry
#### Exercise
Why is the set of solutions of the equation $x+2y = 6$ a line?

##### Solution:
If $x,y$ satisfy $x+2y = 6$  we can write $x=-2y+6$ and so
$$(x,y)=(-2y+6,y)=(6,0)+y(-2,1)$$
tells us the point $(x,y)$ can be reached by taking the step $(6,0)$ after which we move in the direction of the step $(2,-1)$ either forward of backward $|y|$ times the length of  $(2,-1)$.
### Dot Products
#### $\defn$ – Dot Product (Steps)
We define the *dot product* of steps $\u$ and $\w$ to be
$$\u \cdot \w = \abs{\u} \abs{\w} \cos(\t),$$
#### $\prop$ – Properties of the Dot Product
(1) the dot product is symmetric, i.e., $\u\cdot \w = \w \cdot \u$.  
(2) $\u$ and $\v$ are perpendicular if and only if $\u\cdot\v=0$
(3) $(\u+\v)\cdot \w=\u\cdot \w+\v\cdot \w$

##### Proof
(1) and (2) can be seen from the definition.
The third property follows is because we are simply scaling the lengths of $\u$ and $\v$ along the axis by a factor of $\abs{\w}$.  But since it's additive in $\u$ and symmetric, the dot product must also be additive in $\w$ as claimed in (4).
#### $\defn$
If $\u = (x, y)$ and $\w=(x', y')$ are vectors in $\R^2$ then we define their *dot product* to be 

$$\u \cdot \w = x x' + y y' = \abs{\u} \, \abs{\w} \cos(\t),$$
where $\t$ is the angle between $\u$ and $\v$ and $\abs{\u} , \abs{\w}$ denote the length of $\u$ and of $\w$. 
## Computation
## Vector Spaces
#### $\ex$
The set $\R^2=\setof{(x, y)}{x, y\in \R}$ is the set of all steps in the plane. We have seen how to take linear combinations of steps.
#### $\ex$
Similarly we can talk about vectors with more then two entries: $\R^3$ for instance, but also $\R^4$, $\R^5$, $\dots$, *etc*. Formally we have 
$$\R^n = \setof{(x_1, x_2, \dots, x_{n})}{x_1, x_2, \dots, x_{n} \in \R},$$
and we define
$$\begin{align*}
    (x_1, x_2, \dots, x_{n}) + (y_1, y_2, \dots, y_{n}) &= (x_1+y_1,x_2+y_2,\dots,x_n+y_n) \\
    \l\, (x_1, x_2, \dots, x_{n}) &= (\l\, x_1, \l\, x_2, \dots, \l\, x_{n}),
\end{align*}$$
where $\l$ is a real number.
#### $\ex$
We can go even further and think about sequences of infinite length, such as those that appear in calculus and analysis.$$\R^\N = \setof{(a_n)_{n\ge 0}}{\text{$\forall n\in \N$ we have $a_n\in \R$}} = \setof{a}{\text{$a$ is a function $\N\to \R$}}.$$We can add and scale such things in the natural way:
$$\begin{align*}(a_n)_{n\ge 0} + (b_n)_{n\ge 0} &= (a_n+b_n)_{n\ge 0} \\\l\, (a_n)_{n\ge 0} &= (\l a_n)_{n\ge 0}.\end{align*}$$
#### $\ex$
A *polynomial* with real coefficients is a function of the form $p(X)=a_dX^d+ a_{d-1}X^{d-1}+ \cdots +a_1X+a_0$, where $a_d, \ldots, a_0\in\R$. The set of all polynomials with real coefficients is denoted $$\R[X]=\{a_dX^d+ a_{d-1}X^{d-1}+ \cdots +a_1X+a_0 \mid a_0, \ldots, a_d\in \R\}.$$a vector space. We already know how to add polynomials and multiply them by real numbers. If $p$ and $q$ are polynomials with real coefficients and $\l\in \R$ then we have new polynomials $p+q$ and $\l\, p$ with
$$(p+q)(X) = p(X) + q(X) \quad\text{and}\quad (\l p)(X) = \l\, p(X).$$
We also know how to multiply  two polynomials together.  Eventually we'll talk about gadgets which are vector spaces and for which we can also multiply vectors together. Such things will be called *algebras*. For the moment though we're only concerned with scaling vectors---multiplying them by numbers.
#### $\ex$
If we define $M_{m\times n}(\R)$ to be the set of all $m\times n$ matrices with real entries then this forms a vector space.

$$M_{m\times n}(\R) = \setof*{\begin{bmatrix}a_{11} & a_{12} & \cdots & a_{1n} \\a_{21} & a_{22} & \cdots & a_{2n} \\\vdots & \vdots & \ddots & \vdots \\a_{m1} & a_{m2} & \cdots & \a_{m n}\end{bmatrix}}{\text{$\forall i, j$ we have $ a_{i j}\in \R$}}.$$

We add matrices of the same dimensions by
$$\begin{bmatrix}a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{m n}\end{bmatrix} +
\begin{bmatrix}b_{11} & b_{12} & \cdots & b_{1n} \\
b_{21} & b_{22} & \cdots & b_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
b_{m1} & b_{m2} & \cdots & b_{m n}\end{bmatrix} =
\begin{bmatrix}  a_{11} + b_{11} & a_{12} + b_{12} & \cdots & a_{1n} + b_{1n}\\
a_{21} + b_{12} & a_{22} + b_{22} & \cdots & a_{2n} + b_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} + b_{m1} & a_{m2} + b_{m2} & \cdots & a_{m n} + b_{m n} \end{bmatrix}.$$
Similarly, we scale them by

$$\l\; \begin{bmatrix}a_{11} & a_{12} & \cdots & a_{1n} \\
             a_{21} & a_{22} & \cdots & a_{2n} \\
             \vdots & \vdots & \ddots & \vdots \\
             a_{m1} & a_{m2} & \cdots & a_{m n}\end{bmatrix} = 
                     \begin{bmatrix}\l\,a_{11} & \l\,a_{12} & \cdots & \l\,a_{1n} \\
                          \l\,a_{21} & \l\,a_{22} & \cdots & \l\,a_{2n} \\
                          \vdots & \vdots & \ddots & \vdots \\
                          \l\,a_{m1} & \l\,a_{m2} & \cdots & \l\,a_{m n}\end{bmatrix}.$$

#### $\ex$
Going even further than  \cref{ex:poly}, we can consider vector spaces where the things we take linear combinations of (the *vectors*) are other functions. For example 
$$C[0,1]=\set{\text{$f:[0,1]\to\R$ such that $f$ is continuous}}.$$
We know that linear combinations of continuous functions are continuous, so this is a vector space.
## Linear Maps
#### $\ex$
Let's take our first example of adding vectors and apply a rotation to each one. In other words let's define a map $R:\R^2\to \R^2$ that rotates any step by (in this case) $110^\circ$. The diagram demonstrating that $(3,7)+(2,-3)=(5,4)$ rotates together to give a demonstration that 
$$R(3,7) + R(2,-3) = R(5,4) = R\parens[\big]{(3,7)+(2,-3)}.$$
In (brief) summary: the rotation of a sum is the sum of the rotations. It should be clear that the rotation of a scaling of $\v$ is simply the scaling of the rotation. 
#### $\ex$
Now let's apply a reflection through the red line in the diagram (which happens to be the line $5x+y=0$). We define $T:\R^2\to \R^2$ that reflects any step in this line. The diagram demonstrating that $(3,7)+(2,-3)=(5,4)$ reflects together to give a demonstration that 
$$T(3,7) + T(2,-3) = T(5,4) = T\parens[\big]{(3,7)+(2,-3)}.$$
The reflection of a sum is the sum of the reflections. Scaling also works.
#### $\defn$ – Linear Map
Given two vectors spaces $V$ and $W$ (over $\R$) we say that a function $T:V\to W$ is a *linear map* if for all $\v,\v'\in V$ and $\l\in \R$ we have $$\begin{align*}T(\v+\v') &= T(\v) + T(\v') \\T(\l\,\v) &= \l\, T(\v).\end{align*}$$
#### $\ex$
Consider the vector space $\R[X]$ of polynomials in a variable $X$ with real coefficients (see \Cref{ex:poly}). Consider the map $D:\R[X]\to \R[X]$ defined by $D(p)=p'$. In other words $D$ maps every polynomial to its derivative. This is a linear map. That simply means that if $\l\in \R$ and $p, q\in \R[X]$ then
$$(p+q)' = p'+q' \qquad\text{and}\qquad (\l p)' = \l p'.$$
In other words the derivative of the sum of polynomials is the sum of the individual derivatives, and the derivative of a constant multiple of a polynomial is that same multiple of the derivative. These standard facts (that apply not only to polynomials but to other differentiable functions) are precisely the condition for $D$ to be a linear map.
#### $\ex$
Consider the matrix $A\in M_{3\times 3}(\R)$ given by $$A = \begin{bmatrix}1&2&-3\\ 1&1&-2 \\ 2&7&-2\end{bmatrix}.$$
Define a function $T: \R^3 \to \R^3$ by$$\begin{equation}T((x, y, z)) = A \,  \begin{bmatrix}x\\ y\\ z\end{bmatrix} = \begin{bmatrix}1&2&-3\\ 1&1&-2 \\ 2&7&-2\end{bmatrix} \, \begin{bmatrix}x\\ y\\ z\end{bmatrix}= \begin{bmatrix}x+2y-3z\\ x+y-2z\\ 2x+7y-2z\end{bmatrix}.\end{equation}$$
Standard facts about matrix multiplication tell us that this is a linear map:
$$\begin{align*}
T((x, y, z)+(x', y', z')) &= A \parens[\Bigg]{ \begin{bmatrix}x\\ y\\ z\end{bmatrix} + \begin{bmatrix}x'\\ y'\\ z'\end{bmatrix}} = A \begin{bmatrix}x\\ y\\ z\end{bmatrix} + A \begin{bmatrix}x'\\ y'\\ z'\end{bmatrix} = 
T((x, y, z)) + T((x', y', z')) \\
T( \l (x, y, z)) &= A \parens[\Bigg]{ \l \begin{bmatrix}x\\ y\\ z\end{bmatrix}} = \l\, A \begin{bmatrix}x\\ y\\ z\end{bmatrix} = \l \, T((x, y, z)) .
\end{align*}$$
Not only that, but this linear  map can be viewed as being constructed using linear combinations. We have
$$T((x, y, z)) = \begin{bmatrix}1&2&-3\\ 1&1&-2 \\ 2&7&-2\end{bmatrix} \, \begin{bmatrix}x\\ y\\ z\end{bmatrix}= \begin{bmatrix}x+2y-3z\\ x+y-2z\\ 2x+7y-2z\end{bmatrix} 
= x\begin{bmatrix}1\\1\\2\end{bmatrix} + y\begin{bmatrix}2\\1\\7\end{bmatrix} + z\begin{bmatrix}-3\\-2\\-2\end{bmatrix}.$$
The result of computing $T((x, y, z))$ is the linear combination, using coefficients $x, y$, and $z$, of the *columns* of $A$.
## Tying Things Together
#### Perspective – Intersection of Three Planes
In \cref{sec:geometry} we alluded to the fact that the solutions to a linear equation in $\R^3$ form a plane. In \Cref{lem:plane} we'll see why this is so. Once we know that each equation defines a plane in $\R^3$, we see the set of solutions to the system is the set of all points lying on all three planes, that is, the intersection of the three planes.  We anticipate that unless there is something special about these planes (such as two of them being parallel) the three planes should have exactly one common point.
#### $\prop$
The set of solutions to the equation $ax+by+cz=d$, where $a,b,c$ are not all zero, form a plane in 3-space.

##### *Proof.*
Note that the equation $ax+by+cz=d$ can be written using dot product as 
$$(a,b,c)\cdot (x,y,z)=d.$$
Let's consider a particular solution $(x_0,y_0,z_0)$ to the above equation. For example, if $a\neq 0$ I could pick $(x_0,y_0,z_0)=(d/a,0,0)$ and similarly if $b\neq0$ and $c\neq 0$. Then we have
$$(a,b,c)\cdot (x_0,y_0,z_0)=d$$
and subtracting this from the above equation gives
$$(a,b,c)\cdot (x-x_0,y-y_0,z-z_0)=0.$$
This means $(x-x_0,y-y_0,z-z_0)$ is perpendicular to $(a,b,c)$ (or 0). Thinking of $(x-x_0,y-y_0,z-z_0)$ as a step with head at $(x,y,z)$ and tail at $(x_0,y_0,z_0)$ we see it is perpendicular to $(a,b,c)$. There is a unique plane that passes through the point $(x_0,y_0,z_0)$ and is perpendicular to $(a,b,c)$ and we have just seen that $(x,y,z)$ is a solution if and only if it lies in this plane.
#### Perspective – Linear Combinations of Vectors
We can rewrite the system as $$x\begin{bmatrix}1\\1\\2\end{bmatrix} + y\begin{bmatrix}2\\1\\7\end{bmatrix} + z\begin{bmatrix}-3\\-2\\-2\end{bmatrix} = \begin{bmatrix}-7\\-5\\8\end{bmatrix}.$$Thus the system is asking which coefficients $x, y, z$ we can use in a linear combination of three vectors on the left hand side  to obtain the vector on the right hand side.

This in turn, as we saw in \cref{ex:T}, can be rephrase in the language of linear transformations. Using the function $T$ defined  in \cref{eqn:T} we can write the system as  $$T((x, y, z)) = \begin{bmatrix}-7\\-5\\8\end{bmatrix},$$This can be rephrased as understanding whether the vector on the right hand side is a value of $T$ (we will soon phrase this as whether the vector on the right hand side is in the range of $T$) and if so, which inputs give this value. In other words we are looking for the {\em preimage} of the vector on the right hand side with respect to $T$. 
# Beginnings
## Fields
#### $\defn$ – Field
![[Field]]
#### $\defn$ – Compatibility
![[Compatible with Addition & Multiplication]]
#### $\rem$
The fact that the operations of addition and multiplication are functions $+,\times:\F\times \F \to \F$ implicitly gives the following additional properties:
- Closure under addition: for all $x, y\in \F$ we have $x+y\in \F$.
- Closure under addition: for all $x, y\in \F$ we have $x\times y\in \F$.
#### $\ex$ – The Complex Numbers
The *complex* numbers are the numbers of the form $$\C=\{a+bi \mid a,b\in \R\}$$with addition and multiplication defined by
$$\begin{eqnarray*}
(a+bi)+(c+di)&=(a+b)+(c+d)i\\
(a+bi)\times(c+di)&=(ac-bd)+(ad+bc)i
\end{eqnarray*}$$
Note that by our definition of multiplication
$$i^2=i\times i=(0+1i)\times(0+1i)=-1+0i=-1.$$
#### $\ex$ – The Rational Numbers
The rational numbers $\Q$ are a field, indeed they are a subfield of $\R$ (simply meaning that $\Q\sse \R$ and the field operations for $\Q$ are the same whether you think of elements of $\Q$ as rational numbers or real numbers). This fact means that conditions A1-A2, M1-M2, and C1 are trivially satisfied, since they're true for real numbers, not just rationals. Since the special real numbers $0,1$ are in fact in $\Q$ we also get A3, M3, and C2 for free. This only leaves A4 and M4; given $x\in \Q$ we know that there are real numbers $-x$ and $x\inv$ such that $x+(-x)=0$ and $xx\inv=1$, but what we need to know is that there are rational numbers with these properties\footnote{Of course if $x=0$ we don't need to find a multiplicative inverse for $x$.}. Fortunately it is that case that if $x$ is rational then so are $-x$ and $x\inv$. Thus $\Q$ is a field. 
#### $\ex$ – Field with Two Elements
The field with two elements, $\F_2$, has as its only elements the two residue classes modulo $2$, with addition and multiplication defined modulo $2$. To be specific, we have the following addition and multiplication tables.$$\begin{array}{c|cc}
            + & 0 & 1 \\
            \hline
            0 & 0 & 1 \\
            1 & 1 & 0 \\         
        \end{array} \qquad
        \begin{array}{c|cc}
            \times & 0 & 1 \\
            \hline
            0 & 0 & 0 \\
            1 & 0 & 1 \\
\end{array}$$There are in fact many interesting examples of vector spaces where we use $\F_2$ for our numbers. For instance many schemes of data transmission use the ideas of linear algebra to build error correction into digital communication. 
#### $\ex$
More generally, if $p$ is a prime then the collection $\Z_p$ of remainders upon division by $p$ is a field with addition and multiplication being the usual modular arithmetic operations. I will usually denote the elements of $\Z_p$ simply by $\set{0,1,2,\dots,p-1}$. 
The operations are given by $$\begin{eqnarray*}
a+b &= \text{remainder of } (a+b) \text{ upon division  by } p\\
a\times b &= \text{remainder of } (a\times b) \text{ upon division  by } p
\end{eqnarray*}$$Essentially every one of the properties of a field are standard facts about modular arithmetic, and indeed are true in $\Z_m$ for non-prime $m$. The exception is M4, which requires the modulus to be prime. If $x\in \Z_p$ and $x\not=0$ then in particular $\gcd(x, p)=1$ when thought of as integers, so by Bezout's identity (a consequence of Euclid's algorithm for finding greatest common divisors) there exist integers $a, b\in \Z$ such that $$ax + bp = 1$$Thus in $\Z_p$ we have $ax=1$, and we can take $x\inv=a$. 
#### Notation
We make some standard abbreviations when computing in fields. We write
$$\begin{align*}
x-y &:= x+(-y) \\
x/y &:= x y\inv \\
x^0 &:= 1 \\
x^n &:= \underbrace{x \times x \times \dots \times x}_{\text{$n$ factors}}\quad \text{for integers $n\ge 1$} \\
x^{-m} &:= \underbrace{x\inv \times x\inv \times \dots \times x\inv}_{\text{$m$ factors}} \quad \text{for integers $m\ge 1$} \\
\end{align*}$$
We also define, for $n\in \N$, $$n := \underbrace{1+1+\dots+1}_{\text{$n$ summands}} \in \F.$$
#### $\rem$
Above we have defined elements $1,2,3,\dots$ in any field $\F$. In $\Z_7$ we have $10=3=-4$, and in $\Z_{29}$ we have $59=30=1$.

You might think it would be confusing that $287$ is simultaneously the name of an integer and a field element, particularly in fields $\F_{7}$ or $\F_{41}$ where $287=0$, but context resolves all such confusions, usually without anyone noticing.
#### $\lem$ – Arithmetic in Fields
If $\F$ is a field an $x, y\in \F\setminus\set{0}$ then for For all $n, m\in \Z$ we have
$$\begin{align*}
(x y)^n &= x^n y^n & (x/y)^n &= x^n y^{-n} \\
x^n x^m &= x^{n+m} & \left(x^n\right)^m &= x^{nm}.\\
\end{align*}$$
## Vector Spaces
#### $\defn$ – Vector Space
![[Vector Space]]
#### Notation
We make a standard abbreviation in the context of a vector space as follows:$$\v-\w := \v+(-\w)$$for $\v,\w\in V$.
#### $\lem$ – Grand Reassuring Lemma
If $V$ is a vector space over the field $\F$ then the definitions we have made work well with our intuitions in the following ways.
(a) All identities are unique. There is a unique element $0\in \F$ satisfying A3. There is a unique $1\in \F$ satisfying M3. There is a unique element $\0\in V$ satisfying VA3.
(b) All inverses are unique. For $x\in \F$, $y\in\F\setminus\set{0}$, and $\v\in V$ there are unique elements $-x, y\inv \in \F$ and $-\v\in V$ such that $$x+(-x) = 0 \qquad y y\inv = 1 \qquad \v+(-\v) = \0.$$
(c) Inverting twice gets you back where you started: for all $x\in \F$, $y\in \F\setminus\set{0}$, and $\v\in V$ we have $$-(-x) = x \qquad (y\inv)\inv = y \qquad -(-\v) = \v.$$
(d) For all $x\in \F$ and $\v\in V$ we have $(-x)\v = -(x\v)$. In particular $(-1)\v=-\v$.
(e) For $x, y\in\F$ and $\v\in V$ we have 
	(1) $x y=0$ if and only if at least one of $x, y$ is $0$
	(2) $x\v=\0$ if and only if $x=0$ or $\v=\0$.

##### *Proof.*
#### $\ex$
(a) The classic vector spaces (over $\R$) are $\R^2$ and $\R^3$. With identical checks we see that also $\R^n$, $n\ge 1$ and $\R^\N$ are vector spaces.
(b) Also vital are subspaces of $\R^n$, such as the plane $\setof{(x, y, z)}{x+y+z=0}\sse \R^3$ and the line $\setof{t(1,0,-1)}{t\in \R}\sse \R^3$.  
(c) Note that both the line and the plane given here pass through the origin $(0,0,0)$. A line or plane that does not pass through the origin is not a subspace. Why not?
(d) Similarly $\Q, \Q^2, \Q^3,\dots$, and $\Q^\N$ are vector spaces over $\Q$ and $\F^n$ (for any field $\F$ and any $n\ge 0$) is a vector space over $\F$.
(e) $\R$ is a vector space over $\Q$
(f) $\C$ is a vector space over $\R$
(g) The set of polynomial $\R[X]$ is a vector space over $\R$ and in fact an $\R$-algebra.\footnote{An algebra is a vector space for which we can also multiply two vectors (i addition to multiplying vectors with scalars.} 
(h) The set $M_{m\times n}(\F)$ of $m\times n$ matrices whose entries come from $\F$ is a vector space of $\F$, with the usual notions of adding matrices and multiplying them by scalars. 
(i) The set $C(\R)=\setof{f:[0,1]\to\R}{\text{f is continuous}}$ is a vector space over $\R$. It is a subspace of $\R^{[0,1]}$.
#### $\defn$ – Subspace
If $V$ is a vector space over $\F$ and $W\sse V$ then we say that $W$ is a *(linear) subspace* of $V$ if $W$ is non-empty and $W$ is closed under taking linear combinations. That is to say, for all $\vs \in W$, $\ls \in \F$ we have $\sum_{i=1}^n \l_i\v_i \in W$. It is easy to show (by induction) that it suffices to check that $\0\in W$ and for all $\v,\w\in W$, $\l,\mu\in \F$ we have $\l\v+\mu\w\in W$. 
#### $\lem$ – Subspaces are Vector Spaces
If $V$ is a vector space over $\F$ and $W\sse V$ is a subspace of $V$ then $W$ is a vector space in its own right (with the operations that come with $V$; we add and scale vectors in $W$ just as we do in $V$.)

##### *Proof.*
Most of the vector space axioms are satisfied automatically: VA1, VA2, and SM1--4 work in $W$ because they work for every vector in $V$ and every scalar in $\F$. One key point is that because $W$ is closed under taking linear combinations there really \emph{is} a vector addition map $+\colon W\times W \to W$ and a scalar multiplication map $\F\times W\to W$. The result of adding two vectors in $W$ is again a vector in $W$, similarly for scaling. 

That leaves only VA3 and VA4. We need to show that $\0\in W$ and that if $\w\in W$ then also $-\w\in W$. Both of these work by choosing appropriate scalings. Since $W\neq \emptyset$ there exists some $\w\in W$, so then $\0 = 0\w \in W$ (because $W$ is closed under linear combinations). Similarly, if $\w\in W$ then $-\w=(-1)\w\in W$.
#### $\defn$ – Span
If $V$ is a [[Vector Space|vector space]] over $\F$ and $S\sse V$ then the *span* of $S$, denoted $\Span(S)$, is the set $$\Span(S) = \setof[\Big]{\sum_{i=0}^n \l_i\v_i}{\vs\in S, \ls\in \F, n\ge 0}.$$I.e., it is the collection of all [[Linear Combination|linear combinations]] of vectors in $S$.
#### $\ex$
$\R[X]= \Span\left(\{1, X, X^2, X^3, \ldots, X^i, \ldots \mid i\geq 0\}\right).$
The set of polynomials of degree at most $d$ is 
$\R[X]_{\leq d}= \Span\left(\{1, X, X^2, X^3, \ldots, X^d\}\right).$
#### $\lem$ – Span is a Subspace
If $V$ is a vector space over $\F$ and $S\sse V$ then $\Span(S)$ is a subspace of $V$.

##### *Proof.*
Clearly $\0\in \Span(S)$; simply take $n=0$ in the definition. Now if $\v,\v'\in \Span(S)$ and $\l,\mu\in \F$ we have, for some $n, n'\ge 0$ and $\vs$, $\vps\in S$, $\ls$, $\lps\in \F$,$$\v = \sum_{i=1}^n \l_i \v_i \qquad \text{and} \qquad \v' = \sum_{i=1}^{n'} \l'_i \v'_i.$$Thus we have $$\l\v+\mu\v' = \l\sum_{i=1}^n \l_i \v_i + \mu \sum_{i=1}^{n'} \l'_i \v'_i \in \Span(S).$$
#### $\ex$
If we think of the monomials $1, X, X^2, X^3, \ldots$ as functions $X^i:\R\to \R$ then, in view of \Cref{lem:linspanissubspace},
\Cref{ex:R[X]span} identifies $\R[X]$ with a subspace of $\C(\R)$ . Moreover \Cref{ex:R[X]span} implies that the polynomials of degree at most $d$ form a subspace of $\R[X]$.
#### $\rem$
By contrast, the set of polynomials of degree exactly $d$ do not form a subspace of $\R[X]$. Why not?
## Linear Maps
#### $\defn$ – Linear Map
If $V,W$ are vector spaces over $\F$ then we say that a function $T:V\to W$ is *linear* if it preserves linear combinations. That is to say, for all $\u,\v\in V$ and $\l,\mu\in \F$ we have $$T(\l\u+\mu\v) = \l T(\u) + \mu T(\v).$$We let $L(V,W)$ denote the set of all linear maps from $V$ to $W$, so $$L(V,W) = \setof{T:V\to W}{T\text{ is linear}}.$$
#### Exercise
Prove that Definition \ref{deflinmap} is equivalent to requiring that  for all $\u,\v\in V$ and $\l \in \F$ we have $T(\u+\v) = T(\u) + T(\v)$ and $T(\l\v)=\l T(\v)$.
#### $\ex$
(a) $T:\R^3\to \R$ given by $T((x, y, z)) = 3x+2y+z$.
(b) If $A\in M_{m\times n}(\F)$ then we can define a linear map $M_A:\F^n\to \F^m$ by doing matrix multiplication. To be completely explicit we define, for $\v=(v_1,v_2,\dots,v_n)\in \F^n$, $$M_A(\v) = A\v = \left({\sum_{j=1}^n A_{i j} v_j }\right)_{i=1}^m.$$It is a fact, that we will prove soon, that every linear map from $\F^n$ to $\F^m$ is of the form $M_A$ for some matrix $A\in M_{m\times n}(\F)$.
(c) Define $I:C[0,1]\to \R$ by $\displaystyle I(f) = \int_{0}^1 f(x) \, dx$. Then $I$ is linear by standard facts about integration.
#### $\defn$ – Set of Linear Maps
If $V$ and $W$ are vector spaces over a field $\F$,	we let $L(V,W)$ denote the set of all linear maps from $V$ to $W$, so
$$L(V,W) = \setof{T:V\to W}{\text{$T$ is linear}}.$$
We have different notation for the special case of $L(V,W)$ where $W=\F$ (which is of course a vector space over $\F$). We write $V^{*}:= L(V,\F)$. These linear maps are especially important because they correspond to the left hand sides of linear equations.
#### $\lem$ – 
If $V,W$ are vector spaces over $\F$ then $L(V,W)$ is also a vector space over $\F$ when we define, for $T,T'\in L(V,W)$ and $\l\in \F$, $$T+T' : \v \mapsto T(\v)+T'(\v) \qquad \l T: \v \mapsto \l T(\v).$$
##### *Proof.*
The proof is straightforward definition checking. As a representative sample I'll prove that vector addition is associative. For $R,S,T \in L(V,W)$ and $\v\in V$ we have 
$$\begin{align*}
(R+(S+T)(\v) &= R(\v) + (S+T))(\v) \\
&= R(\v) + (S(\v)+T(\v)) \\
&= (R(\v)+S(\v))+T(\v) \\
&= (R+S)(\v)+T(\v) \\
&= ((R+S)+T)(\v),
\end{align*}$$
where the central equality is associativity of vector addition in $W$ and everything else is the definition of addition in $L(V,W)$. The zero vector in $L(V,W)$ is the linear map $0:V\to W$ that sends every vector in $V$ to $\0_W$, the zero vector in $W$.
#### Notation
We have different notation for the special case of $L(V,W)$ where $W=\F$ (which is of course a vector space over $\F$). We write $V^*:= L(V,\F)$. These linear maps are especially important because they correspond to the left hand sides of linear equations.
#### $\defn$ – Range and Nullspace
If $T:V\to W$ is a linear map we define the following subspaces associated to it.$$\begin{align*}\\
T(V) = \range(T) &:= \setof{T(\v)}{\v\in V} \\
\ker(T) = \nullspace(T) &:= \setof{\v \in V}{T(\v)=\0}.
\end{align*}$$
#### $\ex$
(a) for $T:\R^3\to \R$ given by $T((x, y, z)) = ax+by+cz$ where not all of $a,b,c$ are zero \Cref{lem:plane} yields that $\ker(T)$ is a plane passing through the origin (note that $(0.0,0)$ is a particular solution to $ax+by+cz=0$.
(b) If $A\in M_{m\times n}(\F)$ the kernel of the linear map $M_A:\F^n\to \F^m, M_A(\v) = A\v$ is the set of solutions $\x$ to the {\em homogeneous} system of equations $A\x=\0$.
(c) If $D:\R[X]\to \R[X]$ is given by $D(p)=\frac{d}{dX}(p)$ then $\ker(D)=R[X]_0=\{r\mid r\in \R\}$, the set of constant polynomials 
#### $\ex$ 
If $T:C[0,1]\to \R$ is given by $T(f)=\int_{0}^1 f(x)dx$ then the range of $T$ is $\range(T) =\R$. To see this take any $r\in\R$ and consider the constant function $f_r:[0,1]\to\R, f_r(x)=r$. Then $f_r\in C[0,1]$ and $T(f_r)=\int_{0}^1 f_r(x) dx=\int_{0}^1 r dx= r$. In conclusion, every $r\in \R$ is in $\range(T)$.
#### $\lem$ – Range and Nullspace are Subspaces
If $T\in L(V,W)$ then $T(V)$ is a subspace of $W$ and $\ker(T)$ is a subspace of $V$.

##### *Proof.*
Consider first vectors $T(\u),T(\v)\in T(V)$. For $\l,\mu\in \F$ we have$$\l T(\u) + \mu T(\v) = T(\l \u+\mu \v) \in T(V),$$so $T(V)$ is closed under taking linear combinations. For $\ker(T)$ we have a criterion for testing membership rather than a way of generating vectors, so the proof looks a little different. Take $\u,\v\in \ker(T)$ and $\l,\mu\in \F$. We would like to prove that $\l\u+\mu\v\in \ker(T)$, and to verify this we simply apply $T$:$$T(\l\u+\mu\v) = \l T(\u) + \mu T(\v) = \l \0 + \mu \0 = \0+\0 = \0.$$Thus $\ker(T)$ is closed under taking linear combinations and we are done.
#### $\ex$
The set $\setof[\big]{f\in C[0,1]}{\int_0^1 f(x) \, dx=0}$ is a subspace of $C[0,1]$ 
#### $\defn$ –Surjective
![[Surjective]]
#### $\prop$
A linear map $T:V\to W$ is surjective if and only if $\range(T)=W$. 

##### *Proof.*
According to Definition \ref{def:kerrange}, $\range(T)=\{T(\v)\mid v\in V\}$. Thus $\range(T)=W$ if and only if for every $\w\in W$ there exists $\v\in V$ so that $\w=T(\v)$ if and only if $T$ is surjective.
#### $\defn$ – Injective
![[Injective]]
#### $\thm$ 
A linear map $T:V\to W$ is injective if and only if $\ker(T)=\{\0_V\}$.
# Vector Spaces and Linear Maps
## Linear Independence, Spanning, and Bases
#### $\defn$
If $V$ is a [[Vector Space|vector space]] over $\F$ and $S\sse V$ then $S$ is *linearly independent* if every [[Linear Combination|linear combination]]of (distinct) vectors from $S$ equaling $\0$ has all its coefficients equal to $0$. In other words for all $\vs\in S$, $\ls\in \F$ with $\v_i\not=\v_j$ for $i\not= j$ we have
$$\Slv{\l}{i}{n} = \0 \quad\implies\quad \l_1=\l_2=\dots=\l_n=0.$$
#### $\ex$
(a) The set $\set{(1,0),(0,1)} \sse\R^2$ is linearly independent since $$\l(1,0) + \mu(0,1) = (0,0) \implies (\l,\mu)=(0,0) \implies \l=0,\mu=0.$$Similarly $\set{\e_1,\e_2,\e_3}\sse \R^3$ is linearly independent.
(b) In $\R^3$ the vectors $(1,0, 0), (2,1,0)$ and $(3,2,1)$ are linearly independent. Indeed, $$\l_1(1,0,0)+\l_2(2,1,0)+\l_3(3,2,1)=\0$$if and only if $$\begin{align*}
\l_1+2\l_2+\l_{3}&=0\\
\l_2+2\l_3&= 0\\
\l_{3}&= 0
\end{align*}$$which yields $\l_1=\l_2=\l_3=0$.
(c) $\set{\sin,\cos}\sse \R^\R$ is linearly independent since if $\l \sin + \mu \cos = 0$ (the right hand side here is the 0 function) then in particular $(\l \sin + \mu \cos)(0) = \mu = 0$ and $(\l \sin + \mu \cos)(\pi/2) = \l = 0$.
(d) $\set{1,\sqrt 2} \sse \R$ is linearly independent when we think of $\R$ as a vector space over $\Q$. Suppose $\l,\mu\in \Q$ satisfy $\l 1 + \mu \sqrt 2=0$. If $\mu=0$ we have $\l 1 = \l=0$. On the other hand if $\mu\not=0$ then $\sqrt2 = -\l/\mu \in \Q$ which we know is impossible.
(e) The set $S=\setof{\cos(x)^n}{n\in \N} \sse \R^\R$ is linearly independent. A linear combination from $S$ equaling the $0$ function would be a finite sequence $\l_0,\ls\in \R$ such that 
		$$
			\l_0 + \l_1\cos(x) + \dots + \l_n \cos^n(x) = 0
		$$
for all $x\in \R$. In other words the polynomial $p = \sum_{i=0}^n \l_iX^i \in \R[X]$ would satisfy  $p(\cos(x))=0$ for all $x\in \R$. Thus every value of $\cos(x)$ would have to be a root of $p$. We know that $\cos$ takes infinitely many values and the only polynomial with infinitely many roots is the $0$ polynomial, so our original linear combination must have been trivial.
#### $\lem$ – Linear Independence Lemma
Let $V$ be a vector space over $\F$. 
(a) If $S\sse T\sse V$ and $T$ is linearly independent then $S$ is linearly independent.
(b) If $S\sse V$ is linearly independent then for all $\v\in \Span(S)$ there is a unique way of writing $\v$ as a linear combination from $S$ in the following sense: for all $\v\in \Span(S)$ there is a unique finite subset $\set{\vs} \sse S$ and unique corresponding coefficients $\ls\in \F$ such that $\Slv = \v$.

##### *Proof.*
The first part is immediate since any linear combination from $S$ is also a linear combination from $T$, so any linear combination from $S$ equaling $\0$ is also a linear combination from $T$ equaling $\0$, so is, by hypothesis, trivial. For the second part suppose that some vector $\v\in \Span(S)$ can be represented in two ways:
$$\Slv = \v = \Smuv.$$
(We've thrown all the vectors used in either representation into the set $\set{\vs}$.) Subtracting the right hand side from the left we have
$$\sum_{i=1}^n (\l_i-\mu_i) \v_i = \0,$$
and thus, since $S$ is linearly independent, $\l_i=\mu_i$ for all $i$.
#### $\defn$
A subset $S$ of a vector space $V$ is called *spanning* (or a *spanning set*) if $\Span(S)=V$. 
#### $\ex$
- The set  $\set{\e_1=(1,0,0),\e_2=(0,1,0),\e_3=(0,0,1)}\sse \R^3$ is a spanning set for $\R^3$.
- The set $S=\{X^i \mid i\in \Z, i\geq 0\}$ is a spanning set for $\R[X]$.	
#### $\lem$ – Spanning Lemma
(a) If $S\sse T$ then $\Span(S)\sse \Span(T)$. In particular if $S$ is spanning then so is $T$.
(b) For subsets $S,T\sse V$ the conditions $T\sse \Span(S)$ and $\Span(S\cup T) = \Span(S)$ are equivalent.

##### *Proof.*
The first is very straightforward. It boils down to observing that if $S\sse T$ then linear combinations from $S$ are in fact linear combinations from $T$. The second is slightly more subtle. First note that one inclusion, $\Span(S)\sse \Span(S\cup T)$, always holds, so really we have to show that $T\sse \Span(S)$ is equivalent to $\Span(S\cup T)\sse \Span(S)$. Suppose then that $T\sse \Span(S)$ and $\v\in \Span(S\cup T)$. We have, for some $\vs \in S$, $\ws[m] \in T$ and $\ls, \mus[m] \in \F$, that $$\v = \Slv + \sum_{j=1}^m \mu_j \w_j.$$Since each $\w_j$ is, by hypothesis, a linear combination of vectors in $S$ it is clear that we can expand this sum into a linear combination of vectors from $S$, hence $\v\in \Span(S)$. Conversely, if $\Span(S\cup T) \sse \Span(S)$ then we have $$T \sse \Span(S\cup T) \sse \Span(S).$$
#### $\defn$
A set $S$ is *maximal linearly independent* if $S$ is [[Linearly Independent|linearly independent]] and every strict superset $T\supsetneq S$ is not linearly independent.
#### $\defn$
A set $S$ is *minimal spanning* if $S$ is a spanning set and every strict subset $T\subsetneq S$ is not spanning.
#### $\lem$ – Interaction Lemma
(a) If $I$ is a maximal linearly independent set then it spans.
(b) If $S$ is a minimal spanning set then it is linearly independent.
##### *Proof.*
Let $I$ be a maximal linearly independent subset of $V$ and let $\v\in V$. If $\v\in I$ then certainly $\v\in \Span(I)$. Otherwise $T=I\cup \set{\v}$ is a strict superset of $I$ and is therefore not linearly independent. So there is some non-trivial linear combination of vectors from $I\cup \set{\v}$ that is $\0$. It cannot be that all the vectors involved in this linear combination come from $I$, else $I$ would not be linearly independent. Thus for some $\l\not=0$ and some $\vs\in I$, $\ls\in \F$ we have $$\l\v + \Slv = \0 $$and hence$$\v = -\frac1\l \Slv \in \Span(I).$$For the second part suppose that $S$ is a  minimal spanning set and $\Slv = \0$ is a non-trivial linear combination from $S$ with, without loss of generality, $\l_1\not=0$. Then $$\v_1 = -\frac1{\l_1} \sum_{i=2}^n \v_i \in \Span(S\setminus\set{\v_1})$$and hence (by part \ref{part:SUT}) of the spanning lemma)$$ \Span(S\setminus\set{\v_1}) = \Span(S) = V.$$This contradicts the minimality of $S$, so no such linear combination can exist.
#### $\defn$
A *basis* is a linearly independent spanning set.
#### $\thm$ – Steinitz Exchange Lemma
If $V$ is a vector space, $S\sse V$ is a spanning set, and $I\sse V$ is a finite linearly independent set then there exists a spanning set $T$ with $I \sse T \sse I\cup S$ and $\abs{T}\le \abs{S}$.

##### *Proof.*
We prove the result by induction on $\abs{I}$. If $\abs{I}=0$ then $I=\emptyset$ and we can take $T=S$. Otherwise $\abs{I}>0$. Pick $\v\in I$ and set $I' = I\setminus\set{\v}$. By induction there exists a spanning set $T'$ with $I' \sse T' \sse I'\cup S$ with $\abs{T'}\le \abs{S}$. If $\v\in T'$ then there is nothing further to do; we can take $T=T'$. Otherwise, our plan now is to insert $\v$ into $T'$ and kick out one element of $T'$, \emph{but not an element of $I$}, so that the result is still spanning. Since $T'$ is spanning we have some $\vs\in T'$, $\ls\in \F$ such that $$\v = \Slv.$$I claim that for some $\v_i\in T'\setminus I'$ we have $\l_i\not =0$, for otherwise $\v-\Slv=\0$ would be a non-trivial linear combination of vectors from $I$ equalling $\0$, a contradiction to the linearly independence of $I$. Now note that $$\v_i = \frac1{\l_i}\parens[\Big]{\v - \sum_{j\not=i} \l_j\v_j} \in \Span(T' \cup \set{\v} \setminus \set{\v_i}),$$so  $$\Span(T'  \cup \set{\v} \setminus \set{\v_i}) = \Span(T'\cup\set{\v}) = V.$$Thus we can take $T= T'  \cup \set{\v} \setminus \set{\v_i}$. It is spanning, and it is easy to check that it satisfies the other conditions.
#### $\defn$
If $V$ is a vector space with a finite spanning set then we say $V$ is *finite dimensional*.
#### $\thm$
Let $V$ be a finite dimensional vector space. 
(a) All bases of $V$ have the same size.
(b) Any spanning set $S$ of $V$ contains a basis.
(c) Any linearly independent set $I\sse V$ is contained in a basis.

##### *Proof.*
For a) suppose that $B_1$ and $B_2$ are bases of $V$. By symmetry it suffices to prove that $\abs{B_1}\le \abs{B_2}$. Since $B_1$ is (in particular) linearly independent, and $B_2$ is spanning, the Steinitz exchange lemma tells us that there exists a spanning set $T$ with $B_1\sse T$ and $\abs{T}\le \abs{B_2}$. We thus have $\abs{B_1}\le \abs{T} \le \abs{B_2}$.

For b), let $S\sse V$ be spanning. By induction on $\abs{S}$ it is easy to prove that $S$ contains a minimal spanning set. (If $\abs{S}=0$ then $S$ itself is clearly minimal; if $\abs{S}>0$ then either $S$ is minimal or it contains a strict subset $S'\subsetneqq S$ that is spanning. By induction $S'$ contains a minimal spanning set, which is a minimal spanning set contained in $S$.) Minimal spanning sets are bases by the Interaction Lemma.

Finally, let $I\sse V$ be linearly independent and let $S$ be a finite spanning set for $V$. (Such an $S$ exists by the definition of finite dimensionality.) By part b) there is a basis $B$ contained in $S$. By the Steinitz exchange property there is a spanning set $T$ with $I\sse T$ and $\abs{T}\le \abs{B}$. By b) we know that $T$ contains a basis, but unless that basis is exactly $T$ then we would have found a basis for $V$ strictly smaller than $B$, contradicting a). Thus $T$ is a basis containing $I$.
#### $\thm$
If $B$ is a basis for the vector space $V$ over $\F$ and $W$ is another vector space over $\F$ then linear maps in $L(V,W)$ are determined uniquely by their values on $B$. To be precise given an arbitrary function\footnote{We don't assume that $f$ is linear since we don't even have a definition of linearity for such maps. $B$ is not a vector space.} $f:B\to W$ there exists a unique linear map $T:V\to W$ such that $T(\b)=f(\b)$ for all $\b\in B$. 

##### *Proof.*
The uniqueness is clear since if $\v\in V$ is written as a linear combination from $B$, so $\v =\sum_1^n\l_i \b_i$, then we must have that$$\begin{equation}T(\v) = \sum_1^n \l_i T(\b_i) = \sum_1^n \l_i f(\b_i).\end{equation}$$Thus to prove existence we simply need to show that (\ref{eq:Tdef}) defines a linear map. Consider $\v,\w\in V$ and $\l,\mu\in \F$. We'll need to express $\v,\w$ as linear combinations from $B$; let $\set{\vecs{\b}{n}}$ be collection of all vectors from $B$ that appear in either representation. Suppose $$\v = \sum_1^n \l_i \b_i \qquad \w = \sum_1^n \mu_i \b_i.$$(Notice that some of the $\l_i,\mu_i$ might be $0$.) Now we have$$\l\v + \mu\w = \sum_1^n (\l\l_i+\mu\mu_i) \b_i,$$and this is the unique representation of $\l\v+\mu \w$ using the basis $B$, except that some of the $\l\l_i+\mu\mu_i$ might be $0$. Thus $$T(\l\v+\mu \w) = \sum_1^n (\l\l_i+\mu\mu_i) f(\b_i) = \l\sum_1^n \l_i f(\b_i) + \mu\sum_1^n \mu_i f(\b_i) = \l T(\v)+\mu T(\w).$$