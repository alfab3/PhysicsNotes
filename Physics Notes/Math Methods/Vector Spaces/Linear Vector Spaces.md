Contains a set of elements ("[[Vectors]]"), using notation - $\ket{\psi},\ket{\phi},\ket{\chi} \in V$. Among which there are operations:

### Axioms
Addition - $\ket{\psi} + \ket{\phi} \in V$
Associative Addition - $(\ket{\psi} + \ket{\phi}) + \ket{\chi} = \ket{\psi} + (\ket{\phi}+\ket{\chi})$
Commutative Addition - $\ket{\psi} + \ket{\phi} \in V, \ket{\phi} + \ket{\psi} \in V$
Scalars - $a,b,c,d,... \in  F$(some field) such that $a\ket{\psi} \in V$ or $a(b\ket{\psi}) = (ab)\ket{\psi}$
Null vector -  $\ket{0}$
$1\ket{\phi} = \ket{\phi}$
$0\ket{\phi} = \ket{0}$

### From these [[Axioms]] the following theorems can be proved:
a) $\ket{0}$ is unique [[Uniqueness]]
Proof: 
Suppose $\ket{0}, \ket{0'}$ both satisfy axiom 3
Then: $$\ket{0} = \ket{0'} + \ket{0} = \ket{0} + \ket{0'} = \ket{0'} $$
b) $\forall\ket{\nu} \in V, \ket{\nu}$ is unique
Proof:
Let $\ket{u}$ and $\ket{v}$ be elements of a vector space $V$. Then there exists a unique element $\ket{x}$ of $V$ satisifying $\ket{x} + \ket{v} = \ket{u}$
The vector space axioms ensure the existence of an element $\ket{v}$ of $V$ with the property $\ket{v} + \ket{-v} =0$, where 0 is the zero element of $V$. The identity $\ket{x} + \ket{v} = \ket{u}$ is satisfied when $\ket{x} = \ket{-v} + \ket{u}$ since
$$
(\ket{u} + \ket{-v}) + \ket{v} = \ket{u} + (\ket{-v} + \ket{v}) = \ket{u} + 0 = \ket{u}
$$
If now $\ket{x}$ is any element of $V$ satisfying $\ket{x} + \ket{v} = \ket{u}$
c) $\forall \ket{\nu} \in V, 0 \cdot \ket{\nu} = \ket{0}$
Proof:
Let $V$ be a Vector space over a field $K$. Then c0=0 and 0$\ket{v}$ =0 for all 

d) $\forall \lambda \in F, \lambda \cdot \ket{0} = \ket{0}$
e) if $\lambda \cdot \ket{\nu} = \ket{0}$ then $\lambda = 0$ or $\ket{\nu} = 0$
f) $\forall \ket{\nu} \in V, -1 \cdot \ket{\nu} = \ket{-\nu}$

From b) we can define the difference of two vectors $\ket{v} -\ket{w}$ as the sum of $\ket{v}$ with the additive inverse of $\ket{w}$
$$\ket{v} - \ket{w} = \ket{v} + \ket{-w}$$

Functions defined on a given intercal form a vector space, with operations defined as $$(f+g)(x) = f(x) + g(x), (df)(x)=df(x)$$

2 important properties of orthonormal basis ([[Basis Set]]) in Linear Vector Spaces. The first is orthonormality: 
$$\braket{\phi_i | \phi_j} = \delta_{ij}$$

and a set of [[projection operator]]s: 
$$\sum_n \ket{\phi_n} \bra{\phi_n} = \mathbb{I}$$ 
which is known as completeness. 

For example let's look at a 2 Dimensional LVS.
$$\ket{\phi_1} = 
\begin{bmatrix}
	1 \\
	0
\end{bmatrix}, \;
\ket{\phi_2} = 
\begin{bmatrix}
	0 \\
	1
\end{bmatrix}$$

$$\ket{\phi_1}\bra{\phi_1} = 
\begin{bmatrix}
	1 \\
	0
\end{bmatrix} [1, 0] = 
\begin{bmatrix}
	1 \; \; 0\\
	0 \; \; 0
\end{bmatrix}$$

$$\ket{\phi_2}\bra{\phi_2} = 
\begin{bmatrix}
	0 \\
	1
\end{bmatrix} [0, 1] = 
\begin{bmatrix}
	0 \; \; 0\\
	0 \; \; 1
\end{bmatrix}$$
So this follows our properties, if we take:
$$\ket{\phi_1}\bra{\phi_2} = 
\begin{bmatrix}
	0 \; \; 1\\
	0 \; \; 0
\end{bmatrix}$$
and accordingly: 
$$\ket{\phi_2}\bra{\phi_1} = 
\begin{bmatrix}
	0 \; \; 0\\
	1 \; \; 0
\end{bmatrix}$$

If we write: 
$$\begin{bmatrix}
	a \; \; b\\
	c \; \; d
\end{bmatrix}$$
This is an operator and 2x2 matrix in 2 dimensional space is an operator. This is short hand for: 
$$A = \begin{bmatrix}
	a_{11} \; \; a_{12}\\
	a_{21} \; \; a_{22}
\end{bmatrix} 
= a_{11} \begin{bmatrix}
	1 \; \; 0\\
	0 \; \; 0
\end{bmatrix}
+ a_{12}\begin{bmatrix}
	0 \; \; 1\\
	0 \; \; 0
\end{bmatrix}
+ a_{21}\begin{bmatrix}
	0 \; \; 0\\
	1 \; \; 0
\end{bmatrix} 
+ a_{22}\begin{bmatrix}
	0 \; \; 0\\
	0 \; \; 1
\end{bmatrix}
= a_{11} \ket{\phi_1} \bra{\phi_1} + a_{12} \ket{\phi_1} \bra{\phi_2} + a_{21} \ket{\phi_2} \bra{\phi_1} + a_{22} \ket{\phi_2} \bra{\phi_2}$$

You can also write these terms: 
$$ a_{11} \ket{\phi_1} \bra{\phi_1} = \ket{\phi_1} a_{11} \bra{\phi_1}$$

To find $a_{11}$: 
$$a_{11} = \bra{\phi_1} A \ket{\phi_1} $$
This is called a matrix element. 

Given our properties of the orthonormal bais any vector $\ket{\psi}$ can be expanded uniquely in the form $\ket{\psi} = \sum_n c_n \ket{\phi_n}$.

Any operator A can be expanded in the form: 
$$A = \sum_{n,m} A_{n,m} \ket{\phi_n} \bra{\phi_m}$$
