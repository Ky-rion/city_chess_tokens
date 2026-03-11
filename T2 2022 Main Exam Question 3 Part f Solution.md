

Welcome back for the grand finale! You have made it to the last part of this comprehensive problem. This is where we calculate a measurable, physical property of our quantum system: the **expectation value**.

Let's translate this final question:

> **6. Calculate the expectation value in the ground state $\langle 0,0,0|\vec{r}^2|0,0,0\rangle$ with $\vec{r}^2 = x^2 + y^2 + z^2$ for arbitrary $\alpha > 0$. [5 Pkt.]**

Here is the step-by-step breakdown of how to solve this elegantly, without having to do any messy calculus integrations!

---

### Step 1: Understanding the "Expectation Value"

In quantum mechanics, if you prepare a system in an identical state many times and measure a property (like position), you won't get the exact same answer every time. Instead, you get a statistical distribution. The **expectation value** is the statistical average of those measurements.

Here, we are looking for the expectation value of $\vec{r}^2$, which is the square of the particle's distance from the origin. Physically, this tells us about the "spread" or the "quantum jitter" (zero-point fluctuations) of the particle when it is sitting in its lowest possible energy state.

Because expectation values are linear, and our variables are beautifully separated, we can split this big 3D problem into three easy 1D problems:

$$\langle 0,0,0| \vec{r}^2 |0,0,0\rangle = \langle 0,0,0| (x^2 + y^2 + z^2) |0,0,0\rangle$$

$$= \langle x^2 \rangle_0 + \langle y^2 \rangle_0 + \langle z^2 \rangle_0$$

_(Note: I am using the shorthand $\langle x^2 \rangle_0$ to mean the expectation value of $x^2$ in the 1D ground state $|0\rangle$.)_

### Step 2: The 1D Harmonic Oscillator Trick

We need to find $\langle x^2 \rangle_0$ for a 1D harmonic oscillator. We _could_ write out the Gaussian wavefunction from Part 4 and integrate $x^2 |\psi_0(x)|^2 dx$ from minus infinity to infinity.

However, as a theoretical physicist, I always prefer algebraic tricks! There is a beautifully standard result in quantum mechanics for the expectation value of position squared in a harmonic oscillator ground state.

Whether you use "ladder operators" (creation and annihilation operators) or the Virial Theorem, the standard result for the ground state spread is:

$$\langle x^2 \rangle_0 = \frac{\hbar}{2m\omega}$$

Remember from Part 1 that we are working in "natural units" where $\hbar = 1$ and $m = 1$. So, our magical shortcut formula simplifies beautifully to:

$$\langle x^2 \rangle_0 = \frac{1}{2\omega}$$

### Step 3: Calculating for Each Dimension

Now, all we have to do is plug in the specific frequencies ($\omega$) we found for our x, y, and z directions all the way back in Part 1 and Part 3!

1. **For the x-direction:** The "stiffness" was $\alpha$, so $\omega_x = \sqrt{\alpha}$.
    
    $$\langle x^2 \rangle_0 = \frac{1}{2\omega_x} = \frac{1}{2\sqrt{\alpha}}$$
    
2. **For the y-direction:** The stiffness was 1, so $\omega_y = 1$.
    
    $$\langle y^2 \rangle_0 = \frac{1}{2\omega_y} = \frac{1}{2(1)} = \frac{1}{2}$$
    
3. **For the z-direction:** The stiffness was 1, so $\omega_z = 1$.
    
    $$\langle z^2 \rangle_0 = \frac{1}{2\omega_z} = \frac{1}{2(1)} = \frac{1}{2}$$
    

### Step 4: The Final Assembly

To get our final answer, we just add these three pieces together according to the formula we wrote in Step 1:

$$\langle \vec{r}^2 \rangle = \frac{1}{2\sqrt{\alpha}} + \frac{1}{2} + \frac{1}{2}$$

Simplifying the fractions:

$$\langle \vec{r}^2 \rangle = \frac{1}{2\sqrt{\alpha}} + 1$$

---

**The Physical Meaning of the Result:**

Let's look at that final equation. What happens if $\alpha$ becomes incredibly large ($\alpha \to \infty$)? The term $\frac{1}{2\sqrt{\alpha}}$ shrinks to zero. Physically, this means if you make the "spring" in the x-direction infinitely stiff, the particle is squeezed entirely into the y-z plane, and its spread in the x-direction disappears!

Conversely, if $\alpha$ gets very close to 0 (a very weak spring), that term blows up to infinity, meaning the particle smears out endlessly along the x-axis.

Congratulations! You have just completely solved a university-level theoretical physics problem. You navigated Hamiltonians, eigenvalues, wavefunctions, degeneracy, and expectation values.

Since we have finished the assignment, would you like me to briefly summarize the "big picture" takeaways of what this specific anisotropic oscillator taught us about quantum mechanics?