## Vector Potential
The Second term in our vector potential expansion. 
$$\begin{gather} \vec A(\vec x) = \frac{\mu_0}{4\pi}\frac{e^{ikr}}{r}\left(\frac{1}{r}-ik\right)\int\vec J(\vec x')(\hat n \cdot \vec x')d^3x' \end{gather}$$


### Integrand
$$\begin{gather} (\hat n \cdot \vec x')\vec J= \frac{1}{2}[(\hat n \cdot \vec x')\vec J + (\hat n\cdot\vec J) \vec x'] + \frac{1}{2}(\vec x' \times\vec J) \times\hat n \end{gather}$$

The second term is the magnetization term: 

$$\begin{gather} \mathcal M = \frac{1}{2}(\vec x \times \vec J) \end{gather}$$
Which gives us: 

$$\begin{gather} A(\vec x) = \frac{ik\mu_0}{4\pi} (\hat n \times\vec m) \frac{e^{ikr}}{r} \left(1-\frac{1}{ikr}\right) \\ \vec m = \int \mathcal Md^3x = \frac{1}{2}\int(\vec x \times \vec J) d^3x\end{gather}$$
### Fields Magnetization Term
$$\begin{gather} \vec E = - \frac{Z_0k^2}{4\pi}(\hat n \times \vec m)\frac{e^{ikr}}{r}\left(1-\frac{1}{ikr}\right) \\ \vec H = \frac{1}{4\pi} \left\{k^2(\hat n \times \vec m)\times \hat n \frac{e^{ikr}}{r} + [3\hat n(\hat n \cdot \vec m)-\vec m] \left(\frac{1}{r^3}-\frac{ik}{r^2}\right)e^{ikr} \right\} \end{gather}$$
### Fields Symmetric Term (In Radiation Zone)
$$\begin{gather} \vec H = ik\hat n \times\vec A/\mu_0 \\ \vec E = ikZ_0(\hat n \times \vec A ) \times \hat n/\mu_0 \end{gather}$$

#### Quadrupole Tensor 
$$\begin{gather} Q_{\alpha\beta} = \int(3x_\alpha x_\beta - r^2\delta_{\alpha\beta}) \rho(x)d^3x \end{gather}$$
We define the components of $\vec Q(\vec n)$: 

$$\begin{gather} Q_\alpha = \sum_\beta Q_{\alpha \beta} n_\beta\end{gather}$$
### Magnetic Induction 
$$\begin{gather} \vec H = -\frac{ick^3}{24\pi}\frac{e^{ikr}}{r}\hat n \times \vec Q(\hat n) \end{gather}$$

#### Time Averaged power radiated per unit solid angle
$$\begin{gather} \frac{dP}{d\Omega} = \frac{c^2 Z_0k^6}{1152\pi^2}|[\hat n \times \vec Q(\hat n )]\times\hat n]^2 \\ |[\hat n \times\vec Q(\hat n)]\times\hat n|^2 = \vec Q^* \cdot \vec Q - |\hat n \cdot\vec Q|^2 \end{gather}$$

However the Quadrupole Tensor is traceless so: 

$$\begin{gather} P = \frac{c^2 Z_0 k^6}{1440 \pi} \sum_{\alpha, \beta}|Q_{\alpha\beta}|^2 \end{gather}$$
## Example: Oscillating Spheroidal Distribution of Charge
Off diagonal elements of $Q_{\alpha\beta}$ vanish. The diagonal terms are
$$\begin{gather} Q_{33} = Q_0, \;\; Q_{11} = Q_{22} = -\frac{1}{2}Q_0\end{gather}$$
Angular distribution of radiated power is 
$$\begin{gather} \frac{dP}{d\Omega} =\frac{c^2Z_0k^6}{512\pi^2}Q_0^2 \sin^2\theta \cos^2\theta \\ P =\frac{c^2Z_0k^6 Q_0^2}{960 \pi} \end{gather}$$
