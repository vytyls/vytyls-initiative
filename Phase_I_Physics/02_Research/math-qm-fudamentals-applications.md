---
date: 25.09.15
time: 12:37:27
tags:
  - mathematics
  - quantumMechanics
---
# MTH - Quantum Mechanics Fundamentals and Applications

## Detailed Briefing Document: Quantum Mechanics Fundamentals and Applications

This briefing document synthesizes the core concepts, principles, and applications of quantum mechanics as presented in the provided excerpts from "QuantumBook.pdf" by Daniel V. Schroeder. It highlights key ideas, theoretical frameworks, numerical methods, and significant physical examples.

### 1. The Nature of Quantum Mechanics

Quantum mechanics is a fundamental theory that governs the structure and interactions of all matter. It provides explanations for phenomena such as atomic stability, radioactive decay, and the greenhouse effect of carbon dioxide. Its utility extends across chemistry, materials science, and subatomic physics, enabling the design of technologies like microscopes, lasers, solar cells, and secure communication methods.

Schroeder emphasizes the inherent difficulty of learning quantum mechanics due to its divergence from common sense, likening it to the "ancient Indian parable of the blind men trying to apprehend an elephant." The book aims to make the subject accessible by starting with a single, structureless particle in one dimension, leveraging classical wave intuition, before progressing to more complex systems.

### 2. Wave Mechanics: The Foundation

#### 2.1. Wave-Particle Duality and Planck's Constant

At the heart of quantum mechanics is the concept of wave-particle duality. Particles like electrons exhibit wave-like behavior, as demonstrated by diffraction experiments. These experiments show "random blips at low intensity, with the wavelength-dependent pattern emerging at higher intensity," implying that "randomness and probabilities seem to be inherent in the de Broglie relation." The relationship between a particle's energy (E) and frequency (f), and momentum (p) and wavelength (λ), is governed by Planck's constant (h):

- **Einstein relation:** $E = hf$
- **de Broglie relation:** $p = h/λ$

These relations are generalized for any particle through the concept of wavefunctions.

#### 2.2. Wavefunctions ($\psi(x)$)

A **wavefunction** ($\psi(x)$) is a complex-valued function of space that encodes the current state of a quantum system. Unlike a classical particle, whose state is defined by its position and momentum, a quantum particle's state is described by this infinitely detailed function.

- **Probability Density:** The probability of finding a particle at a given location $x$ is proportional to the **square modulus** of the wavefunction, $|ψ(x)|^2$. This is known as the **Born rule for position**:
- $(Probability of finding particle between a and b) = \int_a^b |ψ(x)|^2 dx$.
- The function $|ψ(x)|^2$ is called the **probability density**.
- **Normalization:** For probabilities to sum to 100%, the total integral of the probability density over all space must equal 1: $\int_{-\infty}^{\infty} |ψ(x)|^2 dx = 1$.
- **Average Values:** The average position, $\langle x \rangle$, and the average of any function of $x$, $\langle f(x) \rangle$, are calculated by integrating the function weighted by the probability density:
- $\langle f(x) \rangle = \int_{-\infty}^{\infty} f(x) |ψ(x)|^2 dx$.
- **Complex Nature:** Wavefunctions are generally complex, having both real and imaginary parts. The phase of a wavefunction (represented by color hues in visualizations) is crucial for phenomena like momentum and wave interference. The factor $eiφ$ can be multiplied by a wavefunction without affecting measurement probabilities.

#### 2.3. Position and Momentum Eigenfunctions

- **Localized Wavefunctions:** A narrow, "spiky" wavefunction indicates a well-defined position, akin to a classical particle.
- **"Cat States":** Wavefunctions can have multiple separated spikes, representing a particle existing in a superposition of distinct locations, such as Schrödinger's cat (half alive, half dead).
- **Momentum Eigenfunctions:** A particle with a well-defined momentum $p_x$ is described by a periodic, complex exponential function: $\psi(x) = Ae^{ikx}$, where $k = p_x / \hbar$. The complex nature allows for encoding the direction of momentum.

#### 2.4. Measurement and Wavefunction Collapse

When a measurement is performed, the measured quantity becomes well-defined, and the particle's wavefunction "collapses" into the eigenfunction corresponding to the measurement outcome. This collapse is random but deterministic immediately after measurement. The precise definition of "measurement" remains an open question in quantum mechanics.

#### 2.5. Time Evolution and the Schrödinger Equations

- **Wiggle Factor:** For a state with well-defined energy $E$, the wavefunction oscillates in time with angular frequency $\omega = E/\hbar$. This is incorporated by multiplying the spatial wavefunction by the "wiggle factor" $e^{-i\omega t}$.
- **Time-Dependent Schrödinger Equation (TDSE):** This first-order partial differential equation describes how any wavefunction evolves smoothly in time:
- $i\hbar \frac{\partial \psi}{\partial t} = \hat{H}\psi$,
- where $\hat{H}$ is the Hamiltonian operator (total energy operator). The TDSE is the quantum mechanical equivalent of Newton's second law.
- **Time-Independent Schrödinger Equation (TISE):** For energy eigenfunctions, where the probability density is constant in time, the TDSE simplifies to the TISE:
- $\hat{H}\psi = E\psi$.
- This is an eigenvalue equation, where $E$ is the energy eigenvalue and $\psi$ is the energy eigenfunction.

### 3. Bound States in One Dimension

Bound states occur when a particle is trapped in a limited region of space, leading to quantized (discrete) energy levels.

#### 3.1. Qualitative Features of Wavefunctions

Solutions to the TISE exhibit distinct behaviors:

- **Classically Allowed Regions ($E > V(x)$):** Wavefunctions oscillate. Their amplitude and wavelength are smaller where kinetic energy ($E - V(x)$) is larger.
- **Classically Forbidden Regions ($E < V(x)$):** Wavefunctions exhibit exponential decay, dying out as they penetrate deeper into these regions. The decay is steeper where $V(x) - E$ is larger. This implies a non-zero probability of finding a particle in classically forbidden regions, a phenomenon without a classical counterpart.
- **Quantization:** Quantization of energy levels arises because wavefunctions must fit an integer number of half-oscillations or "bumps" within the confining potential, and must decay to zero in forbidden regions (unless the region extends indefinitely).

#### 3.2. The Infinite Square Well

This idealized potential ($V(x) = 0$ for $0 < x < a$, and $\infty$ elsewhere) is a cornerstone example.

- **Energy Eigenfunctions:** Solutions are standing sine waves: $\psi_n(x) = A \sin(n\pi x/a)$. These are energy eigenfunctions but not momentum eigenfunctions (they are superpositions of positive and negative momentum states).
- **Quantized Energies:** The allowed energy levels are discrete: $E_n = \frac{h^2 n^2}{8ma^2}$. The ground state ($n=1$) has non-zero energy, known as the **zero-point energy**, which is crucial for atomic stability.
- **Completeness and Orthogonality:** The energy eigenfunctions form a complete and orthonormal basis set. Any other wavefunction can be expressed as a linear combination of these eigenfunctions (Fourier series). The coefficients of this expansion determine the probabilities of measuring corresponding energy values: $P(E_n) = |c_n|^2$.

#### 3.3. Numerical Methods for the TISE

- **Shooting Method:** This iterative method involves guessing an energy, numerically integrating the TISE from one boundary, and adjusting the guess until the wavefunction satisfies the boundary conditions at the other end (e.g., smoothly decaying to zero). It's effective for finding individual bound states.
- **Matrix Method (Diagonalization):** This method expresses the Hamiltonian operator as a matrix in a chosen basis of orthonormal functions (e.g., infinite square well eigenfunctions). Finding the eigenvalues and eigenvectors of this matrix then yields the energy eigenvalues and eigenfunctions of the system. This method is generally more abstract but can find all bound states simultaneously.

#### 3.4. The Harmonic Oscillator

A parabolic potential energy $V(x) = \frac{1}{2} m\omega_c^2 x^2$ models vibrating molecules and acoustic phonons.

- **Quantized Energies:** Energy levels are evenly spaced: $E_n = (n + \frac{1}{2})\hbar\omega_c$, where $n=0, 1, 2, \dots$.
- **Ladder Operators:** A powerful algebraic method using "raising" ($a^+$) and "lowering" ($a^-$) operators allows for the derivation of energy eigenvalues and eigenfunctions without explicit calculus. These operators convert one energy eigenfunction into the next higher or lower energy eigenfunction.

#### 3.5. Multiple Wells and Tunneling

- **Double Wells:** In potentials with two minima, energy levels often appear in closely spaced pairs. Wavefunctions typically resemble superpositions of single-well eigenfunctions.
- **Tunneling:** Particles can move between wells through a classically forbidden barrier, a phenomenon called **quantum-mechanical tunneling**. This involves an oscillation of probability density between the wells, with a characteristic "tunneling time" inversely proportional to the energy splitting ($\Delta E$) between the paired states. This behavior is foundational to understanding phenomena like the ammonia maser and is an example of a **two-state system** or **qubit**.

### 4. Unbound States and Wavepackets in One Dimension

Unbound states describe particles with enough energy to escape a potential well, resulting in continuous energy spectra.

#### 4.1. Momentum Space

Wavefunctions can be expressed as superpositions of momentum eigenfunctions using Fourier transforms.

- **Momentum-Space Wavefunction ($\tilde{\psi}(p)$):** This function encodes the amplitude of each momentum state in the overall wavefunction.
- **Born Rule for Momentum:** The probability of measuring momentum between $p_a$ and $p_b$ is given by $\int_{p_a}^{p_b} |\tilde{\psi}(p)|^2 dp$.
- **Momentum Operator:** The average momentum can be calculated directly from the position-space wavefunction using the momentum operator $\hat{p}_x = -i\hbar \frac{d}{dx}$: $\langle p \rangle = \int_{-\infty}^{\infty} \psi^*(x) (\hat{p}_x \psi(x)) dx$.

#### 4.2. Wavepackets and the Uncertainty Principle

A **wavepacket** is a localized wavefunction with an approximately well-defined momentum, representing the closest quantum mechanical analogue to a classical particle.

- **Gaussian Wavepacket:** A common example is $\psi(x) = Ae^{-(x-x_0)^2/a^2} e^{ip_0x/\hbar}$.
- **Group Velocity vs. Phase Velocity:** The wavepacket as a whole moves at the classical particle velocity (group velocity), while the internal "ripples" move at half that speed (phase velocity).
- **Spreading:** Wavepackets naturally spread out over time due to **dispersion**, as different momentum components travel at different speeds. The characteristic spreading time is $ma^2/(2\hbar)$.
- **Heisenberg Uncertainty Principle:** A fundamental limit on the simultaneous precision with which position and momentum can be known: $\sigma_x \sigma_p \ge \hbar/2$. This principle is a specific case of a more general uncertainty principle relating any pair of incompatible observables.

#### 4.3. Numerical TDSE Solutions

The TDSE can be directly solved numerically using the **centered-difference method**, which discretizes both space and time. This allows for predicting the time evolution of any initial wavefunction under any potential energy function. The algorithm involves calculating the wavefunction at a future time step based on its values at the current and previous steps.

#### 4.4. Scattering from a Barrier

When a wavepacket encounters a potential barrier, it can exhibit both reflection and transmission, even if classically it would fully transmit or reflect.

- **Energy Filtering:** The barrier acts as a filter, allowing higher-energy momentum components to transmit and reflecting lower-energy components.
- **Tunneling:** When the particle's energy is less than the barrier height, there is still a non-zero probability of tunneling through the barrier, with the transmission probability decaying exponentially with barrier width and height difference.
- **Interference:** Reflected and transmitted waves create interference patterns.

### 5. Beyond One Dimension: Multiple Spatial Dimensions and Particles

#### 5.1. Multiple Spatial Dimensions

The generalization to multiple spatial dimensions involves wavefunctions that are functions of multiple spatial variables (e.g., $\psi(x, y)$ or $\psi(x, y, z)$).

- **Operators:** Position and momentum operators become vector operators (e.g., $\vec{\hat{r}} = \vec{r}$, $\vec{\hat{p}} = -i\hbar \nabla$). The Hamiltonian includes the Laplacian operator ($\nabla^2$).
- **Separable Wavefunctions:** If the potential energy is separable ($V(x, y) = V_1(x) + V_2(y)$), the TISE can be separated into one-dimensional equations.
- **Degeneracy:** Multiple, distinct eigenfunctions can correspond to the same energy eigenvalue, leading to "degenerate" states. Any linear combination of degenerate eigenfunctions is also an eigenfunction with the same eigenvalue.

#### 5.2. Multiple Particles

A system of two particles in one dimension is mathematically analogous to a single particle in two dimensions, with the coordinates ($x_1, x_2$) replacing ($x, y$).

- **Configuration Space:** The state of multiple particles is described by a single wavefunction in a higher-dimensional **configuration space**.
- **Entanglement:** When a multi-particle wavefunction cannot be factored into a product of individual particle wavefunctions, the particles are **entangled**. Interactions between particles typically lead to entanglement. As Schrödinger stated, "By the interaction the two representatives (or ψ-functions) have become entangled."
- **Identical Particles:** Quantum mechanics allows for truly identical particles, which are indistinguishable. Their wavefunctions must be either **symmetric** (bosons) or **antisymmetric** (fermions) under particle interchange. The **Pauli exclusion principle** (for fermions) states that two identical fermions cannot occupy the same single-particle quantum state.

### 6. Working with Operators

Operators are central to quantum mechanics, representing observable quantities.

#### 6.1. Hermitian Operators

- **Definition:** An operator $\hat{A}$ is Hermitian if $\langle \hat{A}\psi_1 | \psi_2 \rangle = \langle \psi_1 | \hat{A}\psi_2 \rangle$ for all $\psi_1, \psi_2$.
- **Properties:** Hermitian operators have real eigenvalues (corresponding to observable values) and orthogonal eigenvectors (forming a complete, orthonormal basis).

#### 6.2. Commuting and Noncommuting Operators

- **Commutator:** The commutator of two operators is $[\hat{A}, \hat{B}] = \hat{A}\hat{B} - \hat{B}\hat{A}$.
- **Compatible Observables:** Two observables are compatible if their corresponding operators commute. This means they can be simultaneously well-defined and possess a common eigenbasis.
- **Incompatible Observables:** Operators that do not commute (e.g., position and momentum, $[\hat{x}, \hat{p}_x] = i\hbar$) are incompatible. Measuring one affects the other, as quantified by the generalized uncertainty principle: $\sigma_A \sigma_B \ge |\frac{1}{2i} \langle [\hat{A},\hat{B}] \rangle|$.

### 7. Central Forces and Angular Momentum

#### 7.1. Spherical Coordinates and the Hamiltonian

For a particle in three dimensions subject to a spherically symmetric potential $V(r)$, spherical coordinates ($r, \theta, \phi$) are natural. The Hamiltonian is best expressed using the Laplacian operator in spherical coordinates. Crucially, the Hamiltonian can be written in terms of the total angular momentum squared operator $\hat{L}^2$: $\hat{H} = -\frac{\hbar^2}{2mr^2} \frac{\partial}{\partial r} (r^2 \frac{\partial}{\partial r}) + \frac{\hat{L}^2}{2mr^2} + V(r)$.

#### 7.2. Angular Momentum Operators

- **Commutation Relations:** The components of the angular momentum operator ($\hat{L}_x, \hat{L}_y, \hat{L}_z$) do not commute with each other. This means they cannot be simultaneously well-defined.
- **$\hat{L}^2$ and $\hat{L}_z$:** The total angular momentum squared operator $\hat{L}^2$ commutes with each component operator, so $\hat{L}^2$ and $\hat{L}_z$ (by convention) share a common eigenbasis.
- **Eigenvalues:** The eigenvalues of $\hat{L}^2$ are $l(l+1)\hbar^2$, and the eigenvalues of $\hat{L}_z$ are $m\hbar$, where $l$ is the orbital angular momentum quantum number (non-negative integer) and $m$ is the magnetic quantum number (ranging from $-l$ to $l$ in integer steps).
- **Ladder Operators:** Angular momentum raising ($\hat{L}^+$) and lowering ($\hat{L}^-$) operators can be used to move between $\hat{L}_z$ eigenstates within a given $l$ ladder, increasing or decreasing $m$ by 1.
- **Spherical Harmonics ($Y_l^m(\theta, \phi)$):** These are the common eigenfunctions of $\hat{L}^2$ and $\hat{L}_z$, depending only on the angular coordinates $\theta$ and $\phi$. They form a complete orthonormal basis for functions of angles.

#### 7.3. The Radial Equation

By separating the TISE using spherical harmonics, we obtain a **reduced radial equation** for the radial wavefunction $u(r) = rR(r)$: $[ -\frac{\hbar^2}{2m} \frac{d^2}{dr^2} + V_{eff}(r) ] u(r) = E u(r)$, where $V_{eff}(r) = \frac{\hbar^2 l(l+1)}{2mr^2} + V(r)$ is the **effective potential energy**, including a repulsive **centrifugal term** for $l > 0$. This equation is mathematically identical to a one-dimensional TISE, making all the previously learned solution techniques applicable.

#### 7.4. The Hydrogen Atom

The most important example of a central force problem, with the Coulomb potential $V(r) = -\frac{e^2}{4\pi\epsilon_0 r}$.

- **Atomic Units:** Natural units ($a_0 = 0.529 \times 10^{-10}$ m, $E_h = 27.2$ eV) simplify the equations.
- **Quantized Energies:** The energy levels are quantized and given by $E_n = -\frac{13.6 \text{ eV}}{n^2}$, where $n$ is the principal quantum number ($n=1, 2, 3, \dots$).
- **Degeneracy:** For a given $n$, the energy is independent of $l$ and $m$. There are $n^2$ degenerate states for each $n$.
- **Radial Wavefunctions ($R_{nl}(r)$):** These functions (multiplied by spherical harmonics) describe the electron's probability distribution. They involve exponential decay and associated Laguerre polynomials.
- **Nomenclature:** $l=0, 1, 2, 3$ states are called s, p, d, f waves, respectively.

#### 7.5. The Helium Atom

A much more complex two-electron system.

- **Perturbation:** Starting from a simplified model of two non-interacting electrons in a $Z=2$ nucleus, the electron-electron repulsion term $V_{12} = \frac{e^2}{4\pi\epsilon_0 |r_2 - r_1|}$ is added.
- **Matrix Method:** The complex interaction is handled by building a Hamiltonian matrix in a basis of "unperturbed" two-electron wavefunctions and diagonalizing it. This method shows that electron repulsion splits degeneracies and leads to entangled states.
- **Parahelium and Orthohelium:** Spatially symmetric states (parahelium) and antisymmetric states (orthohelium) correspond to different spin configurations and have different energies due to electron-electron repulsion.

### 8. Spin

Spin is an intrinsic form of angular momentum, distinct from orbital angular momentum.

- **Commutation Relations:** Spin operators ($\hat{S}_x, \hat{S}_y, \hat{S}_z$) obey similar commutation relations to orbital angular momentum operators.
- **Eigenvalues:** $\hat{S}^2$ has eigenvalues $s(s+1)\hbar^2$, and $\hat{S}_z$ has eigenvalues $m_s\hbar$.
- **Spin-1/2 Particles:** The most common case, with $s=1/2$.
- **Magnitude:** $|\vec{S}| = \sqrt{3}/2 \hbar$.
- **$S_z$ values:** $m_s = +1/2$ (spin-up, $\chi^+$) or $-1/2$ (spin-down, $\chi^-$).
- **Spinors:** Spin states are represented by two-component complex vectors (spinors).
- **Pauli Matrices:** Spin operators are represented by $2 \times 2$ matrices (e.g., Pauli matrices for spin-1/2).
- **Bloch Sphere:** A 3D sphere visualization where every point corresponds to a unique spin-1/2 physical state, representing the direction of the spin.

#### 8.1. Spin in Magnetic Fields

- **Magnetic Dipole Moment:** Charged particles with spin have a magnetic dipole moment $\vec{\mu} = \gamma \vec{S}$, which interacts with external magnetic fields.
- **Hamiltonian:** For a uniform magnetic field $\vec{B}$ along the $z$-axis, $\hat{H} = -\gamma B \hat{S}_z$.
- **Larmor Precession:** A spin-1/2 particle initially in a superposition of $\hat{S}_z$ eigenstates will precess around the magnetic field direction at the Larmor frequency $\omega_L = \gamma B$.
- **Stern-Gerlach Experiment:** A non-uniform magnetic field splits a beam of particles based on their spin components (e.g., $S_z$), allowing for spin measurement. This process "entangles" the particle's spin and spatial states.

#### 8.2. Photon Polarization

Photons are spin-1 particles but only have two independent polarization states (right-handed and left-handed circular polarization). They are treated as two-state systems (qubits) using Jones vectors (e.g., horizontal and vertical linear polarization as basis states). The Poincaré sphere (Bloch sphere) can represent photon polarization states.

#### 8.3. Addition of Angular Momenta

When combining angular momenta from multiple sources (e.g., two spin-1/2 particles, or orbital and spin angular momentum), the total angular momentum is quantized.

- **Singlet and Triplet States:** For two spin-1/2 particles, the four possible states can be classified into a spin-0 **singlet** state and three spin-1 **triplet** states.
- **Clebsch-Gordan Coefficients:** These coefficients relate the individual-particle basis states to the total angular momentum eigenstates.
- **Tensor Products:** Spinors for composite systems are represented as tensor products of individual particle spinors, and operators are represented by tensor products of individual particle matrices.

### 9. Core Principles of Quantum Mechanics (Generalized)

1. **States as Vectors:** System states correspond to vectors in a complex vector space. Linear combinations of vectors are allowed, representing superpositions and entangled states.
2. **Observables as Hermitian Operators:** Observable quantities correspond to Hermitian operators. Their real eigenvalues are possible measurement outcomes.
3. **Born Rule for Probabilities:** The probability of obtaining an eigenvalue $a_i$ when measuring observable $\hat{A}$ in state $\psi$ is $P(a_i) = |\langle \alpha_i | \psi \rangle|^2$, where $\alpha_i$ is the corresponding eigenstate.
4. **Wavefunction Collapse:** A measurement causes the system's state to abruptly collapse into the eigenstate corresponding to the obtained value.
5. **TDSE for Time Evolution:** The state vector changes smoothly according to $i\hbar \frac{\partial \psi}{\partial t} = \hat{H}\psi$.

These principles, while robust in practice, leave the definition of "measurement" ambiguous, a point of ongoing debate among physicists and philosophers.

---

