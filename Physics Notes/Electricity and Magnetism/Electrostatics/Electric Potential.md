### Definition

The electric potential is defined as the amount of [[Work]] energy needed to move a unit of [[Electric Charge]]  from a reference point to the specific point in the [[Electric Field]] 

The electric potential at a pint $\mathbf r$ in a static electric field $\vec E$ is given by the [[Line Integrals]]: 

$$\begin{gather} V_E = -\int_CE\cdot dl \end{gather}$$

where $C$ is some arbitrary path from some fixed reference point to $\vec r$. In electrostatics the [[Maxwell-Faraday Equation]] reveals that the curl $\Delta \times E$ is zero, making the electric field conservative. Thus the line integral does not depend on the specific path $C$ chosen but only on its endpoints, making $v_E$ well-defined everywhere. The [[Gradient]] theorem allows us to writ:

$$\begin{gather} E = -\nabla V_E \end{gather}$$
This states that the electric field points "downhill" towards lower voltages.


### Electric Potential due to a point charge

The electric potential arising from a [[Point Charge]] $Q$ at a distance $r$ from the charge is observed to be $$\begin{gather} V_E = \frac{1}{4\pi\epsilon_0}\frac{Q}{r} \end{gather}$$

where $\epsilon_0$ is the [[Permitivity of vacuum]], $V_E$ is known as the Coulomb Potential. The electric potential for a system of point charges is equal to the sum of the point charges' individual potentials. This fact simplifies calculations significantly, because addition of potential fields is much easier than addition of the electric fields. Specifically:, the potential of a set of discrete point charge $q_i$ at points $\vec r_i$ becomes

$$\begin{gather}V_E(\vec r) =\frac{1}{4\pi e_0} \sum_i \frac{q_i}{|\vec r - \vec r_i|} \end{gather}$$

where
$\vec r$ is a point which the potential is being evaluated
$\vec r_i$ is a point at which there is a nonzero charge 
$q_i$ is the charge a the point $\vec r_i$

and the potential of a continuous charge  distribution $\rho(r)$ becomes 

$$\begin{gather} V_E = \frac{1}{4\pi\epsilon_0}\int_R\frac{\rho(r')}{|r-r'|}d^3r' \end{gather}$$