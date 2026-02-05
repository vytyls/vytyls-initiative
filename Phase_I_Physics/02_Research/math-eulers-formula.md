---
date: 25.10.21
source: Synthesis Session
tags:
  - mathematics
  - physics
  - foundationalConcepts
  - eulersFormula
  - complexAnalysis
---
# MTH - Euler's Formula

## 1. Introduction: The Bridge Between Worlds

Euler's formula is a fundamental identity in mathematics that establishes a profound and beautiful connection between the exponential function and trigonometry. It is the bridge that links algebra, geometry, and analysis.

At its core, the formula states that for any real number $\theta$ (in radians):

$$
e^{i\theta} = \cos(\theta) + i\sin(\theta)
$$

Where:
* **$e$** is Euler's number, the base of the natural logarithm ($e \approx 2.71828...$).
* **$i$** is the imaginary unit, defined as the solution to $i^2 = -1$.
* **$\theta$** (theta) is the angle, which serves as the input to the trigonometric functions.
* **$\cos$** and **$\sin$** are the cosine and sine trigonometric functions.

This note provides a canonical, math-heavy derivation and exploration of this formula and its implications.

---

## 2. The Mathematical Foundation: Taylor Series Derivation

The most common and rigorous proof of Euler's formula relies on the Taylor series expansions of the constituent functions. A Taylor series is a way to represent any smooth function as an infinite sum of terms calculated from the function's derivatives at a single point.

### 2.1 The Core Series Expansions

We begin with the established Maclaurin series (a Taylor series centered at 0) for $e^x$, $\cos(x)$, and $\sin(x)$:

**1. The Exponential Function ($e^x$):**
$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \dots
$$

**2. The Cosine Function ($\cos(x)$):**
$$
\cos(x) = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{(2n)!} = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \dots
$$

**3. The Sine Function ($\sin(x)$):**
$$
\sin(x) = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!} = \frac{x}{1!} - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \dots
$$

### 2.2 The Derivation

To derive Euler's formula, we substitute $x = i\theta$ into the series for $e^x$:

$$
e^{i\theta} = 1 + \frac{(i\theta)}{1!} + \frac{(i\theta)^2}{2!} + \frac{(i\theta)^3}{3!} + \frac{(i\theta)^4}{4!} + \frac{(i\theta)^5}{5!} + \dots
$$

Next, we evaluate the powers of $i$, remembering that $i^2 = -1$, $i^3 = -i$, $i^4 = 1$, $i^5 = i$, and so on, cycling every four powers:

* $(i\theta)^1 = i\theta$
* $(i\theta)^2 = i^2\theta^2 = -\theta^2$
* $(i\theta)^3 = i^3\theta^3 = -i\theta^3$
* $(i\theta)^4 = i^4\theta^4 = \theta^4$
* $(i\theta)^5 = i^5\theta^5 = i\theta^5$

Now, substitute these back into the series:
$$
e^{i\theta} = 1 + \frac{i\theta}{1!} - \frac{\theta^2}{2!} - \frac{i\theta^3}{3!} + \frac{\theta^4}{4!} + \frac{i\theta^5}{5!} - \dots
$$

The final step is to separate the terms into two groups: those *without* $i$ (the real part) and those *with* $i$ (the imaginary part).

**Real Part:**
$$
\left( 1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} - \dots \right)
$$

**Imaginary Part:**
$$
i \left( \frac{\theta}{1!} - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} - \dots \right)
$$

By comparing these grouped series with the original Taylor expansions, we see they are identical:
* The **Real Part** is the Taylor series for $\cos(\theta)$.
* The **Imaginary Part** is $i$ times the Taylor series for $\sin(\theta)$.

Therefore, we arrive at the formula:
$$
e^{i\theta} = \cos(\theta) + i\sin(\theta)
$$

---

## 3. The Geometric Interpretation: The Unit Circle

Euler's formula is not just an algebraic curiosity; it is a complete geometric description of a circle.

In the **complex plane** (where the x-axis is the "Real" axis and the y-axis is the "Imaginary" axis), the formula $e^{i\theta}$ plots a point on a **unit circle** (a circle with a radius of 1).

* The term **$\cos(\theta)$** is the **x-coordinate** (the Real part).
* The term **$\sin(\theta)$** is the **y-coordinate** (the Imaginary part).



Thus, $e^{i\theta}$ is a "phasor"—a rotating vector of length 1. As the angle $\theta$ increases, the point $(\cos(\theta), \sin(\theta))$ travels counter-clockwise around the unit circle. This provides a way to describe oscillations and rotations using a single, compact exponential term.

---

## 4. Key Corollaries and Applications

### 4.1 Euler's Identity: "The Most Beautiful Equation"

If we set the angle $\theta = \pi$ (180 degrees), we get a special case:
$$
e^{i\pi} = \cos(\pi) + i\sin(\pi)
$$
Since $\cos(\pi) = -1$ and $\sin(\pi) = 0$, this simplifies to:
$$
e^{i\pi} = -1
$$
Rearranging this gives **Euler's Identity**:
$$
e^{i\pi} + 1 = 0
$$
This equation is famous for linking the five most fundamental constants in mathematics: $e$ (the base of natural growth), $i$ (the basis of complex numbers), $\pi$ (the ratio of a circle's circumference), $1$ (the multiplicative identity), and $0$ (the additive identity).

### 4.2 Deriving Trigonometric Identities

Euler's formula provides a powerful way to derive trigonometric identities. By considering $e^{-i\theta}$:
$$
e^{-i\theta} = \cos(-\theta) + i\sin(-\theta) = \cos(\theta) - i\sin(\theta)
$$
We now have a system of two equations:
1.  $e^{i\theta} = \cos(\theta) + i\sin(\theta)$
2.  $e^{-i\theta} = \cos(\theta) - i\sin(\theta)$

By **adding** these two equations, the sine terms cancel:
$$
e^{i\theta} + e^{-i\theta} = 2\cos(\theta)
$$
$$
\cos(\theta) = \frac{e^{i\theta} + e^{-i\theta}}{2}
$$
By **subtracting** the second equation from the first, the cosine terms cancel:
$$
e^{i\theta} - e^{-i\theta} = 2i\sin(\theta)
$$
$$
\sin(\theta) = \frac{e^{i\theta} - e^{-i\theta}}{2i}
$$
These definitions transform trigonometric problems into algebraic ones, which are often much simpler to solve.

### 4.3 Application in Physics: Wave Mechanics

This algebraic simplicity is why Euler's formula is indispensable in physics, particularly in wave mechanics and quantum mechanics.

A physical, real-world wave (like a light wave or a water wave) can be described by $\cos(kx - \omega t)$. Using Euler's formula, we can represent this wave as simply the **real part** of a complex exponential:
$$
\cos(kx - \omega t) = \text{Re}\left( e^{i(kx - \omega t)} \right)
$$
This allows us to describe a **forward-propagating wave** as $\Psi_{+} = A e^{i(kx - \omega t)}$ and a **counter-propagating wave** as $\Psi_{-} = B e^{i(-kx - \omega t)}$.

When we want to see how these waves add up (superposition), we simply add the complex exponentials $\Psi_{+} + \Psi_{-}$, a simple algebraic operation. This is vastly easier than using trigonometric sum-to-product identities. The "interwoven tube" of harmonics we've discussed is a direct visualization of this principle: a complex sum of many $\Psi_n$ terms, each a "thread" in the final structure.