## 1.2) Laurent Series
If $f(z)$ is analytic throughout the region there exists a series expansion in terms of positive and negative powers of (z - a) (where a is the center of the region)

>$$\begin{align} f(z) = \sum_{k=0}^\infty a_k(z-a)^k + \sum^\infty_{k=1}b_k(z-a)^{-k} \end{align}$$

where 
>$$\begin{gather} a_k = \frac{1}{2\pi i}\oint_{K_1} \frac{f(\zeta) d\zeta}{(\zeta - a)^{k+1}} \\ b_k = \frac{1}{2\pi i}\oint_{K_2}(\zeta - a)^{k-1}f(\zeta)d \zeta\end{gather}$$

### 1.2.1) L'Hopital's Rule
In the case where we find a derivative (or more specifically a limit) to give us: $\frac{0}{0}$ we utilize L'Hopital's Rule
>$$\begin{align} \lim_{x \to c} \frac{f(x)}{g(x)} =  \lim_{x \to c} \frac{f'(x)}{g'(x)}\end{align}$$