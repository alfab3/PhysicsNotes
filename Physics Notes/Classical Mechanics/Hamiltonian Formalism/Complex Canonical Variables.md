Unification of the two canonically [[Conjugate Variables]] $(q_j,p_j)$ by introducing a single complex canonical variable $a_j$, such that $$\begin{gather} a_j = \alpha q_j + i\beta p_j \end{gather}$$ where $\alpha$ and $\beta$ are complex numbers. The equations of motion then acquire the form 

$$\begin{gather}i\lambda\dot a_j = \frac{\partial H}{\partial a^*_j}\end{gather}$$

with $$\begin{gather}\lambda = 1/(\alpha\beta^*+\alpha^*\beta) \end{gather}$$ meaning that $$\begin{gather} (\alpha\beta^*+\alpha^*\beta) \neq 0\end{gather}$$

We see that each pair of real equations [[Hamiltonian Function and Hamilton's Equations]] is now replaced with one complex equation. Equivalently, one may use the complex conjugated equation $-i\lambda\dot a_j^* = \partial H/\partial a_j$ (by definition, H is a real-valued function).

In terms of [[Complex Variables]], the expression for [[Poisson Brackets]] reads:

$$\begin{gather}\{A,B\} = (i/\lambda)\sum_j\left[\frac{\partial A}{\partial a_j}\frac{\partial B}{\partial a^*_j}-\frac{\partial A}{\partial a^*_j}\frac{\partial B}{\partial a_j}\right] \end{gather}$$

A mathematical remark is in order here. In the definition of Poisson Brackets and $\lambda$ we use the notion of a partial derivative with respect to a complex variable. For a function $F(z,z^*)$ of the complex variable $z = z' + iz''$, the partial derivatives $\partial/\partial z$ and $\partial/\partial z^*$ are defined as:

$$\begin{gather}\frac{\partial}{\partial z} = \left(\frac{\partial}{\partial z'} - i \frac{\partial}{\partial z''}\right)\frac{1}{2} \\ \frac{\partial}{\partial z^*} = \left(\frac{\partial}{\partial z'} + i \frac{\partial}{\partial z''}\right)\frac{1}{2} \end{gather}$$

The reason for introducing these is that with respect to these operations the variables $z$ and $z^*$ are considered as independent.

Going from a complex canonical variable $a_j$ to a canonical pair $(q_j,p_j)$ is straightforward. Complex conjugating our canonical variable we get:

$$\begin{gather} a^*_j = \alpha^* q_j - i\beta^* p_j \end{gather}$$

Using the combination of this new form and the conjugate we get:
$$\begin{gather} q_j = \lambda(\beta a_j^*+\beta^*a_j) \\ p_j = i\lambda(\alpha a_j^*-\alpha^*a_j)\end{gather}$$ 

We can rescale $\lambda$ by setting $\alpha$ and $\beta$ in such a way then $\lambda = 1$ and our equations become:

$$\begin{gather} q_j = \beta a_j^*+\beta^*a_j \\ p_j = i(\alpha a_j^*-\alpha^*a_j)\end{gather}$$ 
