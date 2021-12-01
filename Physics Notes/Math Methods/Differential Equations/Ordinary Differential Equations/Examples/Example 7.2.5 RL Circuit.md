For a resistance-inductance circuit [[Kirchoff's Laws]] leads to 
$$
L\frac{dI(t)}{dt}+RI(t)=V(t)
$$
where $I(t)$ is the current $L$ and $R$ are respectively, constant values of the inductance and resistance, and $V(t)$ is the time-dependent input voltage 
From 
$$
\alpha(x)=\exp\bigg[\int^x p(x)dx\bigg]
$$
our integrating factor $\alpha(t)$ is 
$$
\alpha(t) = \exp \int^t \frac{R}{L}dt=e^{Rt/L}
$$
then 
$$
I(t)=e^{-Rt/L}\bigg[\int^te^{Rt/L}+C\bigg]
$$
With the constant C to be determined by an initial condition 
For the special case $V(t)=V_0$ a constant 
$$
I(t)=e^{-Rt/L}\bigg[\frac{V_0}{L}\frac{L}{R}e^{Rt/L}+C\bigg] = \frac{V_0}{R}+Ce^{-Rt/L}
$$
