Find the path followed by a light ray if the index of refraction is proportional to $r^{-2}$. We want to make stationary
$$\begin{align} \int nds \;\; \text{or} \;\; \int r^{-2}ds =\int r^{-2}\sqrt{dr^2+r^2d\theta^2} = \int r^{-2} \sqrt{1+r^2 \theta'^2}dr\end{align}$$

The Euler equation is with $F = r^{-2}\sqrt{1+r^2\theta'^2}$. Since $\partial F/\partial \theta = 0$ we have
$$\begin{align} \frac{d}{dr}\left(\frac{r^{-2}r^2\theta'^2}{\sqrt{1+r^2\theta'^2}}\right) \end{align}$$

or

$$\begin{align} \frac{\theta'}{\sqrt{1+r^2\theta^2}} = \text{const.} = K. \end{align}$$

Solve for $\theta'$ and integrate ([[Integral]])

$$\begin{align} \theta'^2 = K^2(1+r^2\theta'^2)\end{align}$$

so 

$$\begin{align} \theta'^2(1-K^2r^2) = K^2\\\theta'=\frac{d\theta}{dr}=\frac{K}{\sqrt{1-K^2r^2}}\\ \theta=\arcsin Kr+\text{const.}\end{align}$$ 