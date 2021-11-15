# Green's Functions

## Fourier Transform

Transform
>$$\begin{gather} f(x) = \int^\infty_{-\infty} \frac{dk}{2\pi} g(k)e^{ikx}  \end{gather}$$

Inverse Transform
>$$\begin{align} g(k) = \int^\infty_{-\infty} f(x)e^{-ikx}dx \end{align}$$

## Solving for Green's Functions
#### Example 1: Helmholtz problem
Fourier transform is given by:

$$\begin{gather} \tilde h(k,y) = \tilde h(k,0) e^{-\sqrt{k^2+l_c^2}|y|} \end{gather}$$