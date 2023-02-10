#### Problem 1
Recall that we use the same notation for steps and points because if you start at the origin and take the step $(x, y)$ you get to the point $(x, y)$. Adding points, and multiplying points scalars are operations that make sense in the same way that they make sense for steps. On the other hand points are much easier to draw. 

(a) If $\v$ and $\w$ are points, how do you describe the midpoint of $\v$ and $\w$ algebraically? Provide justification.
(b) How do you describe the interval between $\v$ and $\w$ algebraically? Provide justification.
(c) How do you describe the line through $\v$ and $\w$ algebraically? Provide justification.

##### Solution:
Note that we can reduce this case to when the line is in $\R^2$ for each part. 

###### Part (a)
Say $\v=(x_1,y_1)$ and $\w=(x_2,y_2)$. The midpoint between them would be the point $\u=(\frac{x_{1}+x_{2}}{2},\frac{y_{1}+y_{2}}{2})$. This is because we can take the step from $\v$ to $\w$ (conveniently equal to $2\u$) and divide it in half to find the midpoint.
***
###### Part (b)

Let $m=\frac{y_{2}-y_{1}}{x_{2}-x_{1}}$, and $S$ the set of points $\u=(x,y)$ such that $\frac{y_{2}-y}{x_{2}-x}=m$. Thus the step from $\w$ to $\u$ is a scalar multiple of the step from $\w$ to $\v$.

Additionally, a point $\u$ is on the line through $\v$ and $\w$ if $(\u-\v)\cdot(\w-\v)=|\u-\v|\times|\w-\v|$ and when the $x$-coordinate is between the $x$-coordinates of the endpoints.. In words, when $\cos(\t)=1$ in the definition of the dot product (placing $\u$ on the line connecting $\v$ and $\w$, see Part (c)), and $\u$ lies between $\v$ and $\w$ on the line.
***
###### Part (c)
Let $m=\frac{y_{2}-y_{1}}{x_{2}-x_{1}}$, and $S$ the set of points $\u=(x,y)$ such that $\frac{y_{2}-y}{x_{2}-x}=m$. Thus the step from $\w$ to $\u$ is a scalar multiple of the step from $\w$ to $\v$. In other words, $\u-\v=\l(\w-\v)$ for some $\l\in\R$.

Alternatively, a point $\u$ is on the line through $\v$ and $\w$ if $$(\u-\v)\cdot(\w-\v)=|\u-\v|\times|\w-\v|.$$In words, when $\cos(\t)=1$ in the definition of the dot product.
***
#### Problem 2
A *median* of a triangle is a line segment joining one vertex to the midpoint of the opposite side. Use the ideas of steps to prove that all three medians of a triangle meet at a common point.

##### *Proof:*
(I have heard rumors that there is a much faster way to do this, so apologies in advance)

First, note that as the three vertices of a triangle form a plane, it suffices to show that the result holds in $\R^2$.

Let $ABC$ be a triangle with $A=(x_{A},y_{A}), B=(x_{B},y_{B}),$ and $C=(x_{C},y_{C})$
From Part (a) of Problem 1, we see the midpoints of each side of the triangle are the following:
- $(x_{AB},y_{AB}),$ where $x_{AB}=(\frac{x_{A}+x_{B}}{2})$ and $y_{AB}=(\frac{y_{A}+y_{B}}{2})$;
- $(x_{AC},y_{AC}),$ where $x_{AC}=(\frac{x_{A}+x_{C}}{2})$ and $y_{AC}=(\frac{y_{A}+y_{C}}{2})$; and
- $(x_{BC},y_{BC}),$ where $x_{BC}=(\frac{x_{B}+x_{C}}{2})$ and $y_{BC}=(\frac{y_{B}+y_{C}}{2})$.
Set $m_{1}=\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}$, $m_{2}=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}$, and $m_{3}=\frac{y_{BC}-y_{A}}{x_{BC}-x_{A}}$. From Part (c) of Problem 1, we seek a point $D=(x,y)$ such that the following hold:
- $\frac{y_{AB}-y}{x_{AB}-x}=\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}$,
- $\frac{y_{AC}-y}{x_{AC}-x}=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}$, and
- $\frac{y_{BC}-y}{x_{BC}-x}=\frac{y_{BC}-y_{A}}{x_{BC}-x_{A}}$.
Looking just at the first line, we see we can solve for $y$ in terms of of $x$ and everything else, yielding $$y=-\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)+y_{AB}.$$
We can substitute this into the second equation to find
$$\begin{align}

\frac{y_{AC}+\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)-y_{AB}}{x_{AC}-x}&=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\\

y_{AC}+\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)-y_{AB}&=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}(x_{AC}-x)\\

(\frac{y_{A}+y_{C}}{2})+\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)-(\frac{y_{A}+y_{B}}{2})&=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}(x_{AC}-x)\\

-y_{BC}+\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)&=\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}(x_{AC}-x)\\

\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)(x_{AB}-x)-\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}(x_{AC}-x)&=y_{BC}\\

%%x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)+x\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)&=y_{BC}\\%%

x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)-y_{BC}&=x\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)\\

x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)-y_{BC}&=x\left(\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)\right)\\

\frac{x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)-y_{BC}}{\left(\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)\right)}&=x\\

\end{align}$$
(I removed a step so that if would fit on the page, I can provide that if needed). Now that we have $x$, we can plug in the absurdity that is this value back into $y$ to find the point at which all three medians intersect: $D=\left(\left(-\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)\left(x_{AB}-\left(\frac{x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)-y_{BC}}{\left(\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)\right)}\right)\right)+y_{AB},\frac{x_{AB}\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-x_{AC}\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)-y_{BC}}{\left(\left(\frac{y_{AB}-y_{C}}{x_{AB}-x_{C}}\right)-\left(\frac{y_{AC}-y_{B}}{x_{AC}-x_{B}}\right)\right)}\right)\right)$
***
#### Problem 3
(a) Prove that $\forall\, \v,\w \in \R^2$ we have $\abs{\v+\w}^2 = \abs{\v}^2 + 2\,\v\cdot \w + \abs{\w}^2$.
(b) Deduce the Law of Cosines from Part (a) – it states that if $a,b,c$ are the lengths of the three sides of a triangle and $C$ is the angle opposite to the side of length $c$ then 
$$c^2=a^2+b^2-2ab\cos(C).$$
(c) Prove the Parallelogram Law: that $\forall\,\v, \w\in \R^3$ we have $$\abs{\v}^2 + \abs{\w}^2 = \frac{\abs{\v+\w}^2 + \abs{\v-\w}^2}{2}.$$
##### *Proof.*
###### Part (a)
Let $\v,\w \in \R^2$ and consider $$\begin{align}
|\v+w| ^2&=|\v+\w|\cdot|\v+\w|\\
&=|\v|\cdot|\v|+|\v|\cdot|\w|+|\v|\cdot|\w|+|\w|\cdot|\w|\\
&=|\v|^{2}+2\v\cdot\w+|\w|^{2},\\
\end{align}$$
***
###### Part (b) 
Let $abc$ be a triangle with side lengths $a,b,c$, where $C$ is the angle where $a$ and $b$ meet. Let $(x_{C},y_{C})$ denote the vertex of the triangle where sides $a$ and $b$ meet, and similarly define $(x_{A},y_{A})$ and $(x_{B},y_{B})$. Let $a'$ denote the step from $(x_{B},y_{B})$ to $(x_{C},y_{C})$, $b'$ the step from $(x_{A},y_{A})$ to $(x_{C},y_{C})$, and $c'$ the step from $(x_{A},y_{A})$ to $(x_{B},y_{B})$. Notice that $|a'|=|a|$, $|b'|=|b|$, and $|c'|=|c|$, but also that, given our definitions of step arithmetic, we have $|c'|=|b'|-|a'|$, and thus $|c|=|b|-|a|$. With this in mind, observe $$\begin{align}
|c|^2&=|c|\cdot|c|\\
&=(|b|-|a|)\cdot(|b|-|a|)\\
&=|b|\cdot|b|-|b|\cdot|a|-|b|\cdot|a|+|a|\cdot|a|\\
&=|a|^{2}+|b|^{2}-2(a\cdot b)\\
&=|a|^{2}+|b|^{2}-2ab\cos(\t),
\end{align}$$yielding the result.
***
###### Part (c)
Let $\v,\w \in \R^3$. First, consider $$\begin{align}
|\v+w| ^2&=|\v+\w|\cdot|\v+\w|\\
&=|\v|\cdot|\v|+|\v|\cdot|\w|+|\v|\cdot|\w|+|\w|\cdot|\w|\\
&=|\v|^{2}+2\v\cdot\w+|\w|^{2}\\
\end{align}$$and$$\begin{align}

|\v-w|^{2}&=|\v-\w|\cdot|\v-\w|\\
&=|\v|\cdot|\v|-|\v|\cdot|\w|-|\v|\cdot|\w|+|\w|\cdot|\w|\\
&=|\v|^{2}-2\v\cdot\w+|\w|^{2},\\

\end{align}$$verifying that things still work as we'd expect in $\R^3$. Now then, *behold*$$\begin{align}

\frac{|\v+\w|^{2}+|\v-\w|^{2}}{2}&=\frac{|\v|^{2}+2\v\cdot\w+|\w|^{2}+|\v|^{2}-2\v\cdot\w+|\w|^{2}}{2}\\
&=\frac{2|\v|^{2}+2|\w|^{2}}{2}\\
&=|\v|^{2}+|\w|^{2},\\

\end{align}$$completing the proof. 
***
#### Problem 4
Recall that for $\R^2$ we talked about the operations of addition of steps and multiplication of a step by a scalar (real number). In this problem we will explore ways of multiplying two steps to each other in a way that produces a step. Consider the following multiplication operations on $\R^2$:$$\begin{eqnarray*}
(x,y)*(x',y') &=& (xx', yy')\\
(x,y)\circ(x',y') &=& (xx'- yy', xy'+x'y)
\end{eqnarray*}$$The second operation coincides with identifying $(x,y)$ with the {\em complex number} $x+iy$ and performing the usual multiplication of complex numbers.

(a) Do each of the operations $*$ and $\circ$ have multiplicative identity? 
Recall that a multiplicative identity for an operation $\square$ is an element $(\alpha, \beta)$ such that $(\alpha, \beta)\square(x,y)=(x,y)$ for all $(x,y)\in \R^2$.
(b) Do all elements in $\R^2\setminus\{(0,0)\}$ have multiplicative inverses with respect to each of the operations $*$ and $\circ$ ? 
Recall that a multiplicative inverse for an element $(x,y)\in \R^2$ with respect to an operation $\square$ which has multiplicative identity $(\alpha,\beta)$ is an element $(x',y')$ such that $(x,y)\square(x',y')=(x',y')\square(x,y)=(\alpha, \beta)$.
***
#### Problem 5
Consider a triangle with vertices at points $\u,\v,\w$. The *altitude* through a vertex is the line through that vertex perpendicular to the opposite side. 

(a) Prove that the altitude through $\u$ has equation $(\x-\u)\cdot (\v-\w)=0$. 
(b) Deduce that all three altitudes of a triangle meet at a point.
(c) The altitudes of a tetrahedron are defined similarly. Prove that all four altitudes of a tetrahedron meet at a point only if each pair of opposite edges is perpendicular.

##### *Proof.*
###### Part (a)
Let $A$ be a triangle with vertices at points $\u,\v,\w$.
Let $\x$ be a point in the altitude through $\u$. Note that as the altitude is perpendicular to $(\v-\w)$, they meet at a ninety degree angle. Thus, by the definition of the dot product we have $$(\x-\u) \cdot (\v-\w) = |\x-\u| \, |\v-\w| \cos(90)=0,$$as $\cos(90)=0$
***
###### Part (b)
Let $A$ be a triangle with vertices at points $\u,\v,\w$.
From Part (a) we see that the altitude through $\u$ has equation $(\x-\u)\cdot (\v-\w)=0$. Similarly, the altitude through $\v$ has equation $(\x-\v)\cdot (\w-\u)=0$. As these lines are not parallel they must intersect at some unique point $\bf{h}$. 

Notice then that $(\mathbf{h}-\w)\cdot(\u-\v)$ is equal to the following$$\begin{align}
&=(\mathbf{h}\cdot\u)-(\mathbf{h}\cdot\v)-(\w\cdot\u)+(\w\cdot\v)\\
&=(\mathbf{h}\cdot\u)-(\mathbf{h}\cdot\v)-(\w\cdot\u)+(\w\cdot\v)+0+0\\
&=(\mathbf{h}\cdot\u)-(\mathbf{h}\cdot\v)-(\w\cdot\u)+(\w\cdot\v)+(\mathbf{h}\cdot\w-\mathbf{h}\cdot \w)+(\u\cdot\v-\u\cdot\v)\\
&=-((\mathbf{h}\cdot\v)-(\mathbf{h}\cdot\w)-(\u\cdot\v)+(\u\cdot\w))+((\mathbf{h}\cdot\w)-(\mathbf{h}\cdot\u)-(\v\cdot\w)+(\v\cdot\u))\\
&=(\mathbf{h}-\u)\cdot(\v-\w)+(\mathbf{h}-\v)\cdot(\w-\u)\\
&=0,
\end{align}$$meaning that $\mathbf{h}$ lies on the altitude through $\w$. Thus all three altitudes of a triangle meet at $\mathbf{h}$.
***
###### Part (c)
Let $T$ be a tetrahedron. Note that by this Proposition (Prop 1.19 in the notes), we may reduce to the case where $T\sse\R^3$.

Let $\v_{1},\v_{2},\v_{3},\v_{4}$ denote the four vertices of a tetrahedron, and $\a_{1}, \a_{2}, \a_{3}, \a_{4}$ denote their respective altitudes. Suppose that each of the four altitudes of $T$ intersect at a point $p$. Observe$$0 = 0 - 0 = (\v_{4}-\v_{1}) \cdot (p-\v_{2}) - (\v_{4}-\v_{1})\cdot (p-\v_{3}) = (\v_{4}-\v_{1}) \cdot (\v_{2}-\v_{3}),$$given that $p$ lies on every altitude. Thus $\v_{4}-\v_{1}$ is perpendicular to $\v_{2}-\v_{3}$. An analogous equation yields $(\v_{1}-\v_{2}) \cdot (\v_{3}-\v_{4})=0$ as well. Thus each pair of opposite edges is perpendicular.