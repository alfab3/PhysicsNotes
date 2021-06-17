We want to find the velocity of a falling parachutist as a function of time and are particularly interested in the constant limiting velocity, $v_0$, that comes about by air drag, taken to be quadratic, $-bv^2$, and opposing the force of the gravitational attraction $mg$, of the Earth on the parachutist. we chose a coordinate system in which the positive direction is downward so that the gravitational force is positive. For simplicity we assume that the parachute opens immediately, that is, at time $t=0$, where $v(t)=0$, our initial condition. 
Newton's law applied to the falling parachutist gives 
$$
m\dot{v}=mg-bv^2
$$
where $m$ includes the mass of the parachute.

The terminal velocity, $v_0$ can be found from the equation of motion as $t\rightarrow\infty$; when there is no acceleration, $\dot{v}=0$ and 
$$
bv_0^2 = mg, \; or \;v_0=\sqrt{\frac{mg}{b}}
$$

Rewriting our equation from newton's law: 
$$
\frac{m}{b}\dot{v}=v_0^2-v^2
$$

This equation is separable, and we write it in the form 
$$
\frac{dv}{v_0^2-v^2} = \frac{b}{m}dt
$$
Using partial fractions to write
$$
\frac{1}{v_0^2-v^2}=\frac{1}{2v_0}\bigg( \frac{1}{v+v_0}-\frac{1}{v-v_0}\bigg)
$$
it is straightforward to integrate both sides: 
$$
\frac{1}{2v_0}\ln\frac{v_0+v}{v_0-v}=\frac{b}{m}t
$$
Solving for the velocity we have
$$
v = \frac{e^{2t/T}-1}{e^{2t/T}-1}v_0=v_0\frac{\sinh(t/T)}{\cosh(t/T)} = v_0\tanh\bigg(\frac{t}{T}\bigg)
$$
where $T=\sqrt{m/gb}$ is the time constant governing the asymptotic approach of velocity to its limiting value, $v_0$. 

