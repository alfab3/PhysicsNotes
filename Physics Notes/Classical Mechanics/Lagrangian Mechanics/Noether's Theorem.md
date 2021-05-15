The time-independence of the first integral 
$$
\frac{d}{dt}\{\dot{q}\frac{\partial L}{\partial \dot{q}}-L\} = 0
$$
and of angular momentum
$$
\frac{d}{dt}\{mr^2\dot{\theta}\} = 0
$$
are examples of conservation laws. We obtained them both by manipulating the Euler-Lagrange equations of motion, but also indicated that they were in some way connected with symmetries. One of the chief advantages of a variational formulation of a physical problem is that this connection can be made explicity by exploting a strategy due to Emmy Noether. She showed how to proceed directly from the action integral to the conserved quantity without having to fiddle about with the individual equations of motion. We begin by illustrating her technique in the case of angular momentum, whose conservation is a consequence the rotational symmetry of the central force problem. The action integral for the central force problem is

$$
S = \int^T_0 \{\frac{1}{2}m(\dot{r}^2+r^2\dot{\theta}^2-V(r)\}dt
$$

Noether observes that the integrand is left unchanged if we make the variation 
$$
\theta(t) \rightarrow \theta(t) + \epsilon \alpha
$$
where $\alpha$ is a fixed angle and $\epsilon$ is a small, time independent, paramater. This invariance is the symmetry we shall exploit. It is a mathematical identity: it does not require that $r$ and $\theta$ obey the equations of motion. She next observes that since the equations of motion are equivalent to the statement that S is left stationary under any infinitesimal variations in $r$ and $\theta$, the necessarily imply that S is stationary under the specifc variation 
$$
\theta(t)\rightarrow\theta(t)+\epsilon(t)\alpha
$$
where now $\epsilon$ is allowed to be time-dependent. This stationarity of the action is no longer a mathematical identity, but, because it requires $r$, $\theta$ to obey the equations of motion has physical content. Inserting $\delta \theta = \epsilon(t)\alpha$ into our expression for $S$ gives
$$
\delta S = \alpha \int^T_0\{mr^2\dot{\theta}\}\dot{\epsilon} dt
$$
Note that this variation depends only on the time dericative of $\epsilon$ and not $\epsilon$ itself. This is because of the invariance of $S$ under time-independent rotations. We now assume that $\epsilon(t) = 0$ at $t = 0$ and $t=T$, and integrate by parts ti take the time derivative off $\epsilon$ and put it on the rest of the integrand:
$$
\delta S = -\alpha\int\{\frac{d}{dt}(mr^2\dot{\theta}\}\epsilon(t)dt
$$
Since the equations of motion say that $\delta S = 0$ under all infinitetesimal variations, and in particular those due to any time-dependent rotation $\epsilon(t)\alpha$, we deduce that the equations of motion imply that the coefficient of $\epsilon(t)$ must be zero, and so, provided $r(t), \theta(t)$ obey the laws of motion we have
$$
0=\frac{d}{dt}(mr^2\dot{\theta})
$$
As a second illustration we derive energy (first integral) conservation for the case that the system is invariant under time translations - meaning that $L$ does not depend explicity on time. In this case the action integral is invariant under constant time shifts $t \rightarrow t + \epsilon$ in the argument of the dynamical variable: 
$$
q(t)\rightarrow q(t + \epsilon) \approx q(t)+\epsilon\dot{q}
$$
The equations of motion tell us that the action will be stationary under the variation 
$$
\delta q(t) = \epsilon(t)\dot{q}
$$
where again we now permit the parameter $\epsilon$ to depend on $t$. We insert this variation into 
$$
S = \int^T_0Ldt
$$
and find 
$$
\delta S = \int^T_0\{\frac{\partial L}{\partial q}\dot{q}\epsilon + \frac{\partial L}{\partial \dot{q}}(\ddot{q}\epsilon + \dot{q} \dot{\epsilon})\}dt
$$
This expressopm contains undotted $\epsilon$'s