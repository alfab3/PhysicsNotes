While nonlinear first-order ODEs can often be solved using the strategies already presented, the situation is different for the linear first-order [[Ordinary Differential Equation]] because procedures exist for solving the most general equation of this type, which we write in the form
$$
\frac{dy}{dx} + p(x)y=q(x)
$$
If our linear first order ODE is exact, its solution is straightforward. If it is not exact we make it exact by introducing an integrating factor $\alpha(x)$, so that the ODE becomes
$$
\alpha(x)\frac{dy}{dx}+\alpha(x)p(x)y=\alpha(x)q(x)
$$
The reason for multiplication by $\alpha(x)$ is to cause the left-hand of the above equation to become a perfect differential, so we require that $\alpha(x)$ be such that 
$$
\frac{d}{dx}[\alpha(x)y]=\alpha(x)\frac{dy}{dx}+\alpha(x)p(x)y
$$
Expanding the left-hand side of the above equation becomes 
$$
\alpha(x)\frac{dy}{dx}+\frac{d\alpha}{dx}y=\alpha(x)\frac{dy}{dx}+\alpha(x)p(x)y
$$
so $\alpha$ must satisfy
$$
\frac{d\alpha}{dx}=\alpha(x)p(x)
$$
This is a separable equation and therefore soluble. Separating the variables and integrating we obtain
$$
\int^\alpha \frac{d\alpha}{\alpha} = \int^x p(x)dx
$$

We need not consider the lower limits of these integrals because they combine to yield a constant that does not affect the performance of the integrating factor and can be set to zero. Completing the evaluation we reach 
$$
\alpha(x)=exp\bigg[\int^xp(x)dx \bigg]
$$
With $\alpha$ now known we proceed to integrate:
$$
\frac{d}{dx}[\alpha(x)y(x)]=\alpha(x)q(x)
$$
which can be integrated (and divided through $\alpha$) to yield 
$$
y(x)=\frac{1}{\alpha(x)}\bigg[\int^x \alpha(x)q(x)dx+C\bigg] \equiv y_2(x)+y_1(x)
$$
The two terms in the above equation have an interesting interpretation. The term $y_1 = C/\alpha(x)$ is the general solution of the homogeneous equation obtained by replacing $q(x)$ with zero. To see this, write the homogeneous equation as 
$$
\frac{dy}{y}=-p(x)dx
$$
which integrates to 
$$
\ln y = -\int^xp(x)dx + C = -\ln\alpha+C
$$
Taking the exponential of both sides and renaming $e^C$ as $C$, we get just $y=C/\alpha(x)$ The other term
$$
y_2 = \frac{1}{\alpha(x)}\int^x\alpha(x)q(x)dx
$$
corresponds to the right-hand side term $q(x)$, and is a solution of the original inhomogeneous equation. We thus have the general solution to the inhomogeneous solution to the inhomogeneous 