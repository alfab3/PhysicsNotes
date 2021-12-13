## No Zero Modes
Let us start with problems of the type: 

$$\begin{gather} \mathcal L y(x) = f(x) \end{gather}$$

where $\mathcal L$ has no zero modes, such that the Fredholm Alternative ([[Nonhomogeneous problems]]) guarantees a single solution. Then $\mathcal L$ is invertible and we can formally write $y(x) = \mathcal{L}^{-1}f(x)$

The inverse operator $\mathcal L^{-1}$is called "Green's Function"

We look for a solution to the equation $$\begin{gather} \mathcal L_x G(x,\xi) = \delta(x-\xi) \end{gather}$$

Where $\mathcal L_x$ represents all derivatives wirth respect to $x$, $G(x,\xi) = \mathcal L^{-1}$, and $\delta(x-\xi)$ is the identity operator.


$$\begin{gather} y(x) = \int^b_a G(x,\xi)f(\xi)d\xi \end{gather}$$

Proof: $\mathcal L y(x) = \int^b_a \mathcal L_x G(x,\xi)f(\xi)d\xi = f(x)$