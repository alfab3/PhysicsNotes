[[Ordinary Differential Equation]] are differential equations for functions of a single variable: $$\begin{gather} y''(x) = y(x)^2+3(x) \end{gather}$$

ODE's may be linear:

$$\begin{gather} y'''=(x)=4y''(x) + 2x^2y'(x) + 7\sin x \end{gather}$$

or nonlinear:

$$\begin{align} y'(x) = y^2(x)\end{align}$$

ODE's may be homogeneous or non-homogeneous

$$\begin{gather}\text{homogeneous}\\ y'''(x) + 7x^3 y''(x)+3\sin^2xy'(x)+15x^8y(x) = 0\\ \text{nonhomogeneous}: \\y'(x) = x^2\end{gather}$$

ODE's may be with constant (uniform coefficients) or non-uniform
$$\begin{gather}y'''(x) + 3y''(x)+2y'(x)+y(x) = 0\;\;(\text{uniform}) \\ y'(x) + 3xy(x) = 0 \;\; (\text{non-uniform})\end{gather}$$

The rank of the ODE is the highest derivative in the ODE. The rank determines the number of (linearly-independent) "initial" or "boundary" conditions that must be provided for obtaining a unique solution.

For linear ODE's to order $n$ the general solution may be expressed as $$\begin{gather} y(x) = a_1y_1(x)+ ... + a_ny_n(x) + y_{non-homegenous}(x)\end{gather}$$

where:
$\{y_1(x),...y_n(x)\}$ are independent solutions to the homogeneous equation and $y_{non-hom(x)}$ is a specific solution to the non-homogeneous equation

For linear ODE's with constant (uniform) coefficients the general solution is $$\begin{gather} y(x) = \sum^n_{j=1} a_ne^{\lambda_n x} \end{gather}$$

Where $\lambda_n$ may be complex

The above properties apply also to PDE's However things become somewhat complicated due to the presence of few variables.

