### Conceptual Definition
In electromagnetism, Gauss's Law, also known as Gauss's [[Flux]] theorem, is a law relating the distribution of [[Electric Charge]] to the resulting [[Electric Field]]. In its integral form it states that the flux of the electric field out of an arbitrary closed surface is proportional to the electric field across a surface enclosing any [[Charge Distribution]], irrespective of how that charge is distributed. Even though the law alone is insufficient to determine the electric field across a surface enclosing any charge distribution, this may be possible in cases where symmetry mandates uniformity of the field. Where no such symmetry exists, Gauss's law can be used in its differential form, which states that the [[Divergence]] of the electric field is proportional to the local density of charge.

### Integral Form
Gauss's Law may be expressed as: 

$$\begin{gather} \Phi_E = \frac{Q}{\epsilon_0} \end{gather}$$

where $\Phi_E$ is the [[Electric Flux]] through a closed surface $S$ enclosing any volume $V$, $Q$ is the total charge enclosed within $V$ and $\epsilon_0$  is the permittivity of free space. The flux is defined as a [[Surface Integrals]] of the electric field:

$$\begin{gather}\Phi_E = \iint_S \vec E \cdot dA\end{gather}$$

where $E$ is the [[Electric Field]], $dA$ is a vector representing an infinitesimal element of area of the surface.

### Differential Form
By the [[Divergence Theorem]] Gauss's law can alternatively be written in the differential form:

$$\begin{gather} \nabla \cdot \vec E = \frac{\rho}{\epsilon_0 \epsilon_r} \end{gather}$$

## Gauss's Law (From Jackson)

To obtain Guass's law we first consider a [[Point Charge]] $q$ and a closed surface $S$ as shown below:
![[gauss's law example from jackson.jpg]]

Let $r$ be the distance from the charge to a point on the surface, $\mathbf n$ be the outwardly directed unit normal to the surface at that point, $da$ be an element of surface area. If the [[Electric Field]] $\mathbf E$ at the point on the surface due to the charge $q$ camkes an angle $\theta$ with the unit normal, thenm the normal component of $\mathbf E$ times the area element is $$\begin{gather} \mathbf E \cdot \mathbf n\ da = \frac{q}{4\pi\epsilon_0} \frac{\cos\theta}{r^2}da \end{gather}$$

Since $\mathbf E \cdot \mathbf A = EA\cos\theta$

Since $\mathbf E$ is directed along the line from the surface element to the charge $q$, $\cos \theta\ da = r^2 d\Omega$. Therefore $$\begin{gather} \mathbf E \cdot \mathbf n da = \frac{q}{4\pi\epsilon_0} d\Omega \end{gather}$$

If we now integrate the normal component of $\mathbf E$ over the whole surface, it is easy to see that $$\begin{gather} \oint_S\mathbf E\cdot \mathbf n = \begin{cases} q/\epsilon_0 & \text{if q lies inside of S} \\ 0  & \text{if q lies outside of S}  \end{cases} \end{gather}$$

Proof:

$$\begin{gather} \oint E\cdot dA = \iiint \nabla \cdot \vec E\ dV \\ \frac{q}{4\pi\epsilon_0}\nabla \cdot \frac{\hat r}{r - r'} = \frac{q}{4\pi\epsilon_0}4\pi\delta^3(\vec r - \vec r') = \frac{q}{\epsilon_0}\delta^3(\vec r-\vec r') \\ \iiint \frac{q}{\epsilon_0}\delta^3(\vec r- \vec r') = \begin{cases} q/\epsilon_0 & \text{if} \ r = r' \\ 0 & \text{if}\ r \neq r' \end{cases}\end{gather}$$

See also: [[The Divergence of r hat over r2]]

For a discrete set of charges it is immediately apparent that: $$\begin{gather} \oint_S \mathbf E \cdot \mathbf n \ da = \frac{1}{\epsilon_0} \sum_iq_i \end{gather}$$

where the sum is over only those charges inside the surface $S$. For a continuous charge density: 

$$\begin{gather} \oint_S \mathbf E \cdot \mathbf n \ da = \frac{1}{\epsilon_0} \int_V \rho(\mathbf x) d^3x\end{gather}$$

Where $V$ is the volume enclosed by $S$.