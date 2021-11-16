## 3.5) Fourier Transform

Transform
>$$\begin{gather} f(x) = \int^\infty_{-\infty} \frac{dk}{2\pi} g(k)e^{ikx}  \end{gather}$$

Inverse Transform
>$$\begin{align} g(k) = \int^\infty_{-\infty} f(x)e^{-ikx}dx \end{align}$$

### Convolution

A mathematical operation on two functions that produce a third function:

>$$\begin{gather} f \circ g = \int^\infty_{-\infty} d\xi f(x-\xi)g(\xi)\end{gather}$$