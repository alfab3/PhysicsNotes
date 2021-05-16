Choose the y - axis to be perpendicular to the surface of the Earth, the cable being represented by a curve $y = f(x)$ in the $xy$-plane with the constraint $f(x_a) = y_a$. The potential energy of the element $dl$ is proportional to its height $y$ and its length $dl$. Hence, the total potential energy is given by the integral
$$
U[f] = \int ydl = \int^{x_b}_{x_a} f\sqrt{1+(f_x)^2}dx
$$
We do not care about the units, and thus set the pre-factor equal to unity. We see that $U[f]$ has the form $F[f] = \int^{x_b}_{x_a} g(f,f_x,x)dx$ with
$$
g(f,f_x,x) = f\sqrt{1+(f_x)^2}
$$
Here the function $g$ explicity depends on $f$ and $f_x$, but not on $x$