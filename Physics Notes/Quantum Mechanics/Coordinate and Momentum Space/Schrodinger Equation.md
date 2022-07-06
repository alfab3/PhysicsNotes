# Definition
$$\begin{gather} i\hbar\frac{\partial}{\partial t} \psi(x) = - \frac{\hbar}{2m}\frac{\partial^2}{\partial x^2} \psi(x)+V(x)\psi(x) \end{gather}$$
Rather than thinking of $\psi(x)$ as a [[Wave function]], it is more reveling to recognize it as overlap of the state $\ket{\psi}$ with state $\ket{x}$.

$$\begin{gather} \psi(x) = \braket{x|\psi} \end{gather}$$
The only difference between a label in [[Coordinate Space]] and a label that denotes a discrete variable such as spin, is that because the $x$ label is continuous, the normalization has to be changed. 

$$\begin{gather} \braket{x'|x}=\delta(x-x') \end{gather}$$
This implies that $\ket{x}$ has dimensions of inverse length to the one-half power. The completeness relation becomes

$$\begin{gather} \int dx \ket{x}\bra{x} = \mathbb{I} \\ \int dx \braket{\phi|x}\braket{x|\psi} = \braket{\phi|\psi} \end{gather}$$
