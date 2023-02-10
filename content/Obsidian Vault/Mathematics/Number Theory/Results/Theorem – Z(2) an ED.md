#### $\thm$ – Z(2) an ED
The function |N | defined by 
|N (a + b√2)| = |a^{2} - 2b^{2}| 
is a Euclidean norm, so Z[√2] is a Euclidean Domain and hence a UFD.

##### *Proof.*
We proceed as in the other cases. First, note that the norm |N | is multiplicative, 
so if \a | \beta, then |N (\a )| | |N (\beta )| and thus |N (\a )| \leq |N (\beta )|. Now we need to consider 
division. Let \a = a + b√2 and \beta = c + d√2, so 
\a 
\beta = a + b√2 
c + d√2 \cdot c - d√2 
c - d√2 = ac - 2bd 
c^{2} - 2d2 + bc - ad 
c^{2} - 2d2 
√2. 
Like any real number, both ac - 2bd 
c^{2} - 2d2 and bc - ad 
c^{2} - 2d2 are within 1 
2 of an integer, say 
r and s, respectively. Let \g = r + s√2, and let \rho = \a - \beta \g. Then 
\rho 
\beta = \a 
\beta - \g = 
( ac - 2bd 
c^{2} - 2d2 - r 
) 
+ 
( bc - ad 
c^{2} - 2d2 - s 
) √2. 
Therefore, by the triangle inequality, 
∣ 
∣ 
∣ 
∣N 
( \rho 
\beta 
)∣ 
∣ 
∣ 
∣ = 
∣ 
∣ 
∣ 
∣ 
∣ 
( ac - 2bd 
c^{2} - 2d2 - r 
)2 
- 2 
( bc - ad 
c^{2} - 2d2 - s 
)2∣ 
∣ 
∣ 
∣ 
∣ \leq 1 
4 + 2 \cdot 1 
4 < 1. 
Thus |N (\rho )| < |N (\beta )|, as desired.