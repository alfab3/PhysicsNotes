The basic differential laws of magnetostatics are 
$$\begin{gather} \nabla \times \mathbf B = \mu_0\mathbf J \\ \nabla \cdot \mathbf B = 0 \end{gather}$$

The problem is how to solve them. If the current density  is zero in the region of interest, $\nabla \times \mathbf B = 0$ permits the expression of the vector magnetic induction $\mathbf B$ as the gradient of a [[Magnetic Scalar Potential]], 

$$\begin{gather} \mathbf B = -\nabla \Phi_M\end{gather}$$

Then the differential forms reduce to the Laplace equation for $\Phi_M$ and techniques of solving electrostatics problems may be used. (However boundary conditions are treated differently)

A general method of attack is to exploit the equation $\nabla \cdot \mathbf B = 0$. If this is true everywhere, $\mathbf B$ must be the curl of some vector field $\mathbf A (\mathbf x)$ called the vector potential: 

$$\begin{gather} \mathbf B(\mathbf x) = \nabla \times \mathbf A(\mathbf x) \end{gather}$$

The general form of $\mathbf A$ is 
$$\begin{gather} \mathbf A = \frac{\mu_0}{4\pi}\int\frac{\mathbf J (\mathbf x')}{|\mathbf x - \mathbf x'|}d^3x' + \nabla \mathbf\Psi (\mathbf x) \end{gather}$$
the added gradient of an arbitrary scalar function $\Psi$ shows that for a given [[Magnetic Induction]] $\mathbf B$, the vector potential can be freely transformed according to: 

$$\begin{gather} \mathbf A \to \mathbf A + \nabla\Psi \end{gather}$$