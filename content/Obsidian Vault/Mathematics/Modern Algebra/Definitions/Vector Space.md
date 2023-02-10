#### $\defn$ – Vector Space
Let $F$ be a [[Field|field]]. An $F$-*vector space* is a (left) $F$-[[Module|module]].

More specifically, a *vector space* $V$ over a field $\F$ is a set $V$ together with operations of vector addition $+\colon V\times V \to V$ and scalar multiplication $\F\times V\to V$ (the latter of which we denote by simple concatenation; $x\v$ is the scalar multiple of $\v$ by $x$). These must satisfy the following conditions:
- Vector addition is commutative: for all $\v,\w\in V$ we have $\v+\w=\w+\v$
- Vector addition is associative: for all $\u,\v,\w\in V$ we have $\u+(\v+\w) = (\u+\v)+\w$
- There is a (vector) additive identity: there exists a special vector $\0\in V$ such that for all $\v\in V$ we have $\v+\0=\v$.
- There are (vector) additive inverses: for all $\v\in V$ there exists a vector $-\v$ such that $\v+(-\v)=\0$
- Scalar multiplication respects field addition: for all $x, y\in\F$ and $\v\in V$ we have $(x+y)\v=x\v+y\v$
- Scalar multiplication respects field multiplication: for all $x ,y\in \F$ and $\v\in V$ we have $(x y)\v=x(y\v)$
- Scalar multiplication respects the field identity: for all $\v\in V$ we have $1\v=\v$
- Scalar multiplication respects vector addition: for all $x\in \F$ and $\v,\w\in W$ we have $x(\v+\w) = x\v+x\w$.