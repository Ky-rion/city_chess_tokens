

You predicted it perfectly! This is exactly where we put those mathematical tools from Part 3 to work. We are now going to construct a mathematically valid, physically realistic state for our two indistinguishable electrons.

First, the translation of the problem:

> **4. Let now $\Psi(x_1, x_2) = \Phi_1(x_1)\Phi_2(x_2)$. Construct from this a normalized exchange-antisymmetric function $\Psi_-$. Normalize under the assumption that the $\Phi_i$ are orthonormal. [3 Pts.]**

Here is the step-by-step breakdown of how a physicist approaches this.

---

### Step 1: The "Naive" Wavefunction

The problem starts us off with a simple guess: $\Psi(x_1, x_2) = \Phi_1(x_1)\Phi_2(x_2)$.

Physically, this equation says: "Electron 1 is sitting exactly in state $\Phi_1$, and Electron 2 is sitting exactly in state $\Phi_2$."

But remember our golden rule from Part 2? Electrons do not wear nametags! They are entirely indistinguishable. If we use this naive function, we are pretending we can track which electron is which. Because electrons are Fermions, nature demands that their joint wavefunction must be strictly **anti-symmetric**.

### Step 2: Forcing Anti-symmetry

To fix this, we apply the anti-symmetric projector $\hat{\Pi}_-$ we found in Part 3. We take our naive function, and subtract the version where the particles are swapped.

Let's call our unnormalized anti-symmetric function $\Psi_{unnormalized}$:

$$\Psi_{unnormalized} = \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1)$$

_(Professor's side note: When you generalize this to atoms with many electrons, this construction is called a **Slater Determinant**. It's one of the most famous and useful structures in all of quantum chemistry!)_

### Step 3: Understanding "Orthonormal"

Now we have the right shape, but the problem asks us to "normalize" it.

The square of a wavefunction represents a probability. The total probability of finding our two electrons _somewhere_ in the universe must be exactly 100%, or $1$.

To ensure this, we multiply our function by a normalization constant, let's call it $N$:

$$\Psi_- = N [ \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1) ]$$

To find $N$, we use the vital hint given in the problem: the single-particle states $\Phi_i$ are **orthonormal**. This is a portmanteau of two words:

- **Normalized:** The probability of finding a single particle in its state is 1. Mathematically: $\int |\Phi_1|^2 dx = 1$ and $\int |\Phi_2|^2 dx = 1$.
    
- **Orthogonal:** The states are completely distinct and do not overlap. Mathematically, the integral of their product is zero: $\int \Phi_1^*(x)\Phi_2(x) dx = 0$.
    

### Step 4: The Math (Calculating the Normalization Constant)

We require the total probability to be 1:

$$\iint |\Psi_-|^2 dx_1 dx_2 = 1$$

Let's plug in our function and expand the square (using $|A - B|^2 = |A|^2 + |B|^2 - A^*B - B^*A$):

$$1 = N^2 \iint [|\Phi_1(x_1)\Phi_2(x_2)|^2 + |\Phi_1(x_2)\Phi_2(x_1)|^2 - \text{cross terms}] dx_1 dx_2$$

Let's look at the terms individually:

1. **The first squared term:** $\int |\Phi_1(x_1)|^2 dx_1 \cdot \int |\Phi_2(x_2)|^2 dx_2 = 1 \cdot 1 = 1$
    
2. **The second squared term:** $\int |\Phi_1(x_2)|^2 dx_2 \cdot \int |\Phi_2(x_1)|^2 dx_1 = 1 \cdot 1 = 1$
    
3. **The cross terms:** These look like $\Phi_1^*(x_1)\Phi_2(x_1)$. Because the states are **orthogonal**, integrating this gives exactly zero! Both cross terms vanish into nothingness.
    

So, the massive scary integral simplifies beautifully to:

$$1 = N^2 [ 1 + 1 - 0 - 0 ]$$

$$1 = 2 N^2$$

$$N = \frac{1}{\sqrt{2}}$$

### The Final Answer

By plugging $N$ back into our equation, we get the final, rigorously correct, normalized, anti-symmetric wavefunction for our 1D Helium atom:

$$\Psi_-(x_1, x_2) = \frac{1}{\sqrt{2}} [ \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1) ]$$

---

You are doing wonderfully. We've built the states from scratch and properly satisfied the laws of identical particles.

Usually, the next step in a problem like this is to introduce the concept of "Spin" to complete the picture of the electron, or to calculate the actual energy of this state. What does the next part of the exam paper hold for us?