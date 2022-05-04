 ## Vector Potential 
$$\begin{gather} \vec A (\vec x) = \frac{\mu_0}{4\pi} \frac{e^{ikr}}{r}\int \vec J ( \vec x' ) d^3x' \end{gather}$$
Note: this is the $l=0$ part of the series and is valid everywhere outside the source.

Using the Continuity equation one can write the vector potential as:


$$\begin{gather} \vec A (\vec x) = \frac{-\mu_0 \omega}{4\pi } \vec p \frac{e^{ikr}}{r}\end{gather}$$

Where the electric dipole moment $\vec p$ is defined as: 

$$\begin{gather} \vec p = \int \vec x' \rho (\vec x') d^3x'\end{gather}$$

## Fields
$$\begin{gather} \vec H = \frac{ck^2}{4\pi}(\hat n \times \vec p)\frac{e^{ikr}}{r}\left(1-\frac{1}{ikr}\right) \\ \vec E = \frac{1}{4\pi\epsilon_0} \left\{k^2(\hat n \times \vec p)\times \hat n \frac{e^{ikr}}{r} + [3\hat n(\hat n \cdot \vec p)-\vec p] \left(\frac{1}{r^3}-\frac{ik}{r^2}\right)e^{ikr} \right\} \end{gather}$$
#### Far Field (Radiation Zone)
$$\begin{gather} \vec H = \frac{ck^2}{4\pi}(\hat n\times \vec p)\frac{e^{ikr}}{r} \\ \vec E = Z_0\vec H \times \hat n \end{gather}$$
#### Near Field (Similar to Static Case)
$$\begin{gather} H = \frac{i\omega}{4\pi} (n \times \vec p) \frac{1}{r^2} \\ \vec E = \frac{1}{4\pi\epsilon_0} [3\hat n(\hat n \cdot \vec p)-\vec p]\frac{1}{r^3} \end{gather}$$
#### Power Radiated per unit solid angle
$$\begin{gather} \frac{dP}{d\Omega} = \frac{1}{2} \text{Re}[r^2 \hat n \cdot \vec E \times \vec H^*]  \\ \frac{dP}{d\Omega} = \frac{c^2 Z_0}{32 \pi^2}k^4 |(\hat n \times \vec p) \times \hat n|^2\end{gather}$$