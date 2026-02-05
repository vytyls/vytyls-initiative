---
date: 25.10.26
time: 02:22:14
tags:
  - electromagneticField
  - fundamentalForces
  - qed
  - gaugeTheory
  - fourVectorPotential
  - photon
---
# MTH - The Electromagnetic Field

### 1. Core Definition

The **Electromagnetic (EM) Field** is a fundamental field in physics that describes one of the four fundamental forces of nature. It is the field responsible for all electric and magnetic phenomena. Classically, it is described by the unified electric and magnetic fields, and in quantum mechanics, its fundamental quantum (or particle) is the **photon**.

### 2. Classical Electrodynamics

In classical physics, the EM field is described by **Maxwell's Equations**. These equations govern the behavior of two distinct, yet interconnected, vector fields:

* **Electric Field ($\vec{E}$):** A field produced by electric charges, which exerts a force on other charges.
* **Magnetic Field ($\vec{B}$):** A field produced by moving electric charges (currents), which exerts a force on other moving charges.

In the context of special relativity, these two fields are revealed to be different aspects of a single, unified electromagnetic field tensor.

### 3. Relativistic Formulation: The Four-Vector Potential

To ensure the laws of electromagnetism are consistent in all inertial frames (i.e., Lorentz covariant), the electric and magnetic fields are unified.

* **Four-Vector Potential ($A^\mu$):** The field is described using a **four-vector potential**, which combines the scalar electric potential ($\phi$) and the magnetic vector potential ($\vec{A}$) into a single four-vector.
    $$
    A^\mu = (\phi/c, \vec{A})
    $$
    (In units where $c=1$, this is often written $A^\mu = (\phi, \vec{A})$ as in the source note).

* **Field Tensor ($F^{\mu\nu}$):** The physical electric and magnetic fields are derived from this potential as components of the **electromagnetic field tensor**, $F^{\mu\nu}$:
    $$
    F^{\mu\nu} = \partial^\mu A^\nu - \partial^\nu A^\mu
    $$

* **Gauge Invariance:** A crucial property of the EM field is **gauge invariance**. The physical observables (like the $\vec{E}$ and $\vec{B}$ fields, and the $F^{\mu\nu}$ tensor) remain unchanged under a "gauge transformation" of the potential. This transformation is:
    $$
    A_\mu \to A_\mu - \partial_\mu \alpha(x)
    $$
    where $\alpha(x)$ is any scalar function of spacetime. This mathematical "redundancy" is a deep and defining feature of the theory.

### 4. Quantum Electrodynamics (QED)

**Quantum Electrodynamics (QED)** is the **quantum field theory (QFT)** that describes the interactions of light and matter.

* **Quantization:** In QED, the electromagnetic field (described by $A^\mu$) is quantized. This process involves promoting the field to an operator built from **creation and annihilation operators** that describe the addition or removal of its fundamental quanta.
* **Interactions:** QED provides an incredibly precise framework for calculating the probabilities of processes involving charged particles (like electrons) and photons, such as scattering, particle-antiparticle creation, and atomic behavior.

### 5. The Photon

The **photon** is the elementary particle, or **quantum**, of the electromagnetic field.

* **Properties:** Photons are massless, have zero electric charge, and have a spin of 1 (making them bosons). They travel at the speed of light, $c$, in a vacuum.
* **Energy:** The energy of a single photon is directly related to the frequency ($\nu$) of the electromagnetic field by the Planck equation:
    $$
    E = h\nu
    $$
    where $h$ is Planck's constant.