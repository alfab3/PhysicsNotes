An example of [[Partial Differential Equation]] is:

Laplace:
>$$\begin{gather} \nabla^2 \Phi = 0 \end{gather}$$

Poisson:
>$$\begin{gather} \nabla^2 \Phi = P(x) \end{gather}$$

Which are the same equation, but the Laplace is the homogeneous and Poisson is non-homogeneous.

The minimal non trivial configuration is in 2D, however we will use axial symmetry to format this in a 1D case: $\Phi(\vec x)$ where $\vec{x} \in R^3$.  Now we convert to $x \in r, \theta, \phi$

With a [[Curvilinear Coordinates]] system the Laplace equation becomes:

>$$\begin{gather} \nabla^2\Phi = \frac{1}{h_1h_2h_3}\left[\frac{\partial}{\partial x_1} \left(\frac{h_2h_3}{h_1}\frac{\partial}{\partial x_1}\Phi\right) + ...\right] \\ \nabla^2\Phi = \frac{1}{r^2}\frac{\partial}{\partial r}\left(r^2\frac{\partial \Phi}{\partial r}\right) + \frac{1}{r^2\sin\theta}\left[\frac{\partial} {\partial \theta}\left(\sin\theta\frac{\partial \Phi}{\partial \theta}\right) + \frac{1}{\sin\theta}\frac{\partial^2 \Phi}{\partial\phi^2}\right] = 0 \\ =\frac{1}{r}\frac{\partial}{\partial r} (r\frac{\partial \Phi}{\partial r} - \frac{1}{r^2} \hat{L}^2\Phi = 0 \\ \hat{L}^2 = -\frac{1}{\sin\theta}\frac{\partial}{\partial \theta}\left(\sin\theta\frac{\partial}{\partial \theta}\right) - \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial \phi^2}\end{gather}$$

Solution of the form:

>$$\begin{gather} \Phi(r,\theta,\phi) = \sum_{l,m} a_{lm}(r) Y^m_l(\theta, \phi) \end{gather}$$

Where $Y^m_l(\theta, \phi)$ are the spherical harmonics.

$Y_{lm}(\theta,\phi)$ are [[Eigenfunctions]] of $\hat{L}^2$:

>$$\begin{gather} \hat{L}^2 Y_{lm}(\theta,\phi) = l(l+1)Y_{lm}(\theta,\phi) \end{gather}$$

>$$\begin{gather} \frac{1}{r}\frac{\partial}{\partial r}\left(r\frac{\partial a_{lm}(r)}{\partial r}\right) Y_{lm}(\theta,\phi) - \frac{1}{r^2}l(l+1a_{lm}(r) Y_{lm}(\theta,\phi)=0 \\\frac{1}{r}\frac{\partial}{\partial r}\left(r\frac{\partial a_{lm}(r)}{\partial r}\right) - \frac{1}{r^2}l(l+1)a_{lm}(r) =0
\\ a_{lm}(r) = \alpha_{lm}r^l + \beta_{lm}r^{-(l+1)}\end{gather}$$

Substitute back in to prove(maybe? Benny didn't work it out properly)

General Solution to Laplace: 
$$\begin{gather}\Phi(r,\theta,\phi) = \sum_{l,m}[\alpha_{lm}r^l + \beta_{lm}r^{-(l+1)}] Y_{l,m}(\theta, \phi)\end{gather}$$

Spherically symmetric: 

$$\begin{gather}\Phi(r) = \alpha + \beta r^{-1} \end{gather}$$