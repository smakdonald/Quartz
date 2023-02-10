#### $\prop$ – Finding Unique Equivalent Matrix
Let $R$ be a non-zero [[Commutative Ring|commutative]] [[Ring|ring]], let $V$ be a [[Basis and Free Module|free]] $R$-[[Module|module]] of [[Dim (Vector Space)|dimension]] $n$, and let $B = \{b_1, \dots, b_n\}$ be any ordered [[Basis and Free Module|basis]] of $V$. If $P$ is any $n \times n$ matrix with entries in $R$ that is invertible (i.e., there is another $n \times n$ matrix $P^{-1}$ such that $PP^{-1} = I_n = P^{-1}P$), then $P = [\id_V]_B^C$[^1] for a unique basis $C$ of $V$.
  
###### *Proof.* 
Each of the maps$$
  V \xra{v \mapsto [v]^B} R^n \xra{w \mapsto P^{-1} \cdot w} R^n \xra{(r_1, \dots, r_n)^\tau \mapsto \sum_i r_i b_i} V
  $$
is an isomorphism. (The one on the far right is the inverse of the one on the far left. The middle one is since $u \mapsto P \cdot u$ is a two-sided inverse.) So the composition of all three of these maps, let us call it $g$, is also an isomorphism. It follows that $C = \{g(b_1), \dots, g(b_n)\}$ is a basis of $V$.
I leave it as an exercise for you to check that $P = [\id_V]_B^C$.

To show  the uniqueness, say $C = \{c_1, \dots, c_n\}$, say $C' = \{c'_1, \dots, c'_n\}$ are ordered bases such that $[\id_V]_B^{C'} = P = [\id_V]_B^C$. Then $$
  [\id_V]_C^{C'} = [\id_V]_B^{C'} [\id_V]_C^B =  [\id_V]_B^{C'}  \left( [\id_V]_B^{C} \right)^{-1} = PP^{-1}  = I_n.
  $$
For each $i$ we have$$
 [c_i]^C  =  (0, \dots, 0, 1, 0, \dots, 0)^\tau 
 $$
and$$
 [c_i]^C  =  I_n [c_i]^C =  [\id_V]_C^{C'} [c_i]^C =  [c_i]^{C'}
$$so that$$
[c_i]^{C'} =  (0, \dots, 0, 1, 0, \dots, 0)^\tau
$$which gives $c_i = c_i'$.  
***

[^1]: See: [[Homomorphism Matrix]]