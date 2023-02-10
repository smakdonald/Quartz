# Functions and Their Graphs
## Functions
#### $\defn$ – Function
A *function* is a relationship between two variables for which a unique value of the output variable can be determined from a value of the input variable.

In other words, a function is relation in which every input corresponds to exactly one output.
#### $\defn$ – Input and Output
Given a function $f(x)$ and the equation $f(x)=y$, we say that $x$ is the *input* of $f(x)$ and $y$ is the *output* of $f(x)$.
$\rem$ – Functions are cool I promise
#### $\ex$ – Functions and Situations
- The relationship between a chair and the number of legs it has is a function when the chair is viewed as the input, and the number of legs is viewed as the output. This is because every input (chair) has exactly one output (number of legs). If you find a chair that simultaneously has two and four legs, please let me know right away. 
- The cost of filling up a car with gas is a function of the number of gallons purchased. The gas pump represents the function by displaying the corresponding values of the input variable (number of gallons) and the output variable (cost). again, this is a function because buying $5$ gallons of gas cannot cost both $\$20$ and $\$25$ at the same time, so each input has exactly one output!
#### $\ex$ – Functions and Tables
We can express relations using tables and determine whether or not they are functions that way as well. Consider the following table:

| Year (t) | Total Sales (S) |
| -------- | --------------- |
| 2000     | $612,000        |
| 2001     | $663,000        |
| 2002     | $692,000        | 
| 2003     | $749,000        |
| 2004     | $904,000        |

This table represents a function because each input (the values in the Year column) correspond to exactly one output (the values in the Total Sales column)
However, the following table

| Year (t) | Total Sales (S) |
| -------- | --------------- |
| 2000     | $612,000        |
| 2001     | $663,000        |
| 2002     | $692,000        |
| 2002     | $749,000        |
| 2004     | $904,000        |

Does *not* represent a function, as the input $2002$ has two different outputs.

#### $\rem$ – Functions and Tables
Functions can also describe literal tables. By substituting a chair for a table,[^1] the relationship between a table and the number of legs it has is a function when the table is viewed as the input, and the number of legs is viewed as the output.
#### $\thm$ – The Vertical Line Test
A graph represents a function if and only if every vertical line intersects the graph in at most one point.
#### $\ex$ – Functions and Graphs
Consider the following graphs:
![[Line Dance.svg]]
Graph (a) represents a function, as any vertical line we draw will only touch one point on the graph.
However, Graph (b) is not a function, as the vertical line drawn at $x=2$ intersects the graph at two points.
#### $\ex$ – Functions and Equations
- The line $y=2x+4$ represents a function, as any value of $x$ will give us exactly one value of $y$. 
#### $\nota$ – Functions
We express functions using the form $f(x)=y$, where $x$ represents the input of the function and $y$ represents the output. Said verbally, $f(x)=y$ means "$y$ is a function of $x$, and $f$ is the name of the function."

The symbol $f(x)$ is read "$f$ of $x$," is another name for the output, $y$ (as they are equal to each other).
#### $\war$ 
The parentheses in the symbol $f(x)$ do **not** indicate multiplication. Think of the symbol $f(x)$ as a single variable that represents the output value of the function. This is why you very rarely (hopefully never) see $f$ used as a variable, it is usually (always) reserved for functions. The same goes for $g$ and $h$ most of the time.
## Function Notation
### Interpreting the Inputs and Outputs of a Function
One of the most challenging parts of math are the word problems. Still, as functions are used to describe the world around us, it is important that we learn how to interpret them correctly. 
#### $\ex$ 
Let $f(t)$ be the total number of reported flu cases at UNL by the $t\th$ day of the semester. Then the units of the inputs are "days" and the units of the outputs are "flu cases".
- What does $f(103)$ mean?
- What does $f(50)$ mean?
- What does $f(15)=73$ mean?
- What is the meaning of $x$ in the statement $f(x)=56$?

##### Solution.
- $f(103)$ gives the number of flu cases by the $103$rd day of the semester. Notice that $t=103$ is the input of this function and $f(103)$ is the output. 
- $f(50)$ gives the number of flu cases by the $50$th day of the semester. Notice that $t=50$ is the input of this function and $f(50)$ is the output. 
- $f(15)=73$ means that there were $73$ flu cases by the $15\th$ day of the semester. Notice that $t=15$ is the input of this function and $f(15)=73$ is the output. 
- In the equation $f(x)=56$, $x$ would give the day(s) by which there were $56$ flu cases. Thus $f(x)$ is the output of the function and $x$ is the input.
#### $\defn$ – Evaluating a Function
Finding the value of the output variable that corresponds to a particular value of the input variable is called *evaluating the function*. If a function is described by an equation, we substitute the given input value into the equation to find the corresponding output, or function value.
#### $\rem$
Whenever a question says "evaluate", it is a pretty good indicator that we are plugging something in to a function.
#### $\ex$ – Evaluating a Number
Let $f(x)=2x-7$. 
(a) Evaluate $f(x)$ when $x=5$.
(b) Evaluate $f(5)$. 

##### Solution.
As it terns out, Parts (a) and (b) are asking the exact same thing. Our function is $f(x)=2x-7$, as both parts want us to plug in $5$ to $f(x)$. So we substitute: $$\begin{align*}
f(5)&= 2(5)-7\\
&= 10-7\\
&= 3.
\end{align*}$$Thus $f(5)=3$. 
#### $\ex$ – Evaluating a Variable
Evaluate the function $f(x)=4x^{2}-x+5$ for the following expressions.
(a) $x=2h$
(b) $x=a+3$

##### Solution.
As is the case with most math, this looks much scarier than it actually is. In fact, we are doing exactly what we did in the last example, just with letters instead of numbers. 
(a) Our function is $f(x)=4x^{2}-x+5$, and we want to evaluate $x=2h$. So we substitute: $$\begin{align*}
f(2h)&= 4(2h)^{2}-(2h)+5\\
&= 4(4h^{2})-2h+5\\
&= 16h^{2}-2h+5.
\end{align*}$$That's it! That's as far as we can go. It's okay that our answer has $h$'s in it, it's supposed to! 

(b) Our function is $f(x)=4x^{2}-x+5$, and we want to evaluate $x=a+3$. So we substitute: $$\begin{align*}
f(a+3)&= 4(a+3)^{2}-(a+3)+5\\
&= 4(a+3)(a+3)-a-3+5\\
&= 4(a^{2}+6a+9)-a+2.\\
&= 4(a^{2})+4(6a)+4(9)-a+2\\
&= 4a^{2}+24a+36-a+2\\
&= 4a^{2}+23a+38
\end{align*}$$Notice that placing parenthesis around $(a+3)$ when we substituted was essential in this problem. (Why?)
#### $\rem$ – Evaluating Variables
This concept of evaluating a variable will become increasingly relevant once we reach composite functions and function transformations. The important thing to remember is that a variable is just like a number, we just don't know which one! Just pretend it's a $3$ and see how it would behave.
#### $\ex$
(a) Let $f(x)=7x-2$. Find all values of $x$ such that $f(x)=12$.
(b) Let $g(x)=2x^{2}$. Find all values of $x$ such that $f(x)=8$.

##### Solution.
(a) Since $f(x)=7x-2$ and we want $f(x)=12$, we have $12=f(x)=7x-2$, so we can cut out the middle man and say $12=7x-2$. Thus is something we can solve! Observe: $$\begin{align*}
12&= 7x-2\\
14&= 7x\\
2&= x.
\end{align*}$$Thus $x=2$ is our answer.

(b) Since $g(x)=2x^{2}$ and we want $g(x)=8$, we have $8=g(x)=2x^{2}$, so we can cut out the middle man and say $8=2x^{2}$. By dividing both sides by $2$ we have $4=x^2$. So we take the square root of both sides to find $x=\pm2$. This is because $2^2=4$ **and** $(-2)^{2}=4$. So there are two answers, and we write $x=-2,2$.


## Domain and Range
#### $\defn$ – Undefined
As we talked about in class, an operation is *undefined* if, well, there is no defined answer. A bit circular, but it basically means there are certain operations that are "off limits" to us. For this class, there are three operations we need to keep an eye out for:
- Dividing by zero, such as $\frac{1}{0}$.
- Taking the square root of a negative number, such as $\sqrt{-1}$.
- Taking the logarithm of a negative number or $0$. (We'll get to this later, don't worry)
#### $\rem$ – Imaginary Numbers
Technically we can take the square root of a negative number, this is what is called an *imaginary* number. Unfortunately there will be no such imagination in this class.
![[In a World of Pure Imagination.jpg|300]]
#### $\defn$ – Domain and Range
The *domain* of a function is the set of permissible values for the input variable. The *range* is the set of function values (that is, values of the output variable) that correspond to the domain values.
#### $\ex$
When viewed as a function, we can finally answer the famous conjecture posed by Eurodance sensations Rednex in 1995:

>Where did you come from, where did you go? Where did you come from, Cotton-Eye Joe?

Using the vocabulary of functions, we see that Cotton-Eye Joe came from the domain of the function, and where he went was the range.
### Domain and Range from a Graph
We can identify the domain and range of a function from its graph. The domain is the set of $x$-values of all points on the graph, and the range is the set of $y$-values.
#### $\ex$ 
See [Example 117](https://mathbooks.unl.edu/PreCalculus/Domain-Range.html) in the textbook (sorry, strapped for time)

### Finding the Domain from a Formula
If the domain of a function is not given as part of its definition, we assume that the domain is as large as possible. We include in the domain all $x$-values that make sense when substituted into the function's formula. In other words, we take out all the points that would make our function undefined.
#### $\ex$
See [Example 131](https://mathbooks.unl.edu/PreCalculus/Domain-Range.html) in the textbook (sorry, strapped for time)

## Rates of Change
### Increasing and Decreasing
#### $\defn$ – Intervals
- An *interval* is a set that consists of all the real numbers between two numbers $a$ and $b$. 
- A *closed interval* is an interval that contains its endpoints, which we denote using square brackets (squackets): $[a,b]$. 
- An *open interval* is an interval that does not contain its endpoints, which we denote using parenthesis (squackets): $(a,b)$. If a number $x$ is in the interval $(a,b)$, we write $a< x< b$.
- An *infinite* interval is an interval that goes on forever in one or both directions. 
- Some intervals are closed on one end and open on the other. We call such an interval a *half-open* or *half-closed* interval.
- We can combine two or more intervals into a larger set. This is called the *union* of two (or more) intervals, and we use the notation $\cup$ to denote it.
#### $\nota$ – Interval Notation
- If $a\leq x$, we write $[a,\infty)$; If $a< x$, we write $(a,\infty)$
- If $x< b$, we write $(-\infty,b]$; If $x< b$, we write $(-\infty,b)$
- If $a\leq x\leq b$, we write $[a,b]$; If $a< x< b$, we write $(a,b)$
- If $a< x\leq b$, we write $(a,b]$; If $a< x\leq b$, we write $(a,b]$
- If $a\leq x\leq b$, or $c\leq x\leq d$ we write $[a,b]\cup[c,d]$. 
#### $\war$ 
Do not confuse the open interval $(-2,2)$ with the point $(-2,2)$! The notation is the same, so you must decide from the context whether an interval or a point is being discussed. I'm not happy about it either :(
#### $\ex$ 
See [Example 39](https://mathbooks.unl.edu/PreCalculus/Rates-of-Change.html) in the textbook.
#### $\rem$ – Unions of Intervals and WeBWorK
When typing a union of intervals into WeBWorK, you can use a capital U and WebWork will accept it.  It does need to be upper case, though.
#### $\defn$ – Increasing and Decreasing
Let $y=f(x)$ where $a≤x≤b.$ 
- Then the function $f(x)$ is said to be *increasing* on $(a,b)$ if the value of $f(x)$ increases as $x$ increases on $(a,b).$
- Then the function $f(x)$ is said to be *decreasing* on $(a,b)$ if the value of $f(x)$ decreases as $x$ increases on $(a,b)$
### Slope
#### $\defn$ – Slope
The *slope* of a line is the ratio $$\frac{\text{change in}\, y \text{-coordinate}}{\text{change in}\, x \text{-coordinate}}$$as we move from one point to another on the line.
#### $\nota$ – Slope
The slope of a line is given by $$\frac{\Delta y}{\Delta x}=\frac{\text{change in}\, y \text{-coordinate}}{\text{change in}\, x \text{-coordinate}}, \Delta x\neq0.$$The $\Delta$ here means "change". 
#### $\ex$ 
See [Examples 48 and 51](https://mathbooks.unl.edu/PreCalculus/Rates-of-Change.html) in the textbook (sorry, strapped for time)
#### $\form$ – Slope Formula
The slope of the line passing through the points $(x_{1},y_{1})$ and $(x_{2},y_{2})$ is given by $$m=\frac{\Delta y}{\Delta x}=\frac{y_{2}-y_{1}}{x_{2}-x_{1}},x_{2}\neq x_{1}$$Written using function notation, this is equivalent to (the same as) the following: $$m=\frac{\Delta y}{\Delta x}=\frac{f(x_{2})-f(x_{1})}{x_{2}-x_{1}},x_{2}\neq x_{1}$$
#### $\defn$ – Rate of Change
The slope of a line measures the *rate of change* of the output variable with respect to the input variable.
#### $\rem$ – Rate of Change and Slope of Lines
For the purposes of this class, slope and rate of change are the same thing. When a question asks you for the rate of change, it is *really* asking you for the slope of the line. 
#### $\ex$ 
Steve goes on a road trip. He travels a total of $955$ miles, and the trip takes $19$ hours from start to finish. What is his average rate of change of distance? Please include units in your answer.

##### Solution.
Steve's initial position is $0$ miles from the starting place at time $0$ hours and he arrives at his destination after traveling $955$ miles over $19$ hours. You can break this down to use the average rate of change formula with ordered pairs $(0,0)$ and $(19,955)$. Then the average rate of change of distance is $$\frac{955-0}{19-0}=50.26$$Since we are taking a distance in miles divided by a time in hours, the units are mi/hr.
## Linear Functions
#### $\defn$ – Linear Equation
A *linear function* is a function which has a constant rate of change. It is also a function whose graph is a line.
#### $\ex$ – Linear Functions and Tables
Does the following table represent a linear function?

| $x$  | $f(x)$ |
| ---- | ------ |
| $0$  | $-2$   |
| $3$  | $4$    | 
| $6$  | $10$   |
| $23$ | $44$   |

##### Solution.
In order for a function to be linear, it needs to have a constant average rate of change. Therefore, to determine if these tables represent linear functions, we need to calculate the average rate of change over each interval on the table. Recall that this is the same thing at finding the slope over each interval.

- On the interval $[0,3]$, we have $m=\frac{4-(-2)}{3-0}=\frac{6}{3}=2$.
- On the interval $[3,6]$, we have $m=\frac{10-4}{6-3}=\frac{6}{3}=2$
- On the interval $[6,23]$, we have $m=\frac{44-10}{23-6}=\frac{34}{17}=2$

Since each interval results in the same average rate of change, this function is linear.
#### $\defn$ – $y$-Intercept
A *vertical intercept* is a point where a graph intersects the vertical axis. For a function $f$, the vertical intercept of the graph of $f$ is the point $(0,f(0))$. Because we often use the variable $y$ on the vertical axis, the vertical intercept is often called the $y$-intercept.

To find the vertical intercept of a graph, plug in the value $x=0$ to your function and solve for $y$. 
#### $\ex$ – Finding Vertical Intercepts
Find the $y$-intercept of the function $y=f(x)=2x-76$.

##### Solution.
To find the vertical intercept of a graph, we plug in the value $x=0$ to our function. Thus $f(0)=2(0)-76=-76$. Thus the $y$-value of the $y$-intercept is $-76$. Not so bad!

We can observe this visually in the following graph of $2x-76$:
```functionplot
---
title: 
xLabel: 
yLabel: 
bounds: [-50,100,-100,50]
disableZoom: true
grid: true
---
f(x)=2x-76
```
#### $\rem$ – Ho Ho Ho(ordinate Axes)
![[The Most Wonderful Time of the Year.jpg|300]]
#### $\nota$ – Vertical Intercepts
For simplicity, we often use the variable $b$ for $f(0)$ so that the vertical intercept of a function $f$ is at $(0,b)$.
#### $\defn$ – Slope-Intercept Form
If we write an equation of a linear function in the form, $$f(x)=mx+b$$then $m$ is the slope of the line, and $b$ is the $y$-coordinate of the $y$-intercept of the line.
#### $\defn$ – $x$-Intercept
An $x$-intercept is a point where a graph intersects the $x$-axis. It corresponds to the point $(a,0)$ where a is a value such that $f(a)=0$.

To find the horizontal intercept of a graph, we set our function equal to $0$ and solve for $x$. 
#### $\ex$ – Finding Horizontal Intercepts
Find the $y$-intercept of the function $y=f(x)=2x-76$.

##### Solution.
To find the vertical intercept of a graph, we set our function equal to $0$ and solve for $x$. Thus we have $$\begin{align*}
0&=2x-76\\
76&= 2x\\
38&= x.
\end{align*}$$Thus our $x$-intercept is when $x=38$
We can observe this visually in the following graph of $2x-76$:
```functionplot
---
title: 
xLabel: 
yLabel: 
bounds: [-50,100,-100,50]
disableZoom: true
grid: true
---
f(x)=2x-76
```

#### $\form$ – Slope-Intercept Method for Graphing a Line
(a) Plot the point associated with the vertical intercept, $(0,b)$.
(b) Use the definition of slope to find a second point on the line: Starting at the vertical intercept, move $\Delta y$ units in the $y$-direction and $\Delta x$ units in the $x$-direction. Plot a second point at this location.
(c) Use an equivalent form of the slope to find a third point, and draw a line through the points.
![[Up and Over.svg]]
## Finding Linear Functions
[Textbook](https://mathbooks.unl.edu/PreCalculus/Finding-Linear-Functions.html)
### Point-Slope Form
#### $\ex$ – Finding Equations in Slope-Intercept Form
Tiberius Fang owns a catering business. For any party with up to $200$ guests, he charges $\$4000$. For each additional guest over $200$ he charges $\$20$ per person. Give a formula for the cost in dollars $C$ of having Tiberius Fang cater your party as a function of $p$, the number of guests over $200$.

##### Solution.
Since Tiberius Fang charges $\$4000$ for parties up to $200$ guests, the initial value of this function is $\$4000$. Notice that since represents the number of guests over $200$, parties with 200 guests would be when $p=0$. Tiberius Fang charges $\$20$ for each guest over $200$. So, for every increase in one person (over $200$), the total cost increases by $\$20$. This gives the slope of the function.

Therefore, $C(p)=20p+4000$.
#### $\ex$ – Finding Equations from Graph
Find an equation for the line shown in the graph below:
![[Slope.svg]]

##### Solution. 
The line crosses the $y$-axis at the point $(0,3200)$, so $b=3200$. To calculate the slope of the line, we locate another point, say $(20,6000)$, and compute: $$\begin{align*}
m &= \frac{\Delta y}{\Delta x}\\
&= \frac{y_{2}-y_{1}}{x_{2}-x_{1}}\\
&=\frac{6000-3200}{20-0}\\
&= \frac{2800}{20}\\
&= 140.
\end{align*}$$The slope-intercept form of the equation, with $m=140$ and $b=3200$, is $$y=140x+3200$$
#### $\defn$ – Point-Slope Form
An equation of the line that passes through the point $(x_{1},y_{1})$ and has slope $m$ is $$y=m(x-x_{1})+y_{1}$$
#### $\ex$ – Equation from Slope and Point
Find an equation for the line that passes through $(1,-4)$ and has slope $-\frac{3}{4}$.

##### Solution.
We have two formulas for lines: Point-Slope and Slope-Intercept. As we have been given a slope and a point to work with, I'm gonna go with Point-Slope on this one. Recall that an equation of the line that passes through the point $(x_{1},y_{1})$ and has slope $m$ is $$y=m(x-x_{1})+y_{1}.$$The slope we were given is $m=-\frac{3}{4}$ and the point is $(x_{1},y_{1})=(1,-4)$. All that is left to do is substitute:
$$y=-\frac{3}{4}(x-1)-4.$$
#### $\rem$ – Point Slope is your Friend (Not Food)
Due to repetitive K-12 algebra classes, many students feel a compulsive need to write all lines in Slope-Intercept form. You don't need to do that anymore if you don't want to. It is perfectly fine to leave lines in Point-Slope form, as I did above. In fact, I actually encourage it. 
#### $\ex$ – Equation from Two Points
Find an equation for the line that passes through $(-2,3)$ and $(5,6)$

##### Solution.
This also looks like a great time for the Point-Slope formula, we just need a slope! Luckily for us, two points are exactly enough to find the slope, given that the slope of a line is the ratio $$m=\frac{y_{2}-y_{1} }{x_{2}-x_{1}}.$$ With a little more substitution we see $$\begin{align*}
m&= \frac{y_{2}-y_{1} }{x_{2}-x_{1}}\\
&= \frac{6-3}{5-(-2)}\\
&= \frac{3}{7}
\end{align*}.$$Now, once we plug our slope and one of our points (it doesn't matter which one) into the Point-Slope formula, we will be done! Observe: $$\begin{align*}
y&=m(x-x_{1})+y_{1}\\
&= \frac{3}{7}(x-5)+6.
\end{align*}$$
## Comparing Linear Functions
[Textbook](https://mathbooks.unl.edu/PreCalculus/Comparing-linear-functions.html)
#### $\defn$ – Horizontal and Vertical Lines
For any constant $k$:
- The graph of the equation $y=k$ is a *horizontal line* through $(0,k)$ and its slope is zero.
- The graph of the equation $x=k$ is a vertical line through $(k,0)$ and its slope is undefined. (Why?)
#### $\rem$ – Vertical Lines
Notice that the equation of a vertical line is *not* a function. we can justify this using the Vertical Line test. Specifically, I can think of one vertical line in particular that might cause some problems...
#### $\defn$ – Parallel and Perpendicular Lines
Let $l_1:y=m_{1}x+b_{1}$ and $l_2:y=m_{2}x+b_{2}$ be two lines. We say that
- $l_1$ and $l_2$ are *parallel* if $m_{1}=m_{2}$ and $b_{1}\neq b_{2}$.
- $l_1$ and $l_2$ are *perpendicular* if $m_{1}=\frac{-1}{m_{2}}$. (Opposite reciprocal)
#### $\ex$ – Finding Parallel Line
Find the equation of a line passing through the point $(4,-1)$ and parallel to the line $y=3x+2$.

##### Solution.
Since the two lines are parallel we know that the slope of the new line must be the same as the slope of the original line. That is, $m_{1}=3=m_{2}$. We can now use point slope form $y=3(x-4)-1$. 

At this point we have the equation of a line. However, most people are more comfortable writing lines in slope-intercept form so we will do that here: $y=3x-13$.
#### $\ex$ – Finding Perpendicular Line
Find the equation of a line passing through the point $(4,-1)$ and perpendicular to the line $y=3x+2$.

##### Solution.
Since the two lines are perpendicular we know that the slope of the new line must be the opposite reciprocal of the slope of the original line. Since $m_{1}=3, m_{2}=-\frac{1}{3}$. We can now use point slope form $y=-\frac{1}{3}(x-4)-1.$
#### $\rem$ – Quality Time
![[Parallel.png|300]]
# Quiz One – What to Know
-  Be able to identify when a table, graph, or equation represents a function.
- Given a function, be able to evaluate given inputs and solve for given outputs.
- Be able to find the domain and range of a function from a graph or equation and express it using interval notation.
- Be able to find the rate of change given an equation, graph, or real world situation. 
- Be able to include units in your answer if asked (please don't forget units!)

[^1]: After all, what is a table if not an acoustic chair?