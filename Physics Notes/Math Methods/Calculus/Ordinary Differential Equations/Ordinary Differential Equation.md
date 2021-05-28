An ordinary differential equation (ODE) is an equation that involes one or more unknown functions of a single variable as well as their [[Derivative]] up to a finite order. For a single unknown $y(t)$, the ODE takes the general form: 
$$F(y(t), \; y'(t), \;..., \;y^{(n)}(t); \;(t)) = 0$$
where $n$ is the order of the ODE. 

The ODE is explicit if it takes the form: 
$$y^{(n)}(t) = G(y(t), \; y'(t), \;..., \;y^{(n)}(t); \;(t))$$
otherwise it is implicit. ([[Explicit vs Implicit Solution]]).

An $n-th$ order ODE can be rewritten as a system of $n$ first order ODEs as follows: 
define: $$y_i(t) = y^{i-1} \;\;\; i = 1, ..., n$$
So that:
$$y_i(t) = y(t); \; \; y_1'(t) = y_2(t); \; \; y_2'(t) = y_3(t)$$

and finally:
$$y_n'(t) = G(y_0(t), y_1(t),...,y_n(t);t)$$

