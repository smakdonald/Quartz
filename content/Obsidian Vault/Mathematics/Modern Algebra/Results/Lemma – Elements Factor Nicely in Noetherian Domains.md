#### $\lem$ – Elements Factor Nicely in Noetherian Domains
If $R$ is a [[Noetherian Ring|noetherian]][[Integral Domain|integral domain]], then every non-zero, not-[[Unit|unit]] element factors into a finite product of [[Mathematics/Modern Algebra/Definitions/Prime|irreducible]] elements.

###### *Proof.* 
Pick $x \in R$ with $x \ne 0$ and $x \notin R^\times$. If $x$ is irreducible, there is nothing to prove. Otherwise, we have $x = x_1 x_2$ for
  non-units $x_1, x_2$. If both $x_1, x_2$ are irreducible, the proof is complete. Otherwise, one or both of them factors non-trivially. We may express
 this  conveniently by
  saying that $x_1 = x_3x_4$
  and $x_2 = x_5x_6$ such that either $x_3$ and $x_4$ are both non-units or $x_5$ and $x_6$ are both non-units. (E.g., if $x_2$ is irreducible, we could set
  $x_5 = x_2, x_6 = 1$.) Continuing in the this manner, we form a binary tree with $x$ at the top, $x_1, x_2$ one level down, $x_3,x_4,x_5,x_6$ one level below
  that, etc.
We halt the process of building the tree if at some stage all the leaves of the tree are irreducbile elements,
  at which point we will have proven that $x$ factors in to a product of the irreducible elements given by these leaves.

We need to rule out the possibility that the process never
terminates. If it never terminates, we will have built an infinite
binary tree with the property that some route downward through the tree consists of an infinite list of
of irreducible elements $y_1, y_2, y_3,\dots$ such that $x = y_1z_1$ for a non-unit $z_1$  and, for each $i \geq 1$, $y_{i} = y_{i+1}
z_{i+1}$ for a non-unit $z_{i+1}$. Since $R$ is an integral domain, we have $(x) \subsetneq (y_1)$ and $(y_i) \subsetneq (y_{i+1})$ for all $i \geq 1$. (E.g., if
$(x) = (y_1)$ then $y_1 = xv$ and hence $x = xvz_1$, so that $vz_1 = 1$, contrary to $z_1$ being a non-unit.)
But then we have arrived at an infinite ascending chain of ideals in $R$,
$$
(x) \subsetneq (y_1) \subsetneq (y_2) \subsetneq (y_3) \subsetneq \cdots,
$$
which is not possible in a Noetherian ring.
***