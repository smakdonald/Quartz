#### $\prop$ – Isomorphism iff Bijective Homomorphism
Suppose $f: G \to H$ is a [[Group|group]] [[Homomorphism|homomorphism]]. Then $f$ an [[Isomorphism|isomorphism]] if and only if $f$ is bijective (one-to-one and onto).

###### *Proof.* 
$(\Rightarrow)$ Recall that a function $f: X \to Y$ between two sets is bijective if and only if there is a function $g: Y \to X$ such that $f \circ g = \id_Y$ and $g \circ f = \id_X$. Thus an isomorphism is indeed a bijection. 

$(\Leftarrow)$ If $f$ is bijective homomorphism, then it certainly has a *set-theoretic* two-sided inverse $g$. But we need to show $g$ is actually a homomorphism: for $x,y \in H$ we have $$f(g(xy)) = xy = f(g(x))f(g(y)) =f(g(x)g(y)).$$Since $f$ is one-to-one, $g(xy) = g(x)g(y)$.
***