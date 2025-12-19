

Let's keep this momentum going! We are now at the stage where we actually "solve" the quantum system.

In **Part (3c)**, we need to find two things:

1.  **The Eigenfunctions ($\psi_{m,n}$):** The specific shapes the waves take inside the box.
    
2.  **The Eigenenergies ($E_{m,n}$):** The specific energy levels the particle is allowed to have.
    

We will use the decoupled equations we found in the previous step.

---

### Step 1: Solving the 1D Wave Equation

From Part (3b), we know that the X-part of the wave, $\phi(x)$, must satisfy:

$$-\frac{\hbar^2}{2M} \frac{d^2 \phi}{dx^2} = E_x \phi(x)$$

We can rewrite this in a more familiar oscillator form:

$$\frac{d^2 \phi}{dx^2} + k_x^2 \phi(x) = 0 \quad \text{where} \quad k_x^2 = \frac{2ME_x}{\hbar^2}$$

The general mathematical solution to this differential equation involves sines and cosines:

$$\phi(x) = A \sin(k_x x) + B \cos(k_x x)$$

Now, we apply the **Boundary Conditions** (the walls of the box).

1.  At $x=0$: The wavefunction must be zero because the wall is infinite.
    
    $$\phi(0) = A \sin(0) + B \cos(0) = 0$$
    
    $$0 + B(1) = 0 \quad \Rightarrow \quad B=0$$
    
    So, we can throw away the cosine part. We are left with $\phi(x) = A \sin(k_x x)$.
    
2.  At $x=a$: The wavefunction must also be zero at the other wall.
    
    $$\phi(a) = A \sin(k_x a) = 0$$
    
    Since $A$ cannot be zero (otherwise the particle doesn't exist!), the sine term must be zero.
    
    $$\sin(k_x a) = 0$$
    
    This is only true if the argument is an integer multiple of $\pi$.
    
    $$k_x a = m \pi \quad \Rightarrow \quad k_x = \frac{m \pi}{a}$$
    
    (Where $m = 1, 2, 3...$ We call this a quantum number.)
    

By the exact same logic for the $y$-direction, we get:

$$k_y = \frac{n \pi}{a} \quad \text{with quantum number } n = 1, 2, 3...$$

So, our unnormalized wavefunction is:

$$\psi(x,y) = N \sin\left(\frac{m \pi x}{a}\right) \sin\left(\frac{n \pi y}{a}\right)$$

---

### Step 2: Normalization (Finding $N$)

The problem asks for "normierte" (normalized) functions. This means the total probability of finding the particle _somewhere_ in the box must be $1$ (or $100\%$).

$$\int_{0}^{a} \int_{0}^{a} |\psi(x,y)|^2 \, dx \, dy = 1$$

Substitute our function:

$$N^2 \left( \int_{0}^{a} \sin^2\left(\frac{m \pi x}{a}\right) dx \right) \left( \int_{0}^{a} \sin^2\left(\frac{n \pi y}{a}\right) dy \right) = 1$$

Let's evaluate the first integral. The hint says $\int_0^{\pi} \sin^2(x) dx = \pi/2$, but our limits are 0 to $a$. The standard result for a sine squared integral over exactly half a period (which fits in the box) is half the width of the box. So:

$$\int_{0}^{a} \sin^2\left(\frac{m \pi x}{a}\right) dx = \frac{a}{2}$$

_(If you want to use the hint formally: substitute $u = \frac{m \pi x}{a}$, $dx = \frac{a}{m\pi} du$. The integral becomes $\frac{a}{m\pi} \int_0^{m\pi} \sin^2 u \, du = \frac{a}{m\pi} (m \cdot \frac{\pi}{2}) = \frac{a}{2}$)_.

Plugging this back into our normalization equation:

$$N^2 \cdot \left(\frac{a}{2}\right) \cdot \left(\frac{a}{2}\right) = 1$$

$$N^2 \frac{a^2}{4} = 1 \quad \Rightarrow \quad N = \sqrt{\frac{4}{a^2}} = \frac{2}{a}$$

Result 1: The Normalized Eigenfunctions

$$\psi_{m,n}(x,y) = \frac{2}{a} \sin\left(\frac{m \pi x}{a}\right) \sin\left(\frac{n \pi y}{a}\right)$$

---

### Step 3: Calculating the Eigenenergies

Finally, we need the energy $E$. Recall from the very beginning that $E = E_x + E_y$.

We defined $k_x^2 = \frac{2ME_x}{\hbar^2}$. Rearranging for energy gives:

$$E_x = \frac{\hbar^2 k_x^2}{2M}$$

Substitute our quantized $k_x = \frac{m \pi}{a}$:

$$E_x = \frac{\hbar^2}{2M} \left(\frac{m \pi}{a}\right)^2 = \frac{\hbar^2 \pi^2 m^2}{2Ma^2}$$

Similarly for $y$:

$$E_y = \frac{\hbar^2 \pi^2 n^2}{2Ma^2}$$

Adding them together gives the total energy:

Result 2: The Eigenenergies

$$E_{m,n} = \frac{\hbar^2 \pi^2}{2Ma^2} (m^2 + n^2)$$

(Where $m, n \in \mathbb{N} = \{1, 2, 3, ...\}$)

### Summary for the Student

You now have the complete solution for the particle in the 2D box!

1.  **The waves** look like grid patterns of humps and valleys (sine waves in 2 directions).
    
2.  **The energies** are discrete. You can't just give the particle _any_ energy; it must fit this formula based on integers $m$ and $n$.
    

Ready for the next part? I assume we might look at the ground state or maybe degeneracy next!