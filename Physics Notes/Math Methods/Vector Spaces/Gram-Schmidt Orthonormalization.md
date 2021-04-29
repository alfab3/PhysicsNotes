Suppose you're given $\ket{\psi_1}$ and then you choose a vector $$\ket{\phi_1} = \frac{\ket{\psi_1}}{||\psi_1||} = \frac{\ket{\psi_1}}{\braket{\psi_1|\psi_1}^{1/2}}$$ 

Then you take the second vector $$\frac{\ket{\psi_2} - \braket{\phi_1 | \psi_2}\ket{\phi_1}}{||\ket{\psi_2} - \braket{\phi_1 |\psi_2}\ket{\psi_1}||} = \ket{\phi_2}$$

So this will guarantee: 
$$\braket{\phi_1|\phi_1} = 1 = \braket{\phi_2|\phi_2}$$
and
$$\braket{\phi_1 | \phi_2} = 0$$

Qualitatively, you are given some vector $\ket{\psi_1}$ and you divide by its norm to create the vector $\ket{\phi_1}$ which is the unit vector. Then you have some vector $\ket{\psi_2}$ and you take the dot product of $\ket{\psi_2}$ and $\ket{\phi_1}$ with $\ket{\phi_1}$ on the left hand side. Which essentially is the projection of $\ket{\psi_2}$ and you subtract it off. Then you normalize the vector to get the unit vector which is $\phi_2$.

$$\ket{\psi} = [\ket{\phi}\bra{\phi}]\ket{\psi} = \ket{\phi} \braket{\phi|\psi} = \braket{\phi|\psi}\ket{\phi}$$

So it's a coefficient multiplied by a (unit) vector.  If you have $\ket{\psi}\bra{\psi}$, this is called the [[Projection Operator]].