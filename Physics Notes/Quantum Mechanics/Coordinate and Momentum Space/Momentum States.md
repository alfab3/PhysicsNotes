A momentum state is no more than a linear combination of [[Coordinate Space]] states, 

$$\begin{gather} \ket{p} = \int dx e^{ipx/\hbar} \ket{x} \\ \braket{x|p} = \int dx' e^{ipx'/\hbar} \braket{x|x'} \\ = \int dx' e^{ipx'/\hbar} \delta(x-x') \\ = e^{ipx/\hbar} \end{gather}$$
With this definition of the state $\ket{p}$ the normalization becomes
$$\begin{gather} \braket{p'|p} = \int dxdx' e^{i(px-p'x')\hbar}\braket{x'|x} \\ = \int dx\ e^{i(p-p')x/\hbar} \\ = 2\pi \hbar \delta (p-p')\end{gather}$$
Aside: [[Fourier Transforms and Delta Functions]]

The inverse transformation is $$\begin{gather} \ket{x} = \frac{1}{2\pi\hbar} \int dp e^{-ipx/\hbar}\ket{p} \end{gather}$$
Expressed as a [[Completeness Relation]] 
$$\begin{gather} \int \frac{dp}{(2\pi \hbar)} \braket{x|p}\braket{p|x'} = \int \frac{dp}{(2\pi \hbar)}e^{ip(x-x')/\hbar} \\ = \delta(x'-x) = \braket{x|x'} \end{gather}$$

Thus, 

$$\begin{gather} \frac{1}{2\pi \hbar} \int dp \ket{p} \bra{p} = \mathbb{I} \end{gather}$$
Sandwiching this between some normalized [[States]] $\psi$,

$$\begin{gather} \frac{1}{2\pi\hbar} \int dp\braket{\psi|p}\braket{p|\psi} = \braket{\psi|\psi} \\ \frac{1}{2\pi\hbar}\int dp\psi^*(p)\psi(p) = 1 \\ \psi(p) = \braket{p|\psi} \end{gather}$$

Thus the probability per differential momentum ([[Table of Contents/Momentum]]) for observing a particle with momentum $p$ in some state $\psi$ is 

$$\begin{gather} \frac{dP_\psi}{dp} =\frac{1}{2\pi\hbar}\psi^*(p)\psi(p) \end{gather}$$
Changing the problem to $n$ dimensions only affects the expressions here by changing $dp$ to $d^np$ and replacing $(2\pi\hbar)$ with $(2\pi\hbar)^n$ 

The label $p$ here refers to a continuum of momentum states. If a system is confined, then no [[Eigenstate]]s of the momentum operator really exists, but one still uses the label $p$ to point to eigenstate of the momentum operator within the volume, but with discrete values of $p$ rather than a continuum. In that case the normalizations are different. It is the duty of the watchful reader to accurately interpret the notation. 

The momentum and position [[Operator]]s can be expressed as:

$$\begin{gather} \mathcal X = \int dx\ x \ket{x}\bra{x}  \\ \mathcal P = \int\frac{dp}{2\pi\hbar}p\ket{p}\bra{p}\end{gather}$$

From the definition of $\mathcal X$, one can see that
$$\begin{gather} \braket{\phi|\mathcal X|\psi} = \int dx \braket{\phi|x}x\braket{x|\psi(x)} \\ = \int dx \phi^*(x)x\psi(x) \end{gather}$$
One can also perform a similar operation with the momentum operator. 

$$\begin{gather} \braket{\phi|\mathcal P|\psi} = \int \frac{dp}{2\pi\hbar} \phi^*(p)p\psi(p) \\ \psi(p) = \braket{p|\psi}  \end{gather}$$
However, the customary way to view the momentum operator is not in momentum space, but as a derivative in coordinate space. Expanding $\ket{p}$ in terms of coordinate space states, one can use completeness to express the $\braket{\phi|\mathcal P|\psi}$ in terms of the [[Wave function]]s: 
$$\begin{gather} \mathcal P =\int dx \ket{x} (-i\hbar\partial_x)\bra{x} \end{gather}$$

This algebra also shows that the one can write the momentum as a left acting derivative but with a change of sign. 

Thus the momentum operator can be thought of a $-i\hbar\partial/\partial x$. 

Applying the [[Commutator]] to $\mathcal P$ and $\mathcal X$ 

$$\begin{gather} [\mathcal P, \mathcal X] = \int dx \ket{x}(-i\hbar)(x\bra{x}) - \int dx \ket{x}(x(-i\hbar\partial_x))\bra{x} \\ = -i\hbar\int dx \ket{x}\bra{x} \\ = -i\hbar \mathbb{I} \end{gather}$$
One should keep in mind that in many applications the definition of a momentum state: 

$$\begin{gather} \braket{x|p} \equiv \begin{cases} e^{ipx}/\sqrt{L}, & 0<x<L \\ 0, & otherwise \end{cases} \end{gather}$$

where $L\to \infty$. For this definition $\braket{x|p}$ has dimensions of length$^{-1/2}$, and the values of $p$ are discrete. The normalization of the momentum states are 
$$\begin{gather} \braket{p|p'} = \delta_{pp'} \end{gather}$$
which are [[Kronecker Delta]] functions instead of [[Dirac Delta Function]]s. These states are not actually eigenstates of the momentum operator because $-i\hbar\partial_x\braket{x|p} \neq p\braket{(x|p)}$ when $x < 0$ or $x > L$. Typicaly, this choice is useful when one is considering emission into a continuum of momentum states, and the density of such states factors into the answers. Because the density of states is proportional to $L$, the arbitrarily large lengths cancel from the answer.

Aside: [[Schrodinger's Equation as an Operator]]
