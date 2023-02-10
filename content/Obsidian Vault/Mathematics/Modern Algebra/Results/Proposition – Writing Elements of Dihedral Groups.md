#### $\prop$ – Writing Elements of $D_{2n}$
Every element in $D_{2n}$[^1] can be written as $r^j$ or  $r^js$ for $0 \leq j \leq n-1$. Moreover, no two of these expressions are the same element, and thus $D_{2n}$ has exactly $2n$ elements.

###### *Proof.* 
We will use some geometric notions freely without complete justification. For example, we use that if an isometry of $\R^2$ fixes two points $A$ and $B$, then it is either the identity element or it is reflection about the line $AB$. We  also use that every element of $D_{2n}$ maps the origin to itself (since the origin is the center of mass of $P_n$). Finally, we use that every isometry of $\R^2$ is either *orientation preserving* or *orientation reversing.

Label the vertices of $P_n$ as $V_0, \dots, V_{n-1}$, with $V_0$ being the vertex located on the positive $s$-axis, $V_1$ being the vertex adjacent to $V_0$ in the counter-clockwise direction, etc. We have  $r(V_0) = V_1$, $r(V_1) = V_2$, etc., and so  $r^j(V_0) = V_{j \pmod{n}}$. Moreover any isometry must send a vertex to a vertex because the vertices are the points on $P_n$ at largest distance from the origin.

Let $\a$ be an arbitrary symmetry of $P_n$. Then $\a(V_0) =V_ j$ for some $0 \leq j \leq n-1$. Then the element $r^{-j}\a$ fixes  $V_0$ and the origin, and hence either $r^{-j}\a = e$ or $r^{-j}\a = s$ from the discussion above. We get that $\a = r^j$ or $\a = r^js$, proving the first assertion.

Since $r^j(V_0) = V_{j \pmod{n}}$, we see that if $r^j = r^i$ for $0 \leq i,j \leq n-1$, then $i=j$. We have $r^js \ne r^i$ for any $i,j$ since the former is orientation reversing and the latter is orientation preserving. If $r^is = r^js$ for $0 \leq i,j \leq n-1$, then upon multiplying on the left of $s^{-1}$ we get $i=j$.
***

[^1]: See: [[Dihedral Group]]