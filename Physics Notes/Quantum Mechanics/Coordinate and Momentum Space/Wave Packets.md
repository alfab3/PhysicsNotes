A plane wave confined to a finite regions can be written as 
$$\begin{gather} \psi_{p,L} (x) = \braket{x|p,L} = \frac{1}{\sqrt{L}} e^{ipx/\hbar}  \end{gather}$$

which is normalized in the Length $L$, but is not really an [[Eigenstate]] of the momentum operator due to sharp cutoff at the boundaries. A more physical description of a wave that is confined to a finite region is a wave packet, which confines the probability to a finite region, and because of the uncertainty principle it is accompanied by a spread in the momentum. This state $\ket{Q}$ will NOT be an eigenstate of the momentum operator, but will instead be a linear combination of states $\ket{p}$, which are eigenstates of the momentum operator $\mathcal P = - i\hbar \nabla$.

$$\begin{gather} \ket{Q} = \int\frac{dp}{2\pi\hbar}g(p-Q)\ket{p} \\ g(p-Q) = \braket{Q|p} \end{gather}$$
For our purposes we will assume $g$ to be of a Gaussian form $$\begin{gather} g(p-Q) = \alpha \exp\left(\frac{-(p-Q)^2}{4\Delta^2}\right) \end{gather}$$

The resulting wave packet is properly normalized by:

$$\begin{gather}\alpha = (2\pi)^{1/4}\sqrt{\frac{\hbar}{\Delta}}\end{gather}$$

With this definition, the width of the wave packet in momentum space ([[Momentum States]]) is $\Delta$, i.e. 

$$\begin{gather} \braket{Q|(\mathcal P - \bar{P} |Q} = \frac{1}{2\pi\hbar}\int dp (p- \bar{P})[g(p-Q)]^2 = \Delta^2 \\ \bar P \equiv \braket{Q|P|Q} \end{gather}$$

To understand the spatial shape of the packet, one can see that 
$$\begin{gather}\psi_Q(x) = \braket{x|Q} = \int \frac{dp}{2\pi\hbar} \braket{x|p} \braket{p|Q}\\ = \int \frac{dp}{2\pi\hbar} e^{ipx/\hbar}g(p-Q) \\ = \frac{\alpha\Delta}{\hbar}\sqrt{\frac{2}{\pi}}e^{iQx/\hbar}e^{-x^2\Delta^2/\hbar^2} \\ |\psi_Q(x)|^2=\frac{2 \Delta}{\hbar}\sqrt{\frac{1}{2\pi}}\exp \left\{-\frac{(2\Delta)^2}{\hbar^2}\frac{x^2}{2} \right\} \end{gather}$$

which is also of Gaussian form, with the spatial spread being $\hbar/(2\Delta)$ 

Thus, the product of the spread in momentum space multiplied by the spread in coordinate space is $\hbar/2$ exactly the minimum allowed by the uncertainty principle. If the packet had been described with $e^{ipx/\hbar} \to e^{ip(x-x_0)/\hbar}$, the packet would be centered at $x_0$ instead of the origin. 

For the wave packet at arbitrary times, 

$$\begin{gather} \psi_Q(x,t) = \int \frac{dp}{2\pi\hbar}e^{-iE_pt/\hbar+ipx/\hbar}g(p-Q) \end{gather}$$

we expect the packet to move in time. The packet has contributions from all momenta which represent differential additions with a wide variety of phases for each $p$. At most values of $x$ these phases for each $p$. At most values of $x$ these phases vary to the degree that resulting [[Wave function]] is near zero. However at any given time $t$ there is a point $x$ for which the phases are constant as $p$ is varied near $Q$.  At this point the differential contributions add in-phase and the wave function in coordinate space is a maximum. To find what point we take a derivative of the phase with respect to $p$ at $Q$, and require it to be zero.

$$\begin{gather} \frac{d}{dp}(-iE_pt + ipx)|_{p=Q} = 0 \\ x= \frac{dE_p}{dp}t\end{gather}$$

Given that $dE/dp|_{p=Q} = v$ even for relativistic particles one sees that $x = vt$ which is not surprising. Here $g(p)$ was assumed to be a real function, but if it were given a momentum-dependent phases, $e^{i\phi(p)}$, then the same condition would lead to $x=vt-\hbar d\phi/dp|_{p=Q}$ and the additional term would set the position of the wave packet away from the origin, even at $t=0$. 