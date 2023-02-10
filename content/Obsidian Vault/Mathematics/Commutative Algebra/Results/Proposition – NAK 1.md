#### $\prop$ – NAK 1
Let $R$ be a ring, $I$ an ideal, and $M$ a finitely generated $R$-module. If $IM = M$, then:
(a) there is an element $r\in 1 + I$ such that $rM=0$, and
(b) there is an element $a\in I$ such that $am=m$ for all $m\in M$.

##### *Proof.*
Let $M = R m_1 + \cdots + R m_s$. By assumption, we have equations \[ m_1 = a_{11} m_1 + \cdots + a_{1s} m_s \ , \ \dots \ , \ m_s = a_{s1} m_1 + \cdots + a_{ss} m_s,\] with $a_{ij}\in I$. Setting $A=[a_{ij}]$ and $v=[m_i]$, we have a matrix equation $Av=v$. By~the \hyperref[determinantal trick]{Determinantal trick}, the element $\det(I_{s \times s} - A) \in R$ kills each $m_i$, and hence it kills $M$. Since $\det(I_{s \times s}-A)\equiv \det(I_{s \times s})  \equiv 1 (\!\pmod I)$, this determinant is the element $r$ we seek for the first statement.For the latter statement, set $a=1-r$, which is in $I$ and satisfies $am=m-rm=m$ for all $m\in M$.