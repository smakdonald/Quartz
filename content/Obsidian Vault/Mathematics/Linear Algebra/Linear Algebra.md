# Linear Equations
## Systems of Linear Equations
#### $\defn$ – Linear Equation
A *linear equation* in the variable $x_1,x_2,\dots, x_n$ is an equation that can be written in the form $$a_1x_1+a_2x_2+\cdots +a_nx_n=b$$where $b$ and the *coefficients* $a_1, a_2, \dots, a_n$ are real (or complex) numbers. The subscript $n$ is a positive integer.
#### $\ex$ – Identifying Linear Equations
Which are linear equations? Which are not? 
   $$\begin{align*}
   3x_1+2x_2=-6 & & \pi x_2-5x_1+x_3=\sqrt{3} & & x_1x_2+x_3^2=17 \\ \\ \\  & 1.5x_1-3=2x_2 & & \sqrt{x_1}+x_2=3 & &\\
   \end{align*}$$
#### $\defn$ – Linear System
A *system of linear equations*, or a *linear system*, is a collection of linear equations involving the same variables, say $x_1,x_2,\dots, x_n$. 
#### $\ex$ – Linear Equations
Here three different examples of systems of linear equations.
$\begin{align*}3x_1-x_2+2.5x_3=2\\2x_1+x_2+2x_3=2\\-x_1+5.2x_3=4.5\end{align*}$

$\begin{align*}x_1-x_2+2x_3=2\\2x_1+5x_2=5\end{align*}$

$\begin{align*}x_1-x_2=2\\x_1+2x_2=-4\end{align*}$
#### $\defn$ – Solution
A *solution* is a list of numbers $(s_1, \dots, s_n)$ that makes each equation in the system of linear equations true when substituted for $x_1,x_2,\dots, x_n$, accordingly. The set of all possible solutions is a *solution set* and if two systems have the same solution sets the systems are called *equivalent*.
#### $\ex$ – Determining Solution
Determine if $(1,0,-2)$ is a solution to the following system of linear equations.
$\begin{align*}x_1-x_2+2x_3=-3\\2x_1+5x_2=2\\\end{align*}$
#### $\ex$ – Finding Solution
Find a solution to the third system given in the prior example.
#### $\ex$ – Number of Solutions
How many solutions could the following linear system in variables $x_1$ and $x_2$ have, where $a_1, a_2, c_1, c_2, b,d$ are all numbers? (Hint:} Think about the graphs of these equations would look like. Maybe replace $x_1$ with $x$ and $x_2$ with $y$ and solve for $y$ to get something familiar...)
$\begin{align*}a_1x_1+a_2x_2=b\\c_1x_2+c_2x_2=d\end{align*}$
#### $\thm$ – Solutions to Linear Systems
Every system of linear equations has no solution, one solution, or infinitely many solutions.
#### $\defn$ – (In)Consistent
If a linear system has either one solution or infinitely many solutions, we say the linear system is *consistent*. Otherwise, the system is *inconsistent*.
### Matrices
#### $\defn$ – Matrix
We can record the essential information from a linear system into a rectangular array, which we call a matrix}. For example, consider the system 
$\begin{align*}4x_1+4x_3=16\\x_1+x_2+2x_3=6\\6x_2+2x_3=0\end{align*}$
The *coefficient matrix* (or matrix of coefficients) is


and the *augmented matrix* is

By convention, we talk about the size of a matrix by prioritizing the rows. So the size of a matrix with $m$ rows and $n$ columns is an $m\times n$ matrix.
### Solving a Linear System
#### $\ex$ – Solving Linear System
Solve the system on the prior page. 
$\begin{align*}4x_1+4x_3&=16\hspace{5in}&\\ x_1+x_2+2x_3&=6\hspace{5in}&\\6x_2+2x_3&=0\hspace{5in}&\end{align*}$
First, just do it algebraically, labeling replacements with stuff like $E_1\rightarrow E_2-E_1$. Then, when done, do it with matrices, labeling stuff like $R_1\rightarrow R_2-R_1$.

Start with interchanging the first and second rows, and isolating $x_1$. (Make sure to do +(-4)$R_2$, stuff like that, not $-4R_2$.

Then move on to scale row 2 by -1/4. 

Then cancel row $x_2$ in row 3. 

Point out triangular form}. Could be done here, but let's keep going. (Only if room)

Then test the solution against the original.

Comment at the end that in general you don't need the extra equations, I just did it so you can see that everything I'm doing to the matrix corresponds to what I'm doing to the equations.
#### $\defn$ – Elementary Row Operations
- (Replacement) Replace any row with itself plus a multiple of another row.
- (Interchange) Interchange two rows.
- (Scaling) multiple the entries of a row by a nonzero constant.
Two matrices related by elementary row operations are said to be *row equivalent*.
#### $\rem$
The matrices on the prior page are hence all row equivalent.
#### $\thm$ – Row Equivalence and Solution Sets
If the augmented matrices of two linear systems are row equivalent, then the two systems have the same solution set (that is, the same solutions).
### Existence and Uniqueness
#### $\ex$ – Determining Consistency
Determine if the following system is consistent or inconsistent. 
$\begin{align*}2x_2+3x_3=2\\x_1+3x_2+x_3=6\\2x_1+8x_2+5x_3=15\end{align*}$

interchange rows 1 and 2, replace row 3 with itself plus -2 times row 1, two rows are now opposite
#### $\ex$ – Making System Consistent
Determine the value(s) of $h$ such that the matrix is the augmented matrix of a consistent linear system. Then find the value(s) of $h$ so that the system is inconsistent.
$\begin{align*}\begin{bmatrix}1 & h & 3\\2 & 4 & 10\end{bmatrix}\end{align*}$
#### $\ex$ – Determining Consistency (2)
Determine if the following system is consistent or inconsistent. 
$\begin{align*}2x_2+3x_3=2\\x_1+3x_2+x_3=6\\2x_1+8x_2+5x_3=14\end{align*}$
## Row Reduction and Echelon Forms
#### $\defn$ – Leading Term
the *leading entry* of a row is the first nonzero entry of that row. 
#### $\defn$ – Echelon Form
A rectangular matrix is in *echelon form* (or row echelon form}) if it has the following three properties. 
(1) All nonzero rows are above any rows of all zeros.
(2) Each leading entry of a row is in a column to the right of the leading entry of the row above it.
(3) All entries in a column below a leading entry are zeros.

In this case, we call the matrix an *echelon* matrix. If a matrix is echelon form and satisfies the following additional properties, then it is in *reduced row echelon form* (or row reduced echelon form).

(4) The leading entry in each nonzero row is 1. 
(5) Each leading 1 is the only nonzero entry in its column.
In this case, we call the matrix a *reduced echelon* matrix.
#### $\ex$ – Echelon and Reduced Echelon
Below we have an echelon matrix to the left, and a reduced echelon matrix to the right.
$$\begin{align*}
\begin{bmatrix}
2 & -3 & 0 & 1\\
0 & 1 & 3/2 & 9\\
0 & 0 & 0 & 6
\end{bmatrix} & & 
\begin{bmatrix}
1 & 0 & 0 & 12\\
0 & 1 & 0 & 91.5\\
0 & 0 & 1 & -3
\end{bmatrix}
\end{align*}$$
#### $\ex$ – Identifying Echelon Form
For each matrix, is it in reduced echelon form, echelon form but not reduced echelon form, or neither? 
$$\begin{align*}
\begin{bmatrix}
2 & -3 & 0 & 1\\
0 & 1 & 3/2 & 9\\
0 & 1 & 2 & 6
\end{bmatrix} & & 
\begin{bmatrix}
0 & 0 & 0 & 0 & 0\\
2 & -3 & 0 & 1& 76\\
0 & 1 & 3/2 & 9& 1\\
0 & 0 & 2 & 6& 13
\end{bmatrix} & & 
\begin{bmatrix}
1 & 0 & 0 & 2\\
0 & 1 & 0 & 1.5\\
0 & 0 & 2 & -3
\end{bmatrix}& & 
\begin{bmatrix}
1 & 2  & 0 & 1\\
0 & 0 & 1 & 1\\
0 & 0 & 0 & 0
\end{bmatrix}
\end{align*}$$
#### $\thm$ – Equivalent Echelon Matrix Unique
Each matrix is row equivalent to one and only one reduced echelon matrix.
### Pivot Positions
#### $\defn$ – Pivot Position
A *pivot position* in a matrix $A$ is a location in $A$ that corresponds to a leading 1 in a row in the reduced echelon form of $A$. 

A *pivot column* is a column of $A$ that contains a pivot position.
#### $\ex$ – Labeling Pivot Positions
$A$ is row reduced in several steps below to echelon form. Label the pivot columns and positions on $A$.
$$\begin{align*}
A=\begin{bmatrix}
4 & 0 & 4 & 16\\
1 & 1 & 2 & 6\\
0 & 6 & 2 & 0
\end{bmatrix}
\end{align*}$$
$$\begin{align*}
\text{interchange R1 and R2} & & \begin{bmatrix}
1 & 1 & 2 & 6\\
4 & 0 & 4 & 16\\
0 & 6 & 2 & 0
\end{bmatrix}\\ \\
\text{replace R2 with R2--4$\cdot$R1} & & \begin{bmatrix}
1 & 1 & 2 & 6\\
0 & -4 & -4 & -8\\
0& 6 & 2 & 0
\end{bmatrix}\\ \\
\text{Replace R3 with R3+${6\over 4}\cdot$R2} & & \begin{bmatrix}
1 & 1 & 2 & 6\\
0 & -4 & -4 & -8\\
0& 0 & -4 & -12
\end{bmatrix}\\
\end{align*}$$

The entries in the pivot position are called *pivots*. Note that they (eventually) are a nonzero number, but may not be to start.
### The Row Reduction Algorithm
#### $\ex$ – Using Row Reduction Algorithm
Row reduce the following into echelon form, then reduced echelon form.
$$\begin{align*}
\begin{bmatrix}
0 & 3 &6& 4\\
3& -7& -5& 8\\
3& -9& -9& 6
\end{bmatrix}
\end{align*}$$

Step 1: Begin with the leftmost nonzero column. This is a pivot column. The pivot position is at the top.

Step 2: Select a nonzero entry in the pivot column as a pivot. If necessary, interchange rows to move this entry into the pivot position. 

Step 3: Use row replacement operations to create zeros in all positions below the pivot.

Step 4: Repeat steps 1--4 on the rows below the pivot position you just created until there are no more nonzero rows.

Step 5: Beginning with the rightmost pivot and working upward and to the left, create zeros above each pivot. If a pivot is not 1, make it 1 by a scaling operation. 

### Solutions of Linear Systems
#### $\ex$ – Reduced Matrix
Suppose you have an augmented matrix, and after applying the row reduction algorithm, you row reduce the matrix to the following reduced echelon matrix
$$\begin{align*}
\begin{bmatrix}
1 & 0 & 3 & 2\\
0 & 1 &2  & -5\\
0 & 0 & 0 & 0\\
\end{bmatrix}.
\end{align*}$$

This system corresponds to the following system of linear equations:

Note that $x_1$ and $x_2$ correspond to pivot columns. We call these variables *basic* variables. The other variable, $x_3$, is a *free* variable.

The above system has the following general solution:

In other words, we can make any choice we want for the free variable $x_3$, and this determines the basic variables $x_1$ and $x_2$. 
#### $\ex$ – Simplifying Solutions to Matrix
What would the general solution to the following matrix be, if it is left in echelon form? Is the solution as simple as it can be? 
$$\begin{bmatrix}
1 & 2 & 7 & -8\\
0 & 1 & 2  & -5\\
0 & 0 & 0 & 0\\
\end{bmatrix}$$

Reduced echelon form does more---let's look at the next example.
#### $\ex$ – General Solution of Augmented Matrix
Find the general solution of the linear system whose augmented matrix has been reduced to the following reduced echelon matrix. Which variables are the free variables? Which are basic?$$\begin{align*}
\begin{bmatrix}
1 & -4 & 0 & 4 & 0 & -6\\
0 & 0 & 1 & 13 & 1 & 2\\
0 & 0 & 0 & 0 & 1 & 10\\
0 & 0 & 0 & 0 & 0 & 0\\
\end{bmatrix}
\end{align*}$$
### Existence and Uniqueness
#### $\ex$ – Matrices with Different Solution Numbers
The following matrices correspond to three different linear solutions so that one a no solutions, one has 1 (i.e. a unique) solution, and one has infinitely many solutions. Which is which? Point out the pivot columns.
Comment these aren't in reduced echelon form. Try to prove the theorem with them.}
$$\begin{align*}
\begin{bmatrix}
1 & 0 & 2 & 4.5\\
0 & 2 & 2 & 3\\
0 & 0 & 1 & -9\\
\end{bmatrix}
& & 
\begin{bmatrix}
1 & 0 & 2 & 3\\
0 & 0 & 1 & 6\\
0 & 0 & 0 & 0\\
\end{bmatrix}
 & & 
\begin{bmatrix}
1 & 0 & 2 & 0\\
0 & 3 & -2.5 & 0\\
0 & 0 & 0 & 2\\
\end{bmatrix}
\end{align*} $$
#### $\thm$ – Consistency and Pivot Columns
A linear system is consistent if and only if the rightmost column of the augmented matrix is not a pivot column---that is, if and only if an echelon form of the augmented matrix has no row of the form
$$[0 \ \ \  0 \ \ \  0 \ \ \  \cdots \ \ \  0 \  \ \ b], \text{ with $b$ nonzero.}$$
If a linear system is consistent, then the solution set contains either
- a unique solution, when there are no free variables; or
- infinitely many solutions, when there is at least one free variable. 
#### $\rem$ember---identifying basic variables is the same as identifying pivot columns!
#### $\ex$ – Identifying Consistency
- Suppose each * can be any number (not all necessarily the same), and each $\blacksquare$ can be any nonzero number (not all necessarily the same). Assume each of the following are augmented matrices for a linear system. Is the system consistent or inconsistent? If consistent, is the solution unique?  
$$\begin{align*}
\begin{bmatrix}
\blacksquare & * & * & * & *\\
0 & \blacksquare & * & * & *\\
0 & 0 & 0 & \blacksquare & *\\
\end{bmatrix} && 
\begin{bmatrix}
\blacksquare & * & * & * & *\\
0 & 0 & 0 & 0 & \blacksquare\\
\end{bmatrix} 
\end{align*}$$
- Suppose the coefficient matrix of a linear system of three equations in three variables has a pivot in each column. Explain why the system has a unique solution. 
- A $2\times 4$ coefficient matrix has two pivot positions. Is the corresponding system consistent? Is the solution unique? Explain.
#### Algorithm – Solving Linear Systems
- Write the augmented matrix of the system. 
- Use the row reduction algorithm to obtain an augmented matrix in echelon form. Decide whether the system is consistent. If there is no solution, stop; otherwise go to the next step. 
- Continue row reduction to obtain the reduced echelon form. 
- Write the system of equations corresponding to the matrix obtained in step 3. 
- Rewrite each nonzero equation from step 4 so that its one basic variable is expressed in terms of any free variables appearing in the equation.
## Vector Equations
### Vectors in $\R^2$
#### $\defn$ – Vector
A matrix with one column is called a *column vector*, or a *vector* when clear. 
#### $\ex$
#### $\rem$
#### $\defn$ – Equal Vectors
Two vectors in $\R^2$ are equal if and only if their corresponding entries are equal.
#### Warning
#### $\defn$ – Sum of Vectors
Given two vectors $\u$ and $\v$ in $\R^2$, their sum is the vector $\u+\v$ obtained by adding
corresponding entries of $\u$ and $\v$.
#### $\ex$
#### $\defn$ – Scalar Multiple
Given a vector $\u$ and a real number $c$, the *scalar multiple* of $\u$ by $c$ is the vector $c\u$
obtained by multiplying each entry in $\u$ by $c$. The number $c$ in $c\u$ is called a *scalar*; it is written in lightface type to distinguish it from the boldface vector $\u$.
#### $\ex$
#### $\ex$
### Geometric Description of $\R^2$
#### $\ex$
#### Rule
#### $\ex$
#### $\ex$
### Vectors in $\R^3$ and $\R^n$
#### $\prop$ – Algebraic Properties of $\R^n$
For all $u$, $v$, $w$ in $\R^n$ and all scalars $c$ and $d$:
(a)  $\u+\v=\v+\u$
(b)  $(\u+\v)+\w=\u+(\v+\w)$
(c)  $\u+0=0+\u=\u$
(d)  $\u+(-\u)=-\u+\u=0$, where $-\u$ denotes -$1(\u)$
(e) $c(\u+\v)=c\u+c\v$
(f) $(c+d)\u=c\u+d\u$
(g) $c(d\u)=(cd)\u$
(h) $1\u=\u$

##### *Proof.*
#### $\rem$
### Linear Combinations 
#### $\defn$ – Linear Combination
#### $\ex$
#### $\ex$
#### $\ex$
#### $\thm$
A vector equation
$$x_1\ba_1+x_2\ba_2+\cdots +x_p\ba_p=\bb$$
has the same solution set as the linear system whose augmented matrix is 
$$\begin{bmatrix} a_1 & a_2 & \dots & a_n & b \end{bmatrix}$$
In particular, $\bb$ is the linear combination of $\ba_1,\dots, \ba_p$ if and only if there exists a solution to the linear system corresponding to this matrix (that is, the linear system is consistent).
#### $\ex$
#### $\defn$ – Span
If $\bv_1,\bv_2,\dots, \bv_p$ are in $\R^n$, then the set of all linear combinations of $\bv_1,\bv_2,\dots, \bv_p$ is denoted $\Span\{\bv_1,\dots, \bv_p\}$, and is the subset of $\R^n$ *spanned* (or generated) by $\bv_1,\dots, \bv_p$. That is, $\Span\{\bv_1,\dots, \bv_p\}$ is the collection of all vectors that can be written as 
$$c_1\bv_1+\cdots +c_p\bv_p,$$where $c_1,\dots, c_p$ are scalars.
#### $\rem$
#### Warning
### Geometric Description of $\Span\{\bv\}$ & $\Span\{\bu, \bv\}$
### Linear Combination Applications
#### $\ex$
## The Matrix Equation
#### $\defn$ – Vector-Matrix Product
Let $A$ be an $m\times n$ matrix, with columns $\ba_1,\ba_2, \dots, \ba_n$. That is, $\ba_1,\ba_2, \dots, \ba_n$ are in $\R^m$ so that
$$A=\begin{bmatrix}
\ba_1&\ba_2& \dots & \ba_n
\end{bmatrix}.$$
Let $\bx$ be a vector in $\R^n$, that is, there are real numbers $x_1,\dots, x_n$ so that $$\bx=\begin{bmatrix}
x_1\\ \vdots \\ x_n\end{bmatrix}.$$ Then *product* of $A$ and $\bx$, denoted $A\bx$, is the linear combination of the columns of $A$ using the corresponding entries of $\bx$ as weights; that is,
$$A\bx=\begin{bmatrix}
\ba_1&\ba_2& \dots & \ba_n
\end{bmatrix} \begin{bmatrix}
x_1\\ \vdots \\ x_n\end{bmatrix}=x_1\ba_1+\dots+x_n\ba_n$$
#### Warning
#### $\ex$
#### $\ex$
#### $\thm$
If $A$ is an $m\times n$ matrix, with columns $\ba_1,\dots, \ba_n$, and if $\bb$ is in $\R^m$, the matrix equation $$A\bx=\bb$$has the same solution set as the vector equation
$$x_1\ba_1+x_2\ba_2+\cdots+x_n\ba_n=\bb,$$
which in turn, has the same solution set as the system of linear equations whose augmented matrix is 
$$\begin{bmatrix}
\ba_1 & \ba_2 & \cdots & \ba_n & b
\end{bmatrix}$$
#### $\rem$
### Existence of Solutions
#### $\rem$
#### $\ex$
#### $\defn$ – Span
A set of vectors $\{\bv_1,\bv_2,\dots, \bv_p\}$ in $\R^m$ *spans* (or *generates*) $\R^m$ if every vector is a linear combination of $\bv_1,\bv_2,\dots, \bv_p$. That is, $$\R^m=\Span\{\bv_1,\bv_2,\dots, \bv_p\}.$$
#### $\ex$
#### $\thm$
Let $A$ be an $m\times n$ matrix. Then the following statements are logically equivalent. That is, they are either all true, or all false. 
- For each $\bb$ in $\R^m$, the equation $A\bx =b$ has a solution. 
- Each $\bb$ is $\R^m$ is a linear combination of the columns of $A$.
- The columns of $A$ span $\R^m$.
- $A$ has a pivot in every row.
#### Warning
#### $\ex$
### Computation of $A\bx$
#### $\ex$
#### $\defn$ – Row-Vector Rule for Computing $A\bx$
If the product $A\bx$ is defined, then the $i$th entry in $A\bx$ is the sum of the products of the corresponding entries from row $i$ of $A$ and from the vector $\bx$.
#### $\ex$
### Properties of the Matrix-Vector Product $A\bx$
#### $\thm$
If $A$ is an $m\times n$ matrix, $\bu$ and $\bv$ are vectors in $\R^n$, and $c$ is a scalar, then:
- $A(\bu+\bv)=A\bu+A\bv$;
- $A(c\bu)=c(A\bu)$.
## Solution Sets of Linear Systems
### Solutions to Homogeneous Solutions
#### $\defn$ – Homogeneous
A system of linear equations is said to be *homogeneous* if its matrix equation can be written as $A\bx=\ov{0},$ where $A$ is an $m\times n$ matrix . 
#### $\ex$
#### $\rem$
#### $\ex$
#### $\ex$
#### $\rem$
### Solutions of Nonhomogeneous Solutions
#### $\ex$
#### $\rem$
#### $\thm$
Suppose the equation $A\bx=\bb$ is consistent for some given $\bb$, and let $\ov{p}$ be a solution; that is, $A\ov{p}=\bb$. Then the solution set of $A\bx=\bb$ is the set of vectors of the form $$\bw=\ov{p}+\bv_h,$$where $\bv_h$ is any solution of the homogeneous equation $A\bx=\ov{0}$. 
#### Warning
#### $\ex$
#### Algorithm
- Row reduce the augmented matrix to reduced echelon form.
- Express each basic variable in terms of any free variables.
- Write a typical solution $\bx$ as a vector whose entries depend on free variables, if applicable.
- Decompose $\bx$ into a linear combination of vectors (with numeric entries) using free variables as parameters.
## Applications of Linear Systems
### Economics
#### $\ex$
### Chemistry
#### $\ex$
### Network Flow
#### $\ex$
## Linear Independence
#### $\ex$
#### $\defn$ – Linearly In(Dependent)
A set of vectors $\{\bv_1,\bv_2,\dots, \bv_p\}$ in $\R^n$ is said to be *linearly independent* if the vector equation 
$$x_1\bv_1+x_2\bv_2+\cdots +x_p\bv_p=\ov{0}$$
has only the trivial solution; that is, only has the solution $x_1=x_2=\cdots =x_p=0$.

The set $\{\bv_1,\bv_2,\dots, \bv_p\}$ is *linearly dependent* if there exists scalars $c_1, \dots, c_p$ in $\R$, not all zero, so that 
$$c_1\bv_1+c_2\bv_2+\cdots +c_p\bv_p=\ov{0}.$$
#### $\ex$
#### $\ex$
#### $\ex$
#### $\rem$
#### $\ex$
### Sets of One or Two Vectors
#### $\thm$
Let $\bv$ be nonzero in $\R^n$. Then $\{\bv\}$ is linearly independent. 
#### $\thm$
Let $\bu$ and $\bv$ be in $\R^n$. Then $\{\bu,\bv\}$ is linearly dependent if and only if one of the two is a scalar multiple of one another. 
#### $\rem$
### Sets of Two or More Vectors
#### $\ex$
#### $\thm$
Let $S=\{\bv_1,\bv_2,\dots, \bv_p\}$, where $\bv_1,\bv_2,\dots, \bv_p$ are all vectors in $\R^n$. Then $S$ is linearly dependent if and only if some $\bv_j$ is a linear combination of the preceding vectors $\bv_1,\dots \bv_{j-1}$. That is, for some weights $c_1, \dots, c_{j-1}$, 
$$\bv_j=c_1\bv_1+\cdots +c_{j-1}\bv_{j-1}$$
#### $\rem$
#### $\thm$
If a set contains more vectors than entries in each vector, then the set is linearly dependent. That is, if the vectors in $\{\bv_1,\bv_2,\dots, \bv_p\}$ are all in $\R^n$, then these vectors are linearly dependent if $p>n$ .
#### $\thm$
If a set $\{\bv_1,\bv_2,\dots, \bv_p\}$ has vectors in $\R^n$ so that one of the vectors are the zero vector, then the set must be linearly dependent. 
#### $\ex$
#### $\ex$
## Introduction to Linear Transformations
#### $\ex$
#### $\ex$
#### $\defn$
A *transformation* (or *function* or *mapping*) $T$ from $\R^n$ to $\R^m$ is a rule that assigns each vector $\bx$ in $\R^n$ to a vector $T(\bx)$ in $\R^m$. 

$\R^n$ is the *domain* of $T$ and $\R^m$ is the *codomain*, and sometimes say $T:\R^n\to \R^m$ to indicate the domain is $\R^n$ and range is $\R^m$. 

For each $\bx$ in $\R^n$, we call $T(\bx)$ the *image* of $\bx$. The set of all images, that is, all possible $T(\bx)$ for any $\bx$, is the *range*. 
### Matrix Transformations
#### $\defn$
#### $\ex$
#### $\rem$
### Linear Transformations
#### $\ex$
#### $\defn$
#### $\thm$
#### $\rem$
#### $\ex$
#### $\rem$
#### $\ex$
#### $\ex$
#### $\ex$
## The Matrix of a Linear Transformation
#### $\defn$
#### $\ex$
#### $\ex$
#### $\thm$
#### $\rem$
#### $\rem$
#### $\defn$
#### $\ex$
#### $\ex$
#### $\rem$
### Existence Uniqueness Questions
#### $\defn$
#### $\ex$
#### $\ex$
#### $\thm$
#### $\ex$
#### $\thm$
#### $\rem$
#### $\ex$
#### $\rem$
#### $\ex$
# Matrix Algebra
## Matrix Operations
### Sums and Scalar Multiples
### Matrix Multiplication
### Powers and Transpositions of Matrices
## The Inverse of a Matrix
### Elementary Matrices
### Inverse Algorithm
## Characterizations of Invertible Matrices
### Invertible Linear Transformations
## Matrix Factorizations
### The LU Factorization
### An LU Factorization Algorithm
# Determinants
## Introduction to Determinants
## Properties of Determinants
### Column Operations
### Determinants and Matrix Products
# Vector Spaces
## Vector Spaces and Subspaces
### Subspaces
### Spanning Sets
## Null Spaces, Column Spaces, Linear Transformations
### The Null Space of a Matrix
### The Column Space of a Matrix
### Contrast between $\Nul A$ and $\Col A$
### Kernel and Image of Linear Transformations
## Linear Independence and Bases
### The Spanning Set Theorem
### Bases for $\Nul A$ and $\Col A$
## Coordinate Systems
### The Coordinate Mapping
## The Dimension of a Vector Space
### Subspaces of a Finite-Dimensional Space
### The Dimensions of $\Nul A$ and $\Col A$
## Rank
### Row Space
### The Rank Theorem
## Change of Basis
### Change of Basis in $\R^n$ 
# Eigenvalues & Eigenvectors
## Eigenvectors and Eigenvalues
## The Characteristic Polynomial
### Similarity
## Diagonalization
### Diagonalizing Matrices
## Eigenvectors and Linear Transformations
### Linear Transformations from $V$ to $V$
### Linear Transformations on $\R^n$
## Complex Eigenvalues
# Orthogonality
## Inner Product, Length, and Orthogonality
### Inner Product
### The Length of a Vector
### Distance in $\R^n$
### Orthogonal Vectors
### Orthogonal Complements
## Orthogonal Sets
### Orthogonal Projection
### Orthonormal Sets
## Orthogonal Projections
### Properties of Orthogonal Projections
## The Gram-Schmidt Process
## Least Squares Problems
# Symmetric Matrices
## Diagonalization of Symmetric Matrices
