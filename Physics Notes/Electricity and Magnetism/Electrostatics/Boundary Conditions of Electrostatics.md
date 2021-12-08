For Conductors

$$\begin{gather} \vec E = 0 \\ \vec E = \vec \nabla \phi \Rightarrow\phi = \text{const}\end{gather}$$

Consider a system where all the charges were to the left of some conducting surface or volume (apparently it doesn't matter). 

For our case 1 charge placed to the left of a conducting sheet. 

A charge q is placed at $(-x_0,y_0 = 0)$, the sheet is placed at $x=0$ where $\phi(x = 0,y) = \text{const}$

Note that:
$$\begin{gather}\phi(x,y) = \frac{1}{4 \pi \epsilon_0}\frac{q}{\sqrt{(x+x_0)^2+y^2}}\Bigg|_{x=0} \neq 0 \end{gather}$$

How do we solve this? We must use the [[Method of Images]]. In doing so we place a negative charge an equal distance away from the sheet on the other side. The solution then becomes:

$$\begin{gather}\phi(x,y) = \frac{1}{4 \pi \epsilon_0}\left[\frac{q}{\sqrt{(x+x_0)^2+y^2}} - \frac{q}{\sqrt{(x-x_0)^2+y^2}}\right] \end{gather}$$

For the insulator case:

$\vec E = 0$ with some charge distribution $\rho$ inside. So: $\vec E \cdot \hat n = 0$ and $\frac{\partial \phi}{\partial x} = 0$

Consider the same system as before, we use the [[Method of Images]] to determine the solution:

$$\begin{gather}\phi(x,y) = \frac{1}{4 \pi \epsilon_0}\left[\frac{q}{\sqrt{(x+x_0)^2+y^2}} + \frac{q}{\sqrt{(x-x_0)^2+y^2}}\right] \end{gather}$$

In a conductor with two charges: $q_1$ and $q_2$ on the left of the conductor. We do an image for both charges.

### Not infinite case
Consider a charge in the center of a region or radius R and everything outside of that region is a conductor. 

The electric field in side: $$\begin{gather}
|\vec x| < R \\ \vec E(\vec x) = \frac{1}{4\pi\epsilon_0} \frac{q}{r^2}   \\ \Phi(\vec x) = \frac{-1}{4\pi\epsilon_0}\frac{q}{r} \\ |\vec x| > R \\ \vec E(\vec x) = 0 \\ \Phi(\vec x) = \text{const} = \frac{-1}{4\pi\epsilon_0}\frac{q}{R}\end{gather}$$

Now we look at the total energy: 
$$\begin{gather} \iint \vec E\cdot \hat n \ dA = \frac{1}{\epsilon_0}Q_{en} = \frac{1}{\epsilon_0}q \\ \vec E \cdot \hat n =\sigma\end{gather}$$

Induced charges around the inside of the region

$$\begin{gather}\sigma = \frac{-q}{4\pi R^2} \end{gather}$$

Where $\sigma$ is the charge distribution.

