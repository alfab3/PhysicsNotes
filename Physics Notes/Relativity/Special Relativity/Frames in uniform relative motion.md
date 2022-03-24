If we have a system:

![[relative frames.png]]

Where $k_1$ is moving with relative velocity $\vec w$ w.r.t. $k_0$

$\vec w$ "mixes" the $x$ and $t$ coordinates (and, analogously, $\vec x$ and $t$)

$$\begin{gather} L^\mu_\nu = \begin{bmatrix} L^0_0 & L^0_1 & 0 & 0 \\ L_0^1 & L_1^1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0  & 0 & 1\end{bmatrix} \end{gather}$$
Where we can determine: 

$$\begin{gather} \begin{cases} x'^0 = L_0^0 x^0 + L_1^0x^1 \\ x'^1 = L_0^1x^0 + L_1^1x^1\end{cases} & \begin{cases} x'^2 =L_2^2 x^2 = x^2 \\ x'^3 =x^3 \end{cases}\end{gather}$$

$$\begin{gather} \begin{cases} (L^0_0)^2-(L_0^1) = 1 \\ (L_1^0)^2 - (L_1^1)^2 = -1 \\ L_0^1 L_1^0 - L_0^1 L_1^1 = 0\end{cases} \end{gather}$$
Solutions: 

$$\begin{gather} L_0^0 = L_1^1 = \cosh \phi \\ L_0^1 = L_1^0 = -\sinh\phi\end{gather}$$
$$\begin{gather} x'^0 = \cosh \phi x^0-\sinh\phi x^1 \\ x'^1 = -\sinh\phi x^0 + \cosh\phi x^1\end{gather}$$
$$\begin{gather} \begin{bmatrix} x'^0 \\ x'^1 \end{bmatrix} = \begin{bmatrix} \cosh \phi & -\sinh \phi \\ -\sinh \phi & \cosh\phi
\end{bmatrix} \end{gather}$$

NOTE: boosts are hyperbolic rotations, i.e. a rotation by an imaginary angle

Condition from the transformation of the origin of $k_1$ 

$$\begin{gather}L w \begin{bmatrix} x^0 \\ wt\\0\\0\end{bmatrix} = \begin{bmatrix} x'^0 \\ 0 \\0\\0 \end{bmatrix}\end{gather}$$
$$\begin{gather} L^1_0x^0 + L_1^1 wt = L_0^1x^0 + L_1^1 \frac{x^0}{c}w =0 \\ L_0^1 = - \frac{w}{c}L^1_1 = -\beta L_1^1 \end{gather}$$

