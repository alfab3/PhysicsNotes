The scalar potential ([[Electric Potential]]) has a physical interpretation when we consider the work done on a test charge $q$ in transporting it from one point, $A$, to another point $B$ in the presence of an [[Electric Field]] $\mathbf E(\mathbf x)$. The force acting on the charge at any point is: 

$$\begin{gather} \mathbf F = q \mathbf E \end{gather}$$

so that the work done in mocing the [[Electric Charge]] from $A$ to $B$ is 
$$\begin{gather} W = -\int^B_A \mathbf F \cdot dl = -q\int^B_A \mathbf E \cdot dl \end{gather}$$

The minus sign appears because we are calculating the work done on the charge against the action of the field. Equating to [[Electric Potential]] the work can be written as: 

$$\begin{gather} W = q \int^B_A \nabla \Phi \cdot dl = q \int^B_A d\Phi = q(\Phi_B -\Phi_A) \end{gather}$$ 
which shows that $q\Phi$ can be interpreted as the [[Potential Energy]] of the [[Test Charge]] in the electrostatic field.

It can be seen that the line integral of the electric field between two points is independent of the path and is the negative of the potential difference between the points:

$$\begin{gather} \int^B_A \mathbf E \cdot dl = -(\Phi_B - \Phi_A) \end{gather}$$

This follows directly of course from the definition $E = -\nabla \Phi$. If the path is closed, the line integral is zero: 

$$\begin{gather} \oint E \cdot dl = 0 \end{gather}$$

a result that can also be obtained directly from [[Coulomb's Law (electrostatics)]]. The application of Stokes's theorem if $\mathbf A(\mathbf x)$ is a well behaved vector field, $S$ is an arbitrary open surface, and $C$ is the closed curve bounding $S$, $$\begin{gather} \oint_C \mathbf A \cdot d\mathbf l = \int_S(\nabla \times \mathbf A)\cdot \mathbf n da \end{gather}$$

where $d\mathbf l$ is a line element of $C$, $\mathbf n$ is normal to $S$, and the path $C$ is traversed in a right-hand screw sense relative to $\mathbf n$ leads immediately back to $\nabla \times \mathbf E = 0$. 

