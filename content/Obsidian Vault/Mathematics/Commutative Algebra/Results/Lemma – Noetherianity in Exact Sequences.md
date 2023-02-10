#### $\lem$ – Noetherianity in Exact Sequences
In an [[Exact Sequence|exact sequence]] of modules $$\begin{CD}
0@>>>A@>f>>B@>g>>C@>>>0
\end{CD}$$$B$ is [[Noetherian Module|noetherian]] if and only if $A$ and $C$ are noetherian. 

##### *Proof.*
Assume $B$ is noetherian. Since $A$ is a submodule of $B$, and its submodules are also submodules of $B$, $A$ is noetherian. Moreover, any submodule of $B/A$ is of the form $D/A$ for some submodule $D \supseteq A$ of $B$. Since every submodule of $B$ is finitely generated, every submodule of $C$ is also finitely generated. Therefore, $C$ is noetherian.

Conversely, assume that $A$ and $C$ are noetherian, and let
$$M_1 \subseteq M_2 \subseteq M_3 \subseteq \cdots$$
be a chain of submodules of $B$. First, note that
$$M_1 \cap A \subseteq M_2 \cap A \subseteq \cdots$$
is an ascending chain of submodules of $A$, and thus it stabilizes. Moreover,
$$g(M_1) \subseteq g(M_2) \subseteq g(M_3) \subseteq \cdots$$
is a chain of submodules of $C$, and thus it also stabilizes. Pick a large enough index $n$ such that both of these chains stabilize. We claim that $M_n = M_{n+1}$, so that the original chain stabilizes as well. To show that, take $x \in M_{n+1}$. Then 
$$g(x) \in g(M_{n+1}) = g(M_n)$$
so we can choose some $y \in M_n$ such that $g(x) = g(y)$. Then $x-y \in \ker g = \im f = A$. Now note that $y \in M_n \subseteq M_{n+1}$, so $x-y \in M_{n+1}$, and thus 
$$x-y \in M_{n+1} \cap A = M_n \cap A.$$
Then $x-y \in M_n$, and since $y \in M_n$, we must have $x \in M_n$ as well.