#### $\prop$ – When $G/\sim$ is a Group
For a [[Group|group]] $G$ and equivalence relation $\sim$, the rule $[x] \cdot [y] = [xy]$ is well-defined and makes $G/\sim$ into a group if and only if $\sim$ is [[Compatible with Addition & Multiplication|compatible with multiplication]]. 

###### *Proof.* 
The rule $[x] \cdot [y] = [xy]$ is well-defined if and only if whenever $[x]=[x']$ and $[y]=[y']$, then $[x][y]=[x'][y']$, i.e. $[xy]=[x'y']$ if and only if whenever $x\sim x'$ and $y\sim y'$, then $xy\sim x'y'$. 

Assume $\sim$ is compatible with multiplication. Then $x\sim x'$ implies $xy\sim x'y$ and $y\sim y'$ implies $x'y\sim x'y'$, hence by transitivity $xy\sim x'y'$. 

Conversely, assume the rule $[x] \cdot [y] = [xy]$ is well-defined. Setting $y=y'$ above gives whenever $x\sim x'$ then $xy\sim x'y$. Setting $x=x'$ above gives whenever $y\sim y'$ then $xy\sim xy'$. Hence $\sim$ is compatible with multiplication.

We need to prove that in either of these situations, $G/\sim$ really is a group. For $x,y,z$ we have $$[x] \cdot ([y] \cdot [z]) = [x] \cdot [yz] = [x(yz)] = [(xy)z] = [xy][z] = ([x][y])[z]$$since $G$ itself is a group. We have $[e_G] [x] = [x]$ for all $x$, so that $G/\sim$ has an identity. Finally,
$[x][x^{-1}] = [e_G] = e_{G/\sim}$, so that every element in $G/\sim$ has an inverse.
***