#### $\lem$ – Matrix Multiplication is Associative
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]], let $F, E, G$ be [[Basis and Free Module|free]] $R$-[[Module|modules]] having finite [[Basis and Free Module|bases]] $X = \{x_1, \dots, x_m\}, Y = \{y_1, \dots, y_n\}, Z = \{z_1, \dots, z_p\}$ of  size $m,n,p$, respectively. Given a $n \times m$ matrix $A$ and a $p \times n$ matrix $B$, let $AB$ denote the $p \times m$ matrix obtained by the usual formula for matrix multiplication, and let $T_A^{X,Y}: F \to E$, $T_B^{Y,Z}: E \to G$ and $T_{BA}^{X,Z}: F \to G$ be the maps associated to these matrices relative to the specified bases, as given in Proposition \ref{prop127} #fix .
Then $$T^{Y,Z}_B \circ T_A^{X,Y} = T_{BA}^{X,Z}.$$
In particular, matrix multiplication is associative.
###### *Proof.* 
For the first assertion we just need to check the two maps agree on $x_j$ for all $j$:
  We have
  $$
T_B(T_A(x_j)) = T_B(\sum_i a_{i,j} y_i) = \sum_i a_{i,j} T_B(y_i) 
= \sum_i \sum _l a_{i, j} b_{k, i} z_k
$$
(with the second equation using that $T_B$ is an $R$-map)
and
$$
T_{BA}(x_j) = \sum_k (BA)_{k,j} z_k = \sum_k \left(\sum _i b_{k, i} a_{i, j}\right) z_k.
$$
(I have left off the superscripts $(X,Y)$ etc. for the sake of  my sanity.) 
These two expressions agree since $R$ is commutative. 

The second assertion holds since composition of functions is associative.
***