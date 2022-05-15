## Step and Delta Functional Potential
The One-Dimensional Schrodinger Equation takes the form:
$$\begin{gather} \left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2} + U(x)\right]\psi(x) = E\psi(x) \end{gather}$$
### Delta Functional Potential: 
$$\begin{gather} U(x) = g\delta(x-x_0) \end{gather}$$

Boundary Conditions: 
$$\begin{gather} \psi'(x_* + \epsilon)-\psi'(x_*-\epsilon) = \frac{2m}{\hbar^2} \int^{x_*+\epsilon}_{x_*-\epsilon} U(x)\psi(x)+\mathcal O(\epsilon) \end{gather}$$
Explicit integration of U results in  (with $\lim_ {\epsilon\to 0}$): 

$$\begin{gather} \psi'(x_0+0) - \psi'(x_0-0) = \frac{2mg}{\hbar^2} \psi(x_0) \end{gather}$$
#### Properties:
$$\begin{gather} \psi(x) = \sqrt{\kappa}e^{-\kappa|x-x_0|} \;\;\;\;\; \kappa= \frac{m|g|}{\hbar^2} \\ E = -\frac{\hbar^2\kappa^2}{2m} = -\frac{mg^2}{2\hbar^2}\end{gather}$$

### Square Well
$$\begin{gather} U(x) = \begin{cases} -U_0 & |x| < a \\ 0, & |x|>a \end{cases} \end{gather}$$

![[Screenshot from 2022-05-09 12-08-39.png]]

#### Nondimensionalization
Transformations:
$$\begin{align} x &\to ax \\ U(x) &\to \frac{\hbar^2}{2ma^2}U(x) \\ E &\to \frac{\hbar^2}{2ma^2}E \\ \frac{d}{dx} &\to \frac{1}{a} \frac{d}{dx}\end{align}$$
I prefer to write it more explicitly:
$$\begin{gather} \xi = kx \\ \frac{d}{dx} = k\frac{d}{d\xi} \end{gather}$$
$$\begin{gather} -\psi''(x) + U(x)\psi(x) = E\psi(x) \\   U(x) = \begin{cases} -U_0 & |x| < 1 \\ 0, & |x|>1 \end{cases} \\ U_0 \to \frac{\hbar^2}{2ma^2}U_0\end{gather}$$

#### Analysis of Symmetries
Our solutions in the $|x|<1$ region are: 
$$\begin{gather} \psi_+(x) = A\cos(kx), \;\;\; \psi_-(x) = A\sin(kx), \;\;\; k = \sqrt{U_0-|E|} \;\;\; (|x| \leq 1) \end{gather}$$

Then in the $|x| > 1$ solution is: 

$$\begin{gather} \psi(x) = Be^{-\kappa x}, \;\; x =\sqrt{|E|}, \;\;\; (x>1) \end{gather}$$

Boundary Conditions:
$$\begin{gather} \psi_{\pm}(1-0) = \psi_{\pm}(1+0) & \psi'_{\pm}(1-0) = \psi'_{\pm}(1+0) \end{gather}$$

#### Shallow-Well Regime 
$$\begin{gather} U_0 \ll 1  \\ g = -2aU_0 \\ \psi(x) = Be^{-U_0|x|} \;\;\; E =-U_0^2\end{gather}$$
#### Weakly-bound state 

#### Hard Wall Regime (Deep Well)
$$\begin{gather} U_0 \gg 1 & U_0 \gg \frac{\hbar^2}{ma^2}  \end{gather}$$
Has many bound states

Energy: 

$$\begin{gather} \epsilon = U_0 - |E| \\ \psi_+(x) = A\cos(k_+ x) \;\;\; \psi_-(x) = A\sin(k_-x) \;\;\;\; \epsilon = k^2_{\pm} \\ k_n = \frac{\pi}{2}n\end{gather}$$

#### Exact Solution

## Transmission and Reflection
We have a constant of motion: 

$$\begin{gather} I = \int |\psi(x,t)|^2 dx \;\;\;\; \dot I = 0 \end{gather}$$

With which we can define transmission and reflection coefficients: 

$$\begin{gather} T = I_r/I & I_r = \int|\psi_r(x,t)|^2 dx \\ R = I_l/I & I_l = \int |\psi_l(x,t)|^2 dx\end{gather}$$

In quantum mechanics we have $I = 1$ 

Solutions of the form: 

$$\begin{gather} \psi^{(k)}_{\text{transm}}(x,t) = C_ke^{ikx - iE_kt} F(x-v_kt) \\ \psi^{(k)}_{\text{inc}}(x,t) = A_ke^{ikx - iE_kt} F(x-v_kt) \\ \psi^{(k)}_{\text{refl}}(x,t) = B_ke^{-ikx - iE_kt} F(-x-v_kt) \end{gather}$$

$$\begin{gather} T = |C_k|^2/|A_k|^2 & R = |B_k|^2/|A_k|^2 \\ |B_k|^2 + |C_k|^2 = 1 & A_k = 1\end{gather}$$

#### Potential Step
$$\begin{gather} |B_k|^2 + (k'/k)|C_k|^2 = 1 \end{gather}$$