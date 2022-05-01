## Fields and Radiation of a Localized Oscillating Source
#### Charges and Currents that vary sinusoidally in time: 

>$$\begin{gather} \rho(\vec x, t) = \rho(\vec x)e^{-i\omega t} \\ \vec J(\vec x,t) = \vec J (\vec x)e^{-i \omega t}\end{gather}$$

#### Vector Potential
##### Lorenz Gauge
$$\begin{gather} \vec A(\vec x,t) = \frac{\mu_0}{4\pi} \int d^3x' \int dt' \frac{\vec J(\vec x',t')}{|\vec x-\vec x'|} \delta(t' + \frac{|\vec x- \vec x'|}{c} -t)\\ \vec A (\vec x)= \frac{\mu_0}{4\pi} \int \vec J(\vec x') \frac{e^{ik|\vec x - \vec x'|}}{|\vec x - \vec x'|} d^3x'\end{gather}$$


#### Fields
$$\begin{gather} \vec H = \frac{1}{\mu_0} \nabla\times\vec A \\ \vec E = \frac{iZ_0}{k} \nabla \times \vec H  \\ Z_0 = \sqrt{\mu_0/\epsilon_0}\end{gather}$$


#### Field Zones
Definitions: Source dimensions: $d$, wavelength: $\lambda = 2\pi c/\omega$, $d \ll \lambda$ 

The near (static) zone: $d \ll r \ll \lambda$
The intermediate (induction) zone: $d \ll r \approx \lambda$ 
The Far (radiation) zone: $d \ll \lambda \ll r$ 

#### Scalar Potential 
$$\begin{gather} \Phi (\vec x,t) = \frac{1}{4\pi \epsilon_0} \int d^3x' \int dt' \frac{\vec \rho(\vec x',t')}{|\vec x-\vec x'|} \delta(t' + \frac{|\vec x- \vec x'|}{c} -t) \end{gather}$$