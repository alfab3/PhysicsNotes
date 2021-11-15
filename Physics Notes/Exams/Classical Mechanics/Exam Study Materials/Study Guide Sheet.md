## Newtonian Dynamics
#### Newton's Second Law:
$$\begin{align} m\ddot{\vec x} = \vec F = -\frac{\partial U}{\partial r}\end{align}$$


## Two Body
#### Effective Potential:

$$\begin{align} U_{eff} = U(r)+\frac{l^2}{2mr^2} \end{align}$$

#### Polar Coordinates in a plane
$$\begin{align} x = r\cos\theta \\ y = r\sin\theta \\ v = \dot r^2 + r^2 \dot \theta ^2\end{align}$$

#### Conservation of Angular Momentum

$$\begin{align} \dot{\theta} = \frac{l}{mr^2} \end{align}$$

#### Torque
Defined as $$\begin{align}\vec \tau = \frac{d\vec L}{dt} = \vec{r} \times \vec{F}\end{align}$$

Which defines the rotational force. 
$\vec r$ is the position vector which points from the origin to the rotating body 
$\vec F$ is the force vector which points in the direction of motion
$\vec \tau$ Would then point out of the (2D) plane of motion

so if Angular momentum is a constant, there is no Torque, and in the context of an orbit the motion is confined to a 2D Plane

#### Energy
$$\begin{align}\frac{m\dot x^2}{2} + U(x) = E\end{align}$$

Now everything can be derived from this point. 



#### Stability of Orbit:
Determine if 
$$\begin{align} \frac{dV}{dr}\Bigg|_{r=r_0} \end{align}$$

Defines a local max or minimum, can be done by taking the limit as $r \to 0$, or second derivative test.

#### Conical Section
$$\begin{align} \frac{1}{\rho} = 1 + \lambda_e \cos\theta \end{align}$$

Where $\rho$ is the radius from the focus of the ellipse and $\lambda$ is the eccentricity.

#### Laplace-Runge-Lenz Vector

$$\begin{align} \vec{I} = \frac{1}{\gamma} (\vec v \times \vec L) -\frac{\vec r}{r} \end{align}$$

This is a conserved quantity

Also you can derive the conical section by dotting it with $\vec r$

## Calculus of Variations
Determining the Functional:

2D: 
Cartesian:
$$\begin{align} ds^2 = dx^2+dy^2\end{align}$$
Polar: 
$$\begin{align} ds^2 = dr^2+r^2d\theta^2\end{align}$$

Which can be rewritten as:
$$\begin{align}
ds = \sqrt{1 + y'^2}\ dx
\end{align}$$
Where $y' \equiv \frac{dy}{dx}$

$$\begin{align} ds = \sqrt{r'+r^2}\ d \theta
\end{align}$$

Where $r' = \frac{dr}{d\theta}$

The functional then takes the form:

$$\begin{align} l[f] = \int ds\end{align}$$

Where ds is defined by the length. This is the distance between two point (defined by integral bounds)

To find the shortest distance the integrand must satisfy Euler's equation:

$$\begin{align} \frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'} = 0\end{align}$$

Where $f$ is the integrand.

The Second Form of the Euler Equation

Convenient for use for functions that do not depend on $x:\partial f/\partial x =0$

$$\begin{align} \frac{\partial f}{\partial x} - \frac{d}{dx}\left(f - y'\frac{\partial f}{\partial y'}\right)=0\end{align}$$

Then:

$$\begin{align} f - y'\frac{\partial f}{\partial y'} = \text{const} \end{align}$$
## Lagrangian Formalism

The Lagrangian is defined as: $$\begin{align} \mathcal{L} = T - V\end{align}$$

Where $T$ is kinetic energy and $V$ is potential

#### Steps to determine Lagrangian:

First: Write out position terms (i.e. $x$, $y$, $r$, $\theta$)
Second: Take the time derivative of each position function
Third: Plug in values to $T$ term
Fourth: Use your vertical term to write the potential $U$
Fifth: Plug in and complete Lagrangian

#### Equations of Motion
One must solve the Euler - Lagrange Equation for each DoF term:

$$\begin{align} \frac{\partial \mathcal{L}}{\partial q_i} - \frac{d}{dt}\frac{\partial \mathcal{L}}{\partial \dot{q}_i} = 0\end{align}$$

Where $q_i$ represents some generalized coordinate.

#### Noether's Process

First - Find a symmetry transformation $q \rightarrow q + \delta q$ where $\delta q$ depends on a tiny parameter constant parameter $\epsilon$.

This should send $\mathcal{L} \rightarrow \mathcal{L}$ (meaning it is invariant)

Second - Make the tiny constant parameter $\epsilon$ into a tiny time dependent parameter $\epsilon(t)$. You should find that instead of $\mathcal{L} \rightarrow \mathcal{L}$ as before $\mathcal{L} + \dot\epsilon B$

Third - recall that a solution to EoM, $\delta S = 0$ if $\epsilon(t_1) = \epsilon(t_2) = 0$

Therefore $0 = \delta S = \int^{t_2}_{t_1} \dot\epsilon B dt = - \int^{t_2}_{t_1}\epsilon \dot Bdt$

Therefore $\dot B = 0$


#### Linear Momentum
Spatial Translation Symmetry
$$\begin{align} \sum^N_{j=1} \frac{\partial \mathcal L}{\partial \dot {\vec r}_j}\end{align} = \vec P$$
#### Angular Momentum
Rotational Symmetry

Angular Momentum is defined as the conjugate momentum to the angular variable:
$$\begin{align} l = \frac{\partial \mathcal{L}}{\partial \dot{\theta}} \end{align}$$

#### Energy
Time Translational Symmetry
$$\begin{align} \frac{d}{dt}\left(\sum^N_{j=1}\dot{\vec{r}}_j\frac{\partial \mathcal L}{\partial \dot{\vec{r}}} - \mathcal L\right) = -\frac{\partial \mathcal L}{\partial t} \end{align}$$

Where energy is given as:

$$\begin{align}E = \sum_\alpha \dot{q}_\alpha\frac{\partial \mathcal L}{\partial \dot{q}_\alpha} - \mathcal L = \text{const} \end{align}$$

### Lagrangian Multipliers

Steps:
First - develop fully constrained Lagrangian 
Second - Add Conditionally Constrained terms $$\begin{align} \mathcal{L'} = \mathcal{L} + \sum\lambda_i f_i\end{align}$$

Where $\lambda_i$ are undetermined & $f_i$ and the equations of constraint of the form $f(\{q\}) = \text{const}$

Third - Non-dimensionalize:

Some quantities are:

$$\begin{align} \vec R \leftrightarrow \frac{\vec R}{a} \\ \\ t \leftrightarrow t\sqrt{g/a} \\ \\I \leftrightarrow \frac{I}{ma^2} \\ \\ U \leftrightarrow \frac{U}{mga}\\ \\ T \leftrightarrow \frac{T}{mga}\end{align}$$

Fourth - Find equations of Motion from $\mathcal{L'}$
Fifth - Find equations of motion from $\mathcal{L}$
- use a quantity to rewrite formula in the form of one variable

Sixth - Use equation of motion to get $\lambda_i$

Seventh - Constraint ends when $\lambda_i=0$  

#### Key Points
Derive EoM first, then the EoMs with the multiplier

#### Forces of Constraint
Rolling object will always be:
arc_length_1 = arc_length_2

Constraint causes $\lambda$ to go to 0 when the constraint "ends"