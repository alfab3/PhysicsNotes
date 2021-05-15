Let $F[a,b]$ be the set of $\mathbb{C}$ - valued functions defined on the real interval $[a,b)$. $F[a,b]$ is a infinite dimensional vector space. 

To see this consider for instance the case $[a,b] = [0,1]$, and divide the interval as follows

Region 0 is the point $x = 0$
Region 1 is the point $x = 1$
Region 2 is the region $0 < x < \frac{1}{2}$
Region 3 is the region $\frac{1}{2} < x < \frac{1}{2} + \frac{1}{4}$
Region 4 is the region $\frac{1}{2} + \frac{1}{4} < x < \frac{1}{2} + \frac{1}{4} + \frac{1}{8}$
...

Now, let $f_i(x)$ be non-vanishing only on region $i$. Since any finite subset of $f_i$ is linearly independent, the dimension of the space cannot be finite. 

So let $\{f_i(x)\}$ be an infinite set of functions that provide a basis of $F[a,b]$ then any $\phi \in F[a,b]$ can be decomposed: 

$\phi(x) = \sum^\infty_{i=1} \phi_i f_i(x)$

Where $\phi(x)$ is a vector, $\phi_i$ are the components and $f_i(x)$ are the [[Basis Vectors]]. 

Now we have the problem of defining the convergence of such an infinite sum! But we cannot do this without defuning some sort of "distance" in our function space. 

A measure on the space is called the [[Norm]]