Suppose we have a smooth line in the $xy$-plane passing through two given points, $(x_a,y_a)$ and $(x_b,y_b)$ and specified by the equation 
$$
y = f(x)
$$
The length of the line is a functional of $f$ of the form. Indeed
$$
l[f] = \int dl = \int \sqrt{(dx)^2+(dy)^2} = \int \sqrt{(dx)^2+(f_xdx)^2} = \int^{x_b}_{x_a} \sqrt{1+(f_x)^2}dx
$$

We see that $l[f]$ has the form:
$$
g(f,f_x,x) = \sqrt{1+(f_x)^2}
$$
In this example, the function g does not depend explicitly of f and x, which reflects two translational symmetries: $f\rightarrow f+ \;const$ and $x\rightarrow x + \;const$