In real oscillators([[Harmonic Oscillator]]), [[Friction]], or damping, slows the motion of the system. Due to frictional force, the [[Velocity]] decreases in proportion to the acting frictional force. While in a simple undriven [[Harmonic Oscillator]] the only force acting on the [[Mass]] is the restoring force in a damped harmonic oscillator there is an addition a frictional force which is always in a direction to oppose the motion. In many vibrating systems the frictional force $F_t$ can be modeled as being proportional to the velocity $v$ of the object $F_t = -cv$, where $c$ is called the viscous damping coefficient.

The balance of forces([[Force Newtonian Dynamics]]) for damped harmonic oscillators is then 
$$
F = -kx-c\frac{dx}{dt}=m\frac{d^2x}{dt^2}
$$
$$
\frac{d^2x}{dt^2}+2\xi\omega_0\frac{dx}{dt}+\omega_0^2x=0
$$
where
$$
\omega_0 = \sqrt{\frac{k}{m}}
$$
is called the "undamped angular [[Frequency]] of the oscillator"
$$
\xi = \frac{c}{2\sqrt{mk}}
$$
is called the "damping ratio"

The value of the damping ratio $\xi$ critically determines the behavior of the system. A damped harmonic oscillator
1) Overdamped $\xi > 1$: The sytem returns to steady state without oscillating. Larger values of the damping ration $\xi$ return to equilibrium more slowly
2) Critically damped $\xi = 1$: The system returns to steady state as quickly as possible without oscillating. This is oftern desired for the damping of system such as doors
3) Underdamped $\xi < 1$: The system oscillates with the amplitude gradually decreasing to zero. The angular frequency of the underdamped harmonic oscillator is given by $\omega_1 = \omega_0\sqrt{1-\xi^2}$, the exponential decay of the underdamped harmonic oscillator is given by $\lambda = \omega_0\xi$
