---
date: 25.10.26
time: 02:13:40
tags:
  - wilsonLines
  - gaugeTheory
  - gaugeInvariance
  - observables
  - nonlocality
  - confinement
  - holography
---
# MTH - Wilson Lines and Loops

### 1. Core Definition

A **Wilson line** is a fundamental **non-local, gauge-invariant operator** in gauge theory. It is mathematically defined as the path-ordered exponential of the gauge connection $A$ integrated along a curve $C$.

The operator $W(C)$ is given by the expression:

$$
W(C) = \mathcal{P} \exp\left(i \int_C A \cdot dx\right)
$$

Where:
* $W(C)$ is the Wilson line operator along the path $C$.
* $\mathcal{P}$ denotes the **path-ordering operator**, which is necessary in non-abelian theories (like Yang-Mills) where the gauge fields at different points do not commute.
* $A$ is the **gauge connection** (or gauge field).

A closed Wilson line, where the path $C$ forms a loop, is called a **Wilson loop**.

### 2. Function and Significance

Wilson lines are crucial observables because they measure the **holonomy** of the gauge connection, or the effect of transporting a charged particle along a path through the gauge field.

Because they are gauge-invariant, their expectation values correspond to physical quantities. They are used to detect and probe several key non-perturbative phenomena:

* **Confinement:** The expectation value of a large Wilson loop is the primary order parameter for confinement in Yang-Mills theory. In a confining phase, the value scales with the *area* of the loop (the "area law"), which implies a linear potential between charges and explains why they cannot be separated. In a deconfined phase, it scales with the *perimeter* (the "perimeter law").
* **Topological Order:** They are used to detect topological phases of matter.
* **Boundary Phenomena:** They capture how charges are entangled with the gauge field at boundaries.

### 3. Role in Holography (AdS/CFT)

In the context of the AdS/CFT correspondence, Wilson lines and loops play a critical role in the holographic dictionary:

* A Wilson loop on the **boundary CFT** corresponds to the worldsheet of a fundamental **string** in the **AdS bulk** that is anchored on that loop at the boundary.
* This duality allows for the calculation of Wilson loop expectation values (a difficult non-perturbative problem in the CFT) by calculating the minimal area of a string worldsheet in the classical gravity bulk, which is a much simpler geometric problem.