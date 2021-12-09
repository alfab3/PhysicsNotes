### Vacuum

[[Point Charge]]s may exist and generate an [[Electric Field]]. That is, volumetric charge density (charge/volume) $\rho$ may be non-zero and correspondingly $\phi(\vec x)$ determined by 

$$\begin{gather} \nabla^2 \phi(\vec x)= \frac{\rho(\vec x)}{\epsilon_0} \end{gather}$$

may be non-zero.
### Conductors

Net charge may not exist inside a conductor, and there is no [[Electric Field]].  Any changes may exist only at the boundaries of a conducting body. 


$$\begin{gather} \vec E = 0 \\ \vec E = \vec \nabla \phi \Rightarrow\phi = \text{const}\end{gather}$$

$\sigma(\vec x)$ (charge/area) may be non-zero for $\vec x \in$ the surface of the conductor.

Let us consider now the vicinity of a conductor-vacuum boundary:

![[conductor and vacuum space.png]]

Generally, we expect the field $\vec E( \vec x)$ to be continuous (more precisely: $|\rho(\vec x)| < \infty \Rightarrow \vec E(\vec x)$)

However since the surface of the conductor may have a surface charge $\sigma(\vec x) \neq 0$ ($\Rightarrow |\rho(\vec x)| = \infty$) we expect the [[Electric Field]] to exhibit some discontinuity. To characterize it we construct a "Gauss surface" depicted above around a surface point $\vec x$ such that:

$$\begin{gather} \oint \vec E \cdot \hat n\ d^2x \approx [[\vec E(\vec x)]] A \cdot \hat n(\vec x) = \text{enclosed charge} = \frac{\sigma}{\epsilon_0}\cdot A \\ \Rightarrow [[\vec E(\vec x)]] \cdot \hat n(\vec x) = \frac{\sigma}{\epsilon_0}\end{gather}$$

Where: $[[f(\vec x)]]_r = f(\vec x \to \vec x_r^+) - f(\vec x - \vec x_r^-)$ which represents the difference across a boundary.

The other boundary condition is the obvious one: $$\begin{gather} [[\vec E(\vec x)]] \times \hat n(\vec x) = 0 \end{gather}$$ which means that only the normal component of the [[Electric Field]] is affected by the surface of the charge.

Specifically since $\vec E(\vec x)$ in the interior of a conductor the field $\vec E(\vec x)$ at $\vec x \to \vec x_r^+$ is normal to the surface of the conductor.

Also if we have a volumetric charge in a finite zone of vacuum space then the field is continuous everywhere, including the "surface" of the charged region

![[volumetric charge density.png]]




