Linear 1st order PDEs can be considered the most basic example of conservation law: 

$$\begin{gather} \frac{\partial u}{\partial t} = -\frac{\partial}{\partial x} J(u) \end{gather}$$ or more generally:

$$\begin{align} \frac{\partial u}{\partial t} = - \vec \nabla\vec J(u) \end{align}$$

Where $J(u)$ is a linear function of $u$. This means that when considering the total value of $u$ on any interval $(x_1,x_2)$

$$\begin{gather} u_{\text{tot}}(t) = \int^{x_2}_{x_1}u(x,t)dx \end{gather}$$

then the only way to change $u_{\text{tot}}$ is by if $J\Bigg|_{x_2} \neq J\Bigg|_{x_1}$

(namely there is a net flux of $u$ into or out from the interval $(x_1,x_2)$)

Note that "conservation law" doesn't mean that $u_{\text{tot}}(t)$ is constant in time. It only means what was said above that $u_{\text{tot}}$can change only by net [[Flux]] through the boundaries.

(contrast with $\frac{\partial u}{\partial t} = -\alpha u - \frac{\partial J(u)}{\partial x}$ for which $u_{\text{tot}}$ in $(x_1,x_2)$ changes over time (dissipation if $\alpha > 0$) even though $J\Bigg|_{x_1} =J\Bigg|_{x_2}$

Conservation laws are extremely ubiquitous and important in Physics. They often involve [[Vector Field]]s (e.g. momentum) where the current becomes a Tensor ([[Math Methods/Vector Spaces/Tensor]])  $$\begin{gather} \frac{\partial \vec p}{\partial t} = - \vec \nabla \overleftrightarrow{\sigma} \\ 
\frac{\partial p_i(\vec x)}{\partial t} = -\frac{\partial}{\partial x_j}\sigma_{ij}\end{gather}$$

where $\sigma_{ij}$ is a linear or nonlinear function of $\vec p(\vec{x}),\vec x$ and possibly other fields.

Generalization to a type of conservation law to a class of non-linear problems called quasi-linear of the form:

$$\begin{gather} \frac{\partial u}{\partial t} + b(u,x,t)\frac{\partial}{\partial x} J(u,x,t) = q(u,x,t)\end{gather}$$

Where: $b(u,x,t)$ is a coefficient $J(u,x,t)$ is a current and $q(u,x,t)$ is the source.

The crucial feature of this type of equation is that the coefficients, current, and source may be any function of the [[Scalar Field]] $u(x,t)$ itself but not of its spatial or temporal [[Derivative]]s.

It can be shown that the method of characteristics can be generalized also to this class of problem such that the nonlinear PDE can be converted to a ($\infty$ - set of) ODEs.

Here we will discuss the simplest version such family: 

$$\begin{gather} \frac{\partial u}{\partial t} + \frac{\partial}{\partial x}J(u) = 0\end{gather}$$

### Physical example: "traffic model"

Assume $u(x,t)$ is the density of cars moving in a one-way highway. In the absence of accidents the number of cars at any interval $$\begin{gather} N(t) = \int^{x_2}_{x_1} u(x,t) dx \end{gather}$$ 
can change only if the number of cars that enter the interval at $x_1$ is different from $x_2$, Hence we expect $u(x,t)$ to be described by the above PDE, where the current $\vec J = J \hat{x}$ is the number of cars that cross a point per unit time.

That is $J(x,t) \equiv u(x,t) \cdot v(x,t)$ where $v(x,t)$ is the average speed of cars at point $x$ at time $t$$(\vec v(x,t) = v(x,t)\hat{x})$ Note that the current $\vec J$ is a vector obtained as a product of scalar (density) and vector (velocity) field, similarly to momentum.

To complete the model we need to provide some phenomenological law for the speed in terms of the other fields on the problem. In our simple traffic model this means that we have to provide a model for the speed $v$ in terms of the car density $(u)$ as well as the location $(x)$ and time $(t)$.

$$\begin{gather} v = v(u,x,t)\end{gather}$$

Where $u$ is the effect of density on speed, $x$ is the effect of location on speed, $t$ is effect of time. 

Again focusing on the simplest case let us assume that $v$ is fully determined by the car density:

we see that even the simplest realistic model give $v(u) \neq \text{const}$, such that $J(u) = u v(u)$ is a nonlinear function of $u$ and consequently: 

$$\begin{gather} J'(u) = \alpha - \beta u \neq const \end{gather}$$

Now let us return to our PDE $$\begin{gather} \frac{\partial u}{\partial t} + \frac{\partial}{\partial x}J(u) = 0 \end{gather}$$
and write it as: 
$$\begin{gather}\frac{\partial u}{\partial t} + J '(u) \frac{\partial u}{\partial x} =0  \end{gather}$$
we readily see that we can repeat the characteristic trick and convert the PDE into a set of ODE's: 
$$\begin{gather} \frac{dx_c}{dt}=J'(u_c(t)) \\ \frac{du_c}{dt} = \frac{\partial u_c}{\partial t} + \frac{\partial u_c}{\partial x}\frac{d x_c}{dt} = 0 \\ \Rightarrow u_c(t) = u_c(0) = u(x_c(0),0)\end{gather}$$

Namely the characteristics are straight lines in the $(x,t)$ plane, whose slopes are determined by the initial conditions $u(x, t=0)$

Before discussing the nature of such solutions let us not a profound difference from the linear problem we could construct the characteristic in advance, i.e. by inspecting the equation itself, without paying attention to any particular solution. Specifically we could determine whether there are any weird phenomena (caustics) independently on the initial conditions.

For the nonlinear problem, this is not possible. Namely the construction of characteristics has to be done simultaneously with constructing the solution.