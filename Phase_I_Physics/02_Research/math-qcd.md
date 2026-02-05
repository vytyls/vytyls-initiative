---
date: 25.10.26
time: 02:07:35
tags:
  - qcd
  - strongInteraction
  - yangMillsTheory
  - gaugeTheory
  - confinement
  - asymptoticFreedom
  - quarks
  - gluons
  - standardModel
  - particlePhysics
---
# MTH - Quantum Chromodynamics (QCD)

### 1. Core Definition

**Quantum Chromodynamics (QCD)** is the fundamental quantum field theory that describes the **strong interaction**, one of the four fundamental forces of nature. As the strong-force sector of the Standard Model, QCD explains how fundamental particles called **quarks** interact by exchanging force-carrying bosons called **gluons**. The theory is responsible for binding quarks together to form hadrons (like protons and neutrons) and, by extension, for the residual force that holds atomic nuclei together.

### 2. Fundamental Particles

The theory is built upon two types of elementary particles:

* **Quarks:** These are spin-½ fermions that possess a property called **color charge** (red, green, or blue). They come in six "flavors": up, down, charm, strange, top, and bottom.
* **Gluons:** These are massless spin-1 bosons that mediate the strong interaction. Gluons are the gauge bosons of the theory and carry color-anticolor combinations (e.g., red-antigreen).

### 3. Mathematical Framework: SU(3) Gauge Theory

QCD is mathematically formulated as a non-abelian **$SU(3)$ Yang-Mills gauge theory**. Its dynamics are encoded in the QCD Lagrangian:

$$
\mathcal{L}_{\rm QCD} = -\tfrac{1}{4}F^{a}_{\mu\nu}F^{\mu\nu a} + \sum_{f}\bar\psi_{f}(i\gamma^\mu D_\mu - m_f)\psi_f
$$

This Lagrangian consists of two main parts:

1.  **Gluon Dynamics (Yang-Mills sector):** The $F^{a}_{\mu\nu}$ term describes the gluon field and its self-interactions. $F^{a}_{\mu\nu}$ is the **gluon field strength tensor**.
2.  **Quark Dynamics (Fermion sector):** The $\bar\psi_{f}$ term describes the quarks (with flavor $f$ and mass $m_f$) and their interaction with the gluon field via the **covariant derivative**, $D_\mu$.

Unlike in electromagnetism (a $U(1)$ theory), the non-abelian nature of $SU(3)$ means that gluons carry color charge themselves and interact with each other. This self-interaction is the source of QCD's unique properties.

### 4. Key Phenomena

The $SU(3)$ structure gives rise to two defining, counter-intuitive phenomena:

* **Confinement:** Quarks and gluons cannot be isolated as free particles. The strong force *grows* with distance, meaning it would take infinite energy to separate them. This is why only **color-neutral** composite particles (hadrons like baryons and mesons) are observed in nature.
* **Asymptotic Freedom:** Conversely, at very high momentum transfer (i.e., extremely short distances), the strong coupling constant, $\alpha_s(Q^2)$, *decreases*. This means quarks and gluons behave almost as free particles when they are very close together, which allows for the use of perturbative expansions in high-energy calculations.