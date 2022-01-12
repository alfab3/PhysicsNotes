An electric field is the physical field that surrounds electrically charged particles and exerts force on all other charged particles in the field, either attracting or repelling them. It also refers to the physical field for a system of charged particles. Electric fields originate from electric charges or from time varying magnetic fields. Electric fields and magnetic fields are both manifestations of the [[Electromagnetic Force]]. 

The electric field is defined mathematically as a [[Vector Field]] that associates to each point in space force per unit of charge exerted on an infinitesimal positive [[Test Charge]] at rest at that point. The units for the electric field are volts per meter or Newtons per Coulomb. 

## Mathematical Formulation

$$\begin{gather} \vec E(\vec x_0) = \frac{\vec F}{q_0} = \frac{1}{4\pi\epsilon_0}\frac{q_1}{(\vec x_1 - \vec x_0)}\hat r_{1,0}\end{gather}$$

This is the electric field at position $\vec x_0$ due to the point charge $q_1$. Where charge 0 is $q_0$ at position $\vec x_0$ and charge 1 is $q_1$ at position $\vec x_1$, and $\hat r_{1,0}$ is the unit vector in the direction from point $\mathbf x_1$ to $\mathbf x_0$

### Superposition principle 

Electric fields satisfy the superposition principle, which states that the total electric field at a point, due to a collection of charges is equal to the vector sum of the electric fields at that point due to the individual charges:

$$\begin{gather} \vec E(\vec x) = \vec E_1(\vec x) + \vec E_2(\vec x) + \vec E_3(\vec x) + \ldots = \frac{1}{4\pi\epsilon_0}\sum^N_{k=1}\frac{q_k}{(\vec x_k- \vec x)^2} \hat r_k\end{gather}$$

### Continuous charge distributions 
The superposition principle allows for the calculation of the electric field due to a continuous distribution of charge $\rho(\vec x)$ where $\rho$ is the [[Charge Density]] in coulombs per cubic meter. By considering the charge $\rho(\vec x')dV$ at point $x'$ as a point charge, the resulting electric field, $dE(x)$ at point $x$ can be calculated as
$$\begin{gather} d\vec E(x)  = \frac{1}{4\pi\epsilon_0} \frac{\rho(x')dV}{(x'-x)^2}\hat r' \end{gather}$$

where $\hat r'$ is the unit vector pointing $x'$ to $x$. The total field is then found by adding up the contributions from all the increments of volume by integrating over the volume of the charge distribution $V$: 

$$\begin{gather} \vec E(x)  = \frac{1}{4\pi\epsilon_0}\iiint_V \frac{\rho(x')dV}{(x'-x)^2}\hat r' \end{gather}$$

Similar equations follow for a surface charge with continuous charge distribution $\sigma (x)$ where $\sigma$ is the charge density in coulombs per square meter.

$$\begin{gather} \vec E(x)  = \frac{1}{4\pi\epsilon_0}\iint_S \frac{\sigma(x')dV}{(x'-x)^2}\hat r' \end{gather}$$

and for line charges with continuous charge distribution $\lambda(x)$ where $\lambda$ is the charge density in coulombs per meter
$$\begin{gather} \vec E(x)  = \frac{1}{4\pi\epsilon_0}\int_P \frac{\lambda(x')dV}{(x'-x)^2}\hat r' \end{gather}$$