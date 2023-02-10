### Problem 5 – Showing Module is Torsion-Free
Recall that a $\Z$-[[Module|module]] $M$ is called *torsion-free* if its torsion submodule is $\Tor(M ) =\{0\},$ where $\Tor(M ) = \{m \in M | rm = 0 \text{ for some }r \in \Z\setminus\{0\}\}.$
Consider the $\Z$-module
$$M= \frac{\Z \oplus \Z}{\langle(7, 11)\rangle }\text{ where }\langle(7, 11)\rangle = \{(7k, 11k) | k \in \Z\}.$$
Show that $M$ is torsion free.

##### *Proof.*
Let $m=(a,b)\in\Tor(M)$. Thus $rm=0$ for some nonzero $r\in\Z$. Then $(ra,rb)=0$, and so $ra=0$ and $rb=0$. Then there exists $p,q\in\Z$ such that $7p=ra$ and $7q=rb$  or $11p=ra$ and and $11q=rb$. Notice that in $M$ we have $7,11=0$, and thus neither $7$ nor $11$ can divide $r$. 
Suppose $7p=ra$ and $7q=rb$. As $7$ cannot divide $r$ we see that $7$ divides both $a$ and $b$, placing them both $\langle(7, 11)\rangle$. Thus $m=0$. The same holds true if we use $11$. Thus $m=0$ and $\Tor(M)=\{0\}$. 

#qual