From [[Kirchoff's Laws]] the current $I$ in an [[RC Circuit]] obeys the equation 
$$
R\frac{dI}{dt}+\frac{1}{C}I=0
$$
Find $I(t)$
$$
\frac{dI}{dt}+\frac{1}{RC}I=0
$$
$$
\frac{dI}{I}+\frac{1}{RC}dt=0
$$
$$
\int^I_{I_0} \frac{dI}{I} + \frac{1}{RC}\int^t_{t_0}dt = 0
$$
$$
\ln(I)\bigg|^I_{I_0}+\frac{1}{RC}t\bigg|^t_{t_0} = 0
$$
$$
\ln(I)-\ln(I_0)+\frac{1}{RC}[t-t_0]
$$
We can just say that $t_0 \rightarrow 0$
$$
\ln\bigg(\frac{I}{I_0}\bigg)+\frac{t}{RC}=0
$$
$$
\frac{I}{I_0}+e^{t/RC}=0
$$
$$
\frac{I}{I_0}=e^{-t/RC}
$$
$$
I=I_0e^{t/RC}