Observable in quantum mechanics as we have just seen in the [[THE UNCERTAINTY PRINCIPLE|uncertainty principle]] cannot be represented by numbers and so we have to find another mathematical tool to represent them. This type of tool is called *Hermitian Operator*. Those types of operators are part of [[HILBERT SPACE|Hilbert space]].

The expectation value of a general observable $Q$ is expressed as such:
![[Screenshot_20241004_110540.png]]

Now even if the observable could not be represented by a value it's expectation value has to be a real value so it follows the property:
![[Screenshot_20241004_110900.png]]
If the complex conjugate of the operator does not change it follows also that
you can change the order of operation on the wave function $\psi$:
![[Screenshot_20241004_111318.png]]

## Definition of a Hermitian Operator

An operator $\hat{A}$ is **Hermitian** if it satisfies the following condition for all vectors $|\psi\rangle$ and $|\phi\rangle$ in a Hilbert space:

$$
\langle \psi | \hat{A} \phi \rangle = \langle \hat{A} \psi | \phi \rangle
$$

This equation expresses that the operator is equal to its **adjoint** (what we have discussed previously with the complex conjugate of $Q$), meaning:

$$
\hat{A}^\dagger = \hat{A}
$$

Where $\hat{A}^\dagger$ denotes the adjoint of $\hat{A}$, which is the complex conjugate transpose of $\hat{A}$.

## Key Properties of Hermitian Operators

1. **Real Eigenvalues**: If $\hat{A}$ is Hermitian, all of its [[EIGENVALUES AND EIGENFUNCTIONS|eigenvalues]] are real. This is important because in quantum mechanics, the eigenvalues of Hermitian operators represent measurable physical quantities, which must be real numbers.

2. **Orthogonality of Eigenvectors**: The eigenvectors corresponding to different eigenvalues of a Hermitian operator are orthogonal. This means if $|\psi_1\rangle$ and $|\psi_2\rangle$ are eigenvectors of $\hat{A}$ with different eigenvalues, then:
   $$
   \langle \psi_1 | \psi_2 \rangle = 0
   $$

3. **Spectral Theorem**: A Hermitian operator can be diagonalized in an orthonormal basis, meaning that it can be represented as a diagonal matrix with its real eigenvalues on the diagonal. This is fundamental in quantum mechanics, as it allows the decomposition of quantum states in terms of the eigenstates of an observable.

## Example of a Hermitian Operator

One of the most common examples of a Hermitian operator in quantum mechanics is the **Hamiltonian** operator $\hat{H}$, which represents the total energy of a system. The Hamiltonian is Hermitian, meaning that its eigenvalues (the energy levels of the system) are real, ensuring that measurable energy values are physically meaningful.

Another example is the **position operator** $\hat{x}$ or the **momentum operator** $\hat{p}$, which are both Hermitian in the appropriate representation (such as in the position or momentum space).

## Hermitian Operators in Quantum Mechanics

In quantum mechanics, every **observable** (a measurable quantity like energy, position, or momentum) is associated with a Hermitian operator. When a quantum system is in a state $|\psi\rangle$, a measurement of the observable corresponding to a Hermitian operator $\hat{A}$ will yield an eigenvalue $a$ of $\hat{A}$, and the system will collapse into the corresponding eigenstate.

- **Eigenvalue equation for a Hermitian operator**:
   $$
   \hat{A} | \psi \rangle = a | \psi \rangle
   $$

Here, $a$ is the real eigenvalue (the measurable result), and $|\psi\rangle$ is the corresponding eigenvector (the state of the system after measurement).
