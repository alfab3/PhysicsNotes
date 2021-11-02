The Fourier integral can be viewed as a linear operator $\mathcal{F}$ that transform one vector $\ket{f} \equiv \{f(\vec x\}$ into $\ket{g} = \{g(\vec k)\}$ that is:

$$\begin{align} \ket{g} = \mathcal{F}\ket{f} \end{align}$$

Where $$\begin{align} g(\vec k) = \frac{1}{2\pi}\int e^{i\vec k \vec x} f(\vec x) \ d\vec x \end{align}$$

## Adjoint
$$\begin{align} \mathcal{F}^\dagger\ket{f_1} = \int d \vec k e^{-i\vec k \vec x} f_1(\vec k) \end{align}$$ is a [[Unitary]] operator (not self-adjoint)

$\mathcal{F}^\dagger$ is the inverse Fourier. 

Up to a normalization factor $\mathcal{F}^\dagger\mathcal{F}$ is the identity operator.