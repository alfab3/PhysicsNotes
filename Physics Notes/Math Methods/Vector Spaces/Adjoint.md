Let $L$ be a linear operator on $V$, $L:V \rightarrow V$. We define the adjoint $L^\dagger$ as a nother linear operator $L^\dagger:V \rightarrow V$ defined as $$L^\dagger \ket{v} = (\bra{v}L)^\dagger$$ 

So $L^\dagger$ is really an operator $V^* \rightarrow V^*$.

By construction, then 
$$(L^\dagger\ket{x})^\dagger = \bra{x}L = \braket{L^\dagger \ket{x}, \ket{y}} = \braket{x |L| y } = \braket{\ket{x}, L\ket{y}} $$

Also 
$$\braket{x | L | y}^* = \braket{L^\dagger \ket{x}, \ket{y}}^* = \braket{\ket{y}, L^\dagger \ket{x}} = \braket{y|L|x}$$ 

Using components, finally, one can show $(L^\dagger)^\dagger = L$

An operator $L$ is Self-Adjoint if $L^\dagger = L$