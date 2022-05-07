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
#### Summary of Radiation-Zone Results
$$\begin{gather} \vec A _{\text{rad}}(\vec r, t) = \frac{\mu_0}{4\pi r} \int d^3r' \vec j(\vec r', t - r/c + \hat r \cdot \vec r' /c)\end{gather}$$
Where the radiation fields $$\begin{gather} c \vec B_{\text{rad}} = -\hat r \times \frac{\partial \vec A_{\text{rad}}(\vec r, t)}{\partial t} \\ E_\text{rad} (\vec r,t) = - \hat r\times c \vec B_\text{rad}\end{gather}$$

We can use the Geometry of the Right Handed Triad:

![[Screenshot from 2022-05-04 16-01-48.png]]

From Zangwill 20.109 we have: 

$$\begin{gather} \hat r \times \vec E_{\text{rad}} = c \vec B_\text{rad} \\ \vec E_\text{rad} \times c \vec B_\text{rad} = \hat r|E_\text{rad}|^2 \end{gather}$$
So our power radiated can be written as: 

$$\begin{gather} \frac{dP}{d\Omega} = \frac{r^2}{c\mu_0}|\vec E_\text{rad}|^2 = \frac{1}{c\mu_0}\left|\vec r \times \frac{\partial \vec A_\text{rad}(\vec r,t)}{\partial t}\right|^2\end{gather}$$
We can also use: 

$$\begin{gather} \frac{dP}{d\Omega} = \frac{Z_0}{2}r^2 |\vec H|^2 \end{gather}$$