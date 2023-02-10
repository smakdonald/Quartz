#### $\lem$ – Noetherian Rings
Suppose $R$ is a [[Commutative Ring|commutative]] [[Ring|ring]]. The following conditions are equivalent:
1. $R$ has the [[Ascending Chain Condition|ascending chain condition]] on [[Ideal|ideals]].
2. Every ideal of $R$ is finitely generated --- i.e., for every ideal $I$, there exists a finite set of elements $x_1, \dots, x_n$ in $I$ such that $I = R \cdot x_1 +   \cdots + R \cdot x_n$. 
In this case we say $R$ is *Noetherian*. 

###### *Proof.* 
Assume every ideal is finitely generated and that such a chain is given. Let $J = \cup_n I_n$. Then it is easy to see that $J$ is an ideal. (In detail,  for $a \in J, r \in R$ we have $a \in I_n$ for some $n$ and hence $ra \in I_n \subseteq J$.

If $a,b \in J$, then $a \in I_n$ and $b \in I_m$ for some $n,m$ and hence there is a $N$ such that $a,b \in I_N$. It follows that $a \pm b \in I_N \subseteq J$. Finally $0 \in J$.) Thus by assumption $J$ is finitely generated, say $J = Rx_1 + \cdots +  Rx_m$ for some $x_1, \dots, x_m \in J$.

Each $x_i$ belongs to one of the $I_n$'s and hence, since there are only a finite number of such elements and ideas are nested, there is an $N$ such that $x_1, \dots, x_m \in I_N$. It follows that $I_N = J$
and hence  $I_N = I_{N+1} = I_{N+2} = \cdots$.

Assume $R$ has the acc for ideals and let $J$ be any ideal. Pick any element $a_1\in I$ and set $I_1 = Ra_1$.  If $J = I_1$ we are done. If not, pick $a_2 \in I \setminus I_1$ and set $I_2 =  Ra_1 + Ra_2$. If $J = I_2$  we are done and if not pick $a_3 \in I\setminus I_2$ and let $I_3 = Ra_1 +  Ra_2 + Ra_3$. In this way we form a strictly ascending chain $I_1 \subset I_2 \subset I_3 \subset$, and this process cannot be continued forever since $R$ has the acc. When it terminates, we have $J = Ra_1 + Ra_2 + \cdots + Ra_N$ for some $a_1, \dots, a_N$ and thus $J$ is finitely generated.
***