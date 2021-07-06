For an illustration of linear dependnece consider the solution of the [[Ordinary Differential Equation]]
$$\begin{align} \frac{d^2 \phi(x)}{dx^2}= \phi(x)\end{align} $$

This equation has solutions $\phi_1 = e^x$ and $\phi_2 = e^{-x}$, and we add \phi_3 = \cosh x, also a solution. The Wronskian is $$\begin{align} \begin{bmatrix} e^x & e^{-x} & \cosh x \\ e^x & -e^{-x} & \sinh x \\ e^x & e^{-x} & \cosh x\end{bmatrix} \end{align}$$
The determinant vanishes for all $x$ because the first and third rows are identical. Hence $e^x$, $e^{-x}$, and $\cosh x$ are linearly dependent and indeed we have a relation of the form of:

$$\begin{align} e^x+e^{-x} - 2 \cosh x = 0 \end{align}$$