Here is an isobaric [[Ordinary Differential Equation]]
$$
(x^2-y)dx+xdy=0
$$
Assigning $x$ weight 1, and $y$ weight $m$. the term $x^2dx$ has weight 3; the other two terms have weight $1+m$. Setting $3 = 1 +m$, we find that all terms can be assigned equal weight if we take $m=2$. This means that we should make the substitution $y=x^2v$. Doing so, we get
$$
(1-v)dx + xdv = 0
$$
which separates into 
$$
\frac{dx}{x}+\frac{dv}{v+1}=0 \rightarrow\ln x + \ln (v+1) =\ln C \; or \; x(v+1)=C
$$
From this, we get $v=\frac{C}{x}-1$. Since $y=x^2v$, the ODE has solution $y=Cx-x^2$
