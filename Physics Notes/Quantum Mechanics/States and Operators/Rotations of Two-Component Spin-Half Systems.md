As an example of a [[Unitary Transformations]] we consider rotations in a two-component system. 

For spin-1/2 systems the [[Spin]] operator is: 

$$\begin{gather} \vec S = \frac{\hbar}{2}\vec \sigma \end{gather}$$

Where $\vec \sigma$ represents the Pauli vector, which is a linear combination of the [[Pauli Spin Matrices]] and unity. 

For a [[Unit Vector]] $\hat n$: 

$$\begin{gather} (\vec \sigma\cdot \hat n)^2= \mathbb I \end{gather}$$

For a state with spin-up or spin down along the z-axis, we choose the basis:

$$\begin{gather} \ket{\uparrow} = \begin{bmatrix} 1 \\ 0 \end{bmatrix},\;\; \ket{\downarrow} = \begin{bmatrix} 0 \\ 1 \end{bmatrix} \end{gather}$$

Rotations by an angle $\theta$ are given by $$\begin{gather} \mathcal R(\vec \theta) = e^{i\vec \theta \cdot \vec \sigma/2} \end{gather}$$ where the direction of $\vec \theta$ is along the axis of rotation $\hat n$ so: $\vec \theta = \theta \hat n$ 

Performing a [[Taylor Series]]: 

$$\begin{gather} e^{-i\theta\vec \sigma \cdot \hat n/2} = \cos(\theta/2) - i\sin(\theta/2)\vec\sigma\cdot\hat n \end{gather}$$

For normal vectors the rotation matrix in 2D becomes: 

$$\begin{gather} \mathcal R(\phi) = \begin{bmatrix} \cos\phi & - \sin\phi \\ \sin\phi & \cos\phi\end{bmatrix} = e^{-i\phi\sigma_y} = cos\phi - i\sigma_y \sin\phi\end{gather}$$