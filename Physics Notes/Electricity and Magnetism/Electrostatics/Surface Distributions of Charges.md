One of the common problems in electrostatics is the determination of [[Electric Field]] or [[Electric Potential]] do to a given a surface distributiuon of charges. [[Gauss's Law]] allows us to write down a partial result directly. If a surface $S$ with a unit normal $\mathbf n$ directed from side 1 to side 2 of the surface, has a surface-charge density $\sigma (\mathbf x)$ (measured in [[Coulomb]]s per square meter) and electric fields $E_1$ and $E_2$ on either side of the surface as shown here: 
![[surface distribution of charges 1.jpg]]

then Gauss's law tells us immediately that $$\begin{gather} (\mathbf E_2 - \mathbf E_1) \cdot \mathbf n = \sigma/\epsilon_0 \end{gather}$$

This does not determine $\mathbf E_1$ and $\mathbf E_2$ unless there are no other sources of field and the geometry and form of $\sigma$ are especially simple. All that the above equation says is that there is a discontinuity of $\sigma/\epsilon_0$ in the normal component of the electric field in crossing a surface with a surface-charge density $\sigma$, the crossing being made in the direction of $\mathbf n$.

The tangential component of electric field can be shown to be continuous across a boundary surface by using:

$$\begin{gather} \oint \mathbf E \cdot d \mathbf l =0 \end{gather}$$

for the [[Line Integrals]] of $\mathbf E$ around a closed path. It is only necessary to take a rectangular path with negligible ends and one side on either side of the boundary. An expression for the potential (hence the field, by differentiation)  at any point in space (not just at the surface) can be obtained by: 

$$\begin{gather} \Phi(\mathbf x) =\frac{1}{4\pi \epsilon_0} \int_S \frac{\sigma(\mathbf x')}{|\mathbf x - \mathbf x'|}da' \end{gather}$$