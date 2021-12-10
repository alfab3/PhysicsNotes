# Method of Characteristics

### First Order
Suppose we have a linear first-order partial differential equation

$$\begin{gather} a(x,y) \frac{\partial u}{\partial x} + b(x,y)\frac{\partial u}{\partial y} + c(x,y)u = f(x,y) \end{gather}$$

Coefficients given by the characteristic curves:

$$\begin{gather} \frac{dx_c}{ds} = a(x,t), & \frac{dt_c}{ds}  = b(x,t)\end{gather}$$

Which give us: 

$$\begin{gather} x_c(s) = x_0 + \int^S_{S'=0} a(x_c(s'),t_c(s'))ds' \\ y_c(s) = y_0 + \int^S_{S'=0} b(x_c(s'),t_c(s'))ds' \end{gather}$$

### Algorithm to Solve
1) Establish your ODEs based on the coefficients
2) Solve the ODEs to find the solutions of the characteristic curves, any constants of integration should be considered the initial condition of that characteristic value.
3) Solve the ODE of the non-homogeneous source term (in our above example the term coupled to c)
4) Plug your characteristic into your nonhomogeneous source solution
5) If initial conditions are given, plug those in to your initial constants

### For Traffic Model:
For a given flux: 
$$\begin{gather} J(\rho) = -\rho^2 \to \frac{\partial J}{\partial x} = \frac{dJ}{dp}\frac{\partial \rho}{\partial x} = -2\rho\frac{\partial \rho}{\partial x}\end{gather}$$