### Define 1st Order Operators
Note that we can write the wave equation in ($1+1$) dimensions as $$\begin{gather} \frac{\partial^2u}{\partial t^2} -c^2 \frac{\partial^2 u}{\partial x^2} = \mathcal {L} _+ \mathcal L_- u =  \mathcal {L} _- \mathcal L_+u = 0 \end{gather}$$

where:

$$\begin{gather} \mathcal L_- = \frac{\partial}{\partial t} - c\cdot\frac{\partial}{\partial x} \\ \mathcal L_+ = \frac{\partial}{\partial t} + c\cdot\frac{\partial}{\partial x} \end{gather}$$

This shows the solution to the 1st order [[Partial Differential Equation]] is also a solution to the Second order [[Wave Equation]]. The reverse is also true.

Consider the characteristic families of the 1st order PDEs

$$\begin{gather} x - ct = \text{const} \equiv \eta \\ x + ct = \text{const} \equiv \zeta\end{gather}$$


Use the coordinate transform:

$$\begin{gather} \eta = x - ct; \;\;  \zeta = x+ct \\ \Rightarrow x = \frac{1}{2}(\eta + \zeta);\;\; t=\frac{1}{2c}(\zeta-\eta) \\ \Rightarrow \frac{\partial}{\partial \eta} = - \frac{1}{2c}\mathcal L_- \\\frac{\partial}{\partial \zeta} = \frac{1}{2c}\mathcal L_+ \\ \Rightarrow \frac{\partial^2u}{\partial t^2} -c^2 \frac{\partial^2 u}{\partial x^2} = \mathcal L_+ \mathcal L _-u =0 \Rightarrow \frac{\partial^2}{\partial \eta \partial \zeta} u = 0\end{gather}$$


### Solution
The most general solution of the reformulated wave equation is:
 
$$\begin{gather} u(\eta,\zeta) = f(\eta) + g(\zeta)\end{gather}$$

Where $f$ and $g$ are both functions of single variables and must be determined from initial conditions on $u$ and $\frac{\partial u}{\partial t}$ at  $t = 0$

The first order operators define its own set of characteristics: 
![[diffopscharacteristiccurves.png]]

#### Determining $f(\eta)$ and $g(\zeta)$

Let us consider the initial conditions:

$$\begin{gather} u(x,t = 0)) = f(\eta)\bigg|_{\eta=x-ct}+g(\zeta)\bigg|_{\zeta=x+ct} = f(x) + g(x)\end{gather}$$

and

$$\begin{gather} \frac{\partial u}{\partial t}(x,t=0) = \frac{\partial \eta}{\partial t} f'(\eta)\bigg|_{\eta=x-ct} + \frac{\partial \zeta}{\partial t} g'(\zeta)\bigg|_{\zeta=x+ct} = c(-f'(x) +g'(x))\end{gather}$$

Integrating the [[Derivative]] terms and combining with the first case we get:

$$\begin{gather} g(x) = \frac{1}{2}u(x,t=0) + \frac{1}{2c}\int_{x_0}^{x}\frac{\partial u}{\partial t}(x',t = 0)dx' + \frac{A}{2} \\ f(x) = \frac{1}{2}u(x,t=0) - \frac{1}{2c}\int_{x_0}^{x}\frac{\partial u}{\partial t}(x',t = 0)dx' - \frac{A}{2}\end{gather}$$

So the solution of the [[Wave Equation]] is: 

$$\begin{gather} u(x,t) = g(x + ct) + f(x -ct) \\ \Rightarrow u(x,t) = \frac{1}{2}(a(x+ct)-a(x-ct)) + \frac{1}{2c}\int^{x+ct}_{x-ct} b(x')dx' \end{gather}$$

where: 

$$\begin{gather} a(x) = u(x,t=0)\\ b(x) = \frac{\partial u}{\partial t}(x,t=0) \end{gather}$$

This is equivalent to the [[Fourier Solution of the Wave Equation]].