#### $\lem$ – Quotient Noetherian
Let $R$ be a ring and $I$ an ideal in $R$. If $R$ is [[Noetherian Ring|noetherian]], then so is $R/I$.

##### *Proof.*
There is an order preserving bijection
$$\{ \text{ideals of } R \text{ that contain } I \} \longleftrightarrow \{\text{ideals of }R/I\}$$
that sends the ideal $J \supseteq I$ to $J/I$; its inverse is the map that sends each ideal in $R/I$ to its preimage.
Given this bijection, chains of ideals in $R/I$ come from chains of ideals in $R$ that contain $J$. This implies that if $R$ is noetherian, then $R/I$ is noetherian as well.