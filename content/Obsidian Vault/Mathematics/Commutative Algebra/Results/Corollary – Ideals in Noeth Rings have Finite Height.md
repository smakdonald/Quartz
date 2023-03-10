#### $\cor$ – Ideals in Noeth Rings have Finite Height
If $R$ is a [[Noetherian Ring|noetherian ring]], then any ideal has finite [[Height of an Ideal|height]]. If $(R,\m,k)$ is also [[Local Ring|local]], then $\dim(R) \leqslant \dim_k(\m/\m^2) <\infty$[^1].

##### *Proof.*
If $R$ is noetherian, then every ideal is finitely generated, by \Cref{noetherian fg}, and thus by \hyperref[Krull height theorem]{Krull's height theorem} every ideal has finite height.

Now suppose that $(R,\m,k)$ is a noetherian local ring. By \hyperref[NAK4]{NAK}, $\m$ is generated by $\dim_k(\m/\m^2)$ elements, so $$\dim(R) = \height(m) \leqslant \dim_k(\m/\m^2).$$

[^1]: Notation: [[Krull Dimension of a Ring]]