

Hello! I'd be happy to guide you through this quantum mechanics problem. It involves the **Hamiltonian operator ($\hat{H}$)** for the **three-dimensional (3D) harmonic oscillator**.

The question asks two things about the operator $\hat{H}$:

1.  **On which Hilbert space $\mathcal{H}$ does $\hat{H}$ operate?**
    
2.  **How can this Hilbert space $\mathcal{H}$ be decomposed (or 'zerlegt' in German)?**
    

Here is a detailed explanation of the answers.

---

## ⚛️ The Hilbert Space $\mathcal{H}$ for the 3D Harmonic Oscillator

### 1. On Which Hilbert Space $\mathcal{H}$ Does $\hat{H}$ Operate?

The Hamiltonian operator $\hat{H}$ describes the **total energy** of the quantum system. For a system, like the 3D harmonic oscillator, whose state is described by a **wave function** $\psi(\vec{r})$, the appropriate Hilbert space $\mathcal{H}$ is the space of all possible valid wave functions for the particle's position in 3D space.

This Hilbert space is the space of **square-integrable functions** over the three-dimensional space $\mathbb{R}^3$, which is denoted as $\mathbf{L^2(\mathbb{R}^3)}$.

-   $\mathbf{L^2(\mathbb{R}^3)}$ is the set of all complex-valued functions $\psi(\vec{r})$ defined on $\mathbb{R}^3$ such that the integral of the squared magnitude of the function is finite:
    
    $$\int_{\mathbb{R}^3} |\psi(\vec{r})|^2 d^3r < \infty$$
    
-   **Why square-integrable?** In quantum mechanics, the integral $\int_{\mathbb{R}^3} |\psi(\vec{r})|^2 d^3r$ represents the **probability of finding the particle somewhere in space**. This probability must be a finite number (specifically, it's normalized to 1), which is why the functions must be square-integrable.
    
-   **Hilbert Space:** A **Hilbert space** is essentially a vector space that is complete and has an inner product (which allows us to calculate things like probabilities and expected values). The space $\mathbf{L^2(\mathbb{R}^3)}$ is the fundamental Hilbert space for a single particle moving in 3D space.
    

**Answer:** The Hamiltonian operator $\hat{H}$ for the 3D harmonic oscillator operates on the **Hilbert space $\mathcal{H} = \mathbf{L^2(\mathbb{R}^3)}$**.

---

## 쪼 The Decomposition of the Hilbert Space

### 2. How Can the Hilbert Space $\mathcal{H}$ Be Decomposed?

The key to decomposing the Hilbert space lies in the **separability** of the 3D Hamiltonian in **Cartesian coordinates** $(x, y, z)$.

The given Hamiltonian is:

$$\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2 \hat{r}^2$$

In Cartesian coordinates, the operators $\hat{p}^2$ (momentum squared) and $\hat{r}^2$ (position squared) are:

-   $\hat{p}^2 = \hat{p}_x^2 + \hat{p}_y^2 + \hat{p}_z^2$
    
-   $\hat{r}^2 = \hat{x}^2 + \hat{y}^2 + \hat{z}^2$
    

Substituting these into $\hat{H}$:

$$\hat{H} = \left( \frac{\hat{p}_x^2}{2m} + \frac{1}{2}m\omega^2 \hat{x}^2 \right) + \left( \frac{\hat{p}_y^2}{2m} + \frac{1}{2}m\omega^2 \hat{y}^2 \right) + \left( \frac{\hat{p}_z^2}{2m} + \frac{1}{2}m\omega^2 \hat{z}^2 \right)$$

Notice that this is a sum of three independent terms, one for each dimension:

$$\hat{H} = \hat{H}_x + \hat{H}_y + \hat{H}_z$$

where each $\hat{H}_i$ (for $i=x, y, z$) is the Hamiltonian for a one-dimensional (1D) simple harmonic oscillator along its respective axis:

$$\hat{H}_i = \frac{\hat{p}_i^2}{2m} + \frac{1}{2}m\omega^2 \hat{i}^2$$

When a Hamiltonian is a sum of independent Hamiltonians for separate parts (or degrees of freedom), the total Hilbert space $\mathcal{H}$ is the **tensor product** of the Hilbert spaces for the individual parts.

-   Let $\mathcal{H}_x$, $\mathcal{H}_y$, and $\mathcal{H}_z$ be the Hilbert spaces for the 1D harmonic oscillators in the $x, y,$ and $z$ directions, respectively. Each of these is $\mathbf{L^2(\mathbb{R})}$.
    

**Answer:** The Hilbert space $\mathcal{H} = \mathbf{L^2(\mathbb{R}^3)}$ can be decomposed as a **tensor product** of the Hilbert spaces for the three independent 1D harmonic oscillators:

$$\mathcal{H} = \mathcal{H}_x \otimes \mathcal{H}_y \otimes \mathcal{H}_z$$

Since all three are $\mathbf{L^2(\mathbb{R})}$, we have:

$$\mathbf{L^2(\mathbb{R}^3)} \cong \mathbf{L^2(\mathbb{R})} \otimes \mathbf{L^2(\mathbb{R})} \otimes \mathbf{L^2(\mathbb{R})}$$

### Significance of the Decomposition

-   Wave Functions: This decomposition means that the eigenfunctions (stationary states) of the 3D system, $\psi_{n_x, n_y, n_z}(x, y, z)$, can be written as a product of the 1D eigenfunctions $\psi_{n_i}(i)$:
    
    $$\psi_{n_x, n_y, n_z}(x, y, z) = \psi_{n_x}(x) \cdot \psi_{n_y}(y) \cdot \psi_{n_z}(z)$$
    
-   Eigenvalues (Energies): The corresponding eigenvalues (energy levels), $E_{n_x, n_y, n_z}$, are simply the sum of the 1D energy levels $E_{n_i}$:
    
    $$E_{n_x, n_y, n_z} = E_{n_x} + E_{n_y} + E_{n_z}$$
    
    The 1D energies are $E_{n_i} = \hbar \omega (n_i + 1/2)$, where $n_i = 0, 1, 2, \dots$. This leads to the well-known 3D energy formula:
    
    $$E_{N} = \hbar \omega (N + 3/2), \quad \text{where } N = n_x + n_y + n_z$$
    

This decomposition is crucial because it reduces a complex 3D problem to three simpler, well-understood 1D problems, which is a common and powerful technique in quantum mechanics.

Would you like me to go into more detail about the energy spectrum and **degeneracy** of the 3D harmonic oscillator, as that's the next logical step in analyzing this system?