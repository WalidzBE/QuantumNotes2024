A **Hilbert space** is an essential framework for quantum mechanics, where quantum states are represented as vectors, and physical observable are operators acting on these vectors. The structure of Hilbert space, especially its inner product, allows us to compute probabilities and describe the behavior of quantum systems. 
## Definition of a Hilbert Space

A **Hilbert space** is a complete inner product space that satisfies the following properties:

1. **Vector Space**: It is a set of vectors (like $|\psi\rangle$ and $|\phi\rangle$) that can be added together and multiplied by scalars, just like in conventional vector spaces.

2. **Inner Product**: The space is equipped with an inner product, denoted by $\langle \psi | \phi \rangle$, which is a function that takes two vectors and returns a complex number. The inner product provides a notion of "angle" and "length" in the space, enabling the measurement of distances and projections. The inner product satisfies:
   - $\langle \psi | \psi \rangle \geq 0$, with equality only when $|\psi\rangle = 0$
   - $\langle \psi | \phi \rangle = \overline{\langle \phi | \psi \rangle}$ (conjugate symmetry)

3. **Completeness**: A Hilbert space is **complete**, meaning that any Cauchy sequence of vectors has a limit within the space. This ensures that there are no "gaps" in the space, making it well-suited for rigorous mathematical descriptions of quantum systems. Completeness ensures that the Hilbert space is closed under the operation of taking limits of sequences of vectors. This is important because physical systems are often described using approximations, and we want to ensure that the limits of these approximations still represent valid quantum states.
   In more intuitive terms, completeness means that there are no "gaps" in the Hilbert space. If you take an infinite series of steps that get progressively smaller, the end result (the limit) must still be a valid element (vector) in the Hilbert space. This is crucial for making the space mathematically stable and reliable for representing physical systems.

4. **Norm and Distance**: The inner product defines a norm (or length) of a vector, given by:
   $$
   ||\psi|| = \sqrt{\langle \psi | \psi \rangle}
   $$
   The distance between two vectors can be measured using this norm.

5. **Infinite Dimensionality**: In quantum mechanics, Hilbert spaces are often **infinite-dimensional**, meaning they contain an infinite number of basis vectors. This is necessary to describe systems with a continuous range of states, such as the position of a particle.

## Role in Quantum Mechanics

In quantum mechanics, a Hilbert space is used to represent the set of all possible quantum states of a system. The state of a quantum system is described by a vector in this space, typically denoted as $|\psi\rangle$ (a *ket*). Operators, such as those representing observables (e.g., position, momentum, or

The wave function \( \psi(x) \) must be [[PROOF OF NORMALIZATION PRINCIPLE OF WAVE FUNCTION|normalizable]]: 
$$
  \int |\psi(x)|^2 dx = 1  $$

The Hilbert space relevant to quantum mechanics is the set of all **square-integrable functions** on a given interval:
  $$
  \int_a^b |f(x)|^2 dx < \infty
  $$
# Bra and Ket in Quantum Mechanics

The **bra** and **ket** are essential components of the mathematical framework used to describe quantum states, known as **Dirac notation**. They play a fundamental role in quantum mechanics for representing vectors and their duals in Hilbert space.

## Ket (|ψ⟩)

A **ket** is a vector in a complex Hilbert space, which represents the state of a quantum system. It is denoted as $|\psi\rangle$, where $\psi$ symbolizes the particular state. For example, the quantum state of a particle could be written as $| \psi \rangle$, and this vector contains all the information about the system.

## Bra (⟨ψ|)

A **bra** is the dual of a ket, which corresponds to a row vector in linear algebra, as opposed to the column vector represented by a ket. It is denoted as $\langle \psi |$, and it operates on kets to produce scalar quantities. Mathematically, it is the complex conjugate transpose of the ket.
![[Screenshot_20241004_104655.png]]

## Bra-Ket Notation and Inner Products

The combination of a bra and a ket forms an inner product, which is a scalar quantity and represents probabilities or expectations in quantum mechanics. For example, if $|\psi\rangle$ and $|\phi\rangle$ are two kets, then their inner product is written as $\langle \psi | \phi \rangle$. This scalar result is often used to describe the probability amplitude for transitioning between two quantum states.

## Example:

- For a quantum state $| \psi \rangle$, the corresponding bra is $\langle \psi |$.
- The inner product $\langle \psi | \phi \rangle$ represents the overlap between two quantum states, $\psi$ and $\phi$.

This notation allows for concise representation of operations in quantum mechanics, such as measurements and state evolutions.
## Inner Product in Hilbert Space
The **inner product** of two functions $f(x)$ and $g(x)$in Hilbert space is defined as:
  $$
  \langle f | g \rangle = \int_a^b f(x)^* g(x) dx
  $$
  This satisfies the conditions for an inner product, ensuring it converges if both functions are square-integrable. 
**Properties of the inner product**:
  - **Conjugate symmetry**:
    $$
    \langle g | f \rangle = \langle f | g \rangle^*
    $$
  - The inner product of a function with itself is **real and non-negative**:
    $$
    \langle f | f \rangle = \int_a^b |f(x)|^2 dx
    $$

## Orthonormality and Completeness
A function is **normalized** if its inner product with itself is 1:
  $$
  \langle f | f \rangle = 1
  $$

Two functions are **orthogonal** if their inner product is zero:
  $$
  \langle f | g \rangle = 0
  $$
A set of functions $\{f_n(x)\}$ is **orthonormal** if:
  $$
  \langle f_m | f_n \rangle = \delta_{mn}
  $$
  
A set of functions is **complete** if any other function in Hilbert space can be expressed as a linear combination of them:
  $$
  f(x) = \sum_{n=1}^{\infty} c_n f_n(x)
  $$
  where:
  $$
  c_n = \langle f_n | f \rangle
  $$

### Use of Hilbert Space in Quantum Mechanics
In quantum mechanics, [[OBSERVABLE IN HILBERT SPACE AND HERMITIAN OPERATORS|observable]] are represented by operators acting on the vectors (wave functions) in Hilbert space. The properties of inner products and orthonormality allow for the calculation of probabilities and expectation values for measurements in quantum systems.
