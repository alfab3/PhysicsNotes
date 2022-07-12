One of the most common problems in physics is the harmonic oscillator. In fact, quantum field theory considers every point in space to have its own oscillators for every type of quantum field. We begin with a single oscillator with the Hamiltonian
$$\begin{gather} H = \frac{\mathcal P^2}{2m}+\frac{m\omega^2}{2}\mathcal X^2 \end{gather}$$
where the spring constant is expressed in terms of a [[Frequency]] $\omega,k=m\omega^2$. Here, $\mathcal X$ and $\mathcal P$ are operators. 

Dirac's solution solution to the problem involves first defining two new operators $$\begin{gather} a \equiv \sqrt{\frac{m\omega}{2\hbar}}\mathcal X + i\sqrt{\frac{1}{2\hbar m\omega}}\mathcal P, \; a^\dagger = \sqrt{\frac{m\omega}{2\hbar}}\mathcal X - i\sqrt{\frac{1}{2\hbar m \omega}}\mathcal P \end{gather}$$
The operators are known as the annihilation (or destruction) and creation operators respectively ([[Creation and Annihilation Operators]]) for reasons to be seen below. In some texts, these operators are referred to as ladder operators. 

The operators satisfy simple commutation relations,

$$\begin{gather} [a,a^\dagger] = 1 \end{gather}$$
Then the [[Hamiltonian]] can be written as:
$$\begin{gather} H = \hbar \omega\left(a^\dagger a + \frac{1}{2}\right) \end{gather}$$
To see that the creation operator does exactly what it sounds like, consider an [[Eigenstate]] of the Hamiltonian such that 

$$\begin{gather} a^\dagger a\ket{n} = n \ket{n} \end{gather}$$
At this point we do not know that the [[Eigenvalues]], $n$ of $a^\dagger a$ are integers. By using the commutation relation: 

$$\begin{gather} aa^\dagger = a^\dagger a+ 1 \\ a^\dagger a(a^\dagger \ket{n}) = a^\dagger(a^\dagger a+1)\ket{n} = (n+1)a^\dagger\ket{n}\end{gather}$$

by commuting $a^\dagger$ to the far left. Doing the same with the state $a\ket{n}$ one find:

$$\begin{gather} a^\dagger(a\ket{n}) = (n-1)(a\ket{n}) \end{gather}$$

Then up to a normalization constant: 

$$\begin{gather} a^\dagger\ket{n} \propto \ket{n+1}, & a\ket{n}\propto \ket{n-1} \end{gather}$$

With the normalization:

$$\begin{gather}  a^\dagger\ket{n} = \sqrt{n+1}\ket{n+1} & a\ket{n} = \sqrt{n}\ket{n-1}\end{gather}$$

The operator $a^\dagger a$ is referred to as the number operator and because that energy must not have arbitrarily small negative values, the values of $n$ cannot be arbitrarily negative. Thus the sequence of repeatedly applying the operator $a$ to some state $n$ must terminate at some point. This only happens if there is a state with $n = 0$ 

$$\begin{gather} a\ket{n=0}=0 \end{gather}$$

Which constrains all the $n$ to be integers. With the constraint that $n$ is an integer, the normalization can be expressed as 

$$\begin{gather} (a^\dagger)^ n\ket{0} = \sqrt{n!}\ket{n}
\end{gather}$$

The eigenenergies are

$$\begin{gather} E_n = (n+1/2)\hbar \omega \\ n = 0,1,2 ... \end{gather}$$

It is straight-forward to find the ground state [[Wave function]] if one is sufficiently prescient to guess that the form of the solution is a Gaussian with some as yet undetermined width $b$

$$\begin{gather} \psi_0(x) = e^{-x^2/(2b^2)} \end{gather}$$

To show that this is a solution we first take derivative with respect to $x$. 

$$\begin{gather} \frac{d}{dx}\psi_0(x) = -\frac{x}{b^2}\psi_0(x), & \frac{d^2}{dx^2}\psi_0(x) = \frac{x^2}{b^4}\psi_0(x) - \frac{1}{b^2}\psi_0(x)\end{gather}$$
Plugging into the [[Schrodinger Equation]]: 

$$\begin{gather} -\frac{\hbar^2}{2m} \left(\frac{x^2}{b^4}-\frac{1}{b^2}\right) \psi_0(x) + \frac{m\omega^2x^2}{2} \psi_0(x) = E\psi_0(x)  \end{gather}$$
allows one to determine $b$ and $E$ by inspection 

$$\begin{gather} b = \sqrt{\frac{\hbar}{m\omega}}, & E = \frac{1}{2}\hbar\omega  \end{gather}$$

One may also calculate the normalization $Z$ by enforcing the constraint 

$$\begin{gather} \psi_0(x) = Z^{-1/2}e^{-x^2}, Z = \int^\infty_{-\infty}dx \ e^{-x^2/b^2} \end{gather}$$
Gives: $z = (\pi^1/2 b)$ 

# N - dimensional problem
$$\begin{gather} H\Psi = -\frac{\hbar^2}{2m}\frac{d^2}{dx_1^2}\Psi - \frac{\hbar^2}{2m}\frac{d^2}{2x^2_n} \Psi 
 + \frac{m\omega^2}{2}x_1^2\Psi + \frac{m\omega^2}{2}x_2^2\Psi\ldots+\frac{m\omega^2}{2}x_n^2\Psi \end{gather}$$
 The solution is of the form:
 $$\begin{gather} \Psi(x_1,x_2,\ldots x_n) = \psi_1(x_1)\psi_2(x_2) \cdots\psi_n(x_n) \end{gather}$$
 where $\psi_i$ are the solutions to the 1d Schrodinger equation with [[Eigenenergies]] $\hbar \omega(n_i + 1/2)$ with the ground state energy being for $n = 0$, $E_0 = \hbar\omega/2$. For a 3D Oscillator one can consuder the $x,y,z$ motion as 3 separate oscillators, and the ground state energy would be $3\hbar\omega/2$ 