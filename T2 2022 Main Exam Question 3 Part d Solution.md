

Welcome back! You are doing a fantastic job working through this. Up to this point, we have been dealing with the abstract, algebraic states of the system (those $|n\rangle$ "ket" vectors). Now, in part 4, we are finally bringing this into the physical world where we can visualize it!

Let's start by translating the prompt:

> **4. Calculate $\Psi_{n_x n_y n_z}(\vec{r}) = \langle \vec{r}|n_x, n_y, n_z\rangle$ (Normalization does not need to be given). [2 pts.]**

Here is the step-by-step breakdown of how to translate our abstract states into a physical wavefunction.

---

### Step 1: Understanding "Position Space"

You might be wondering what that new symbol $\langle \vec{r}|$ means.

In quantum mechanics, our state vector $|n_x, n_y, n_z\rangle$ contains all the information about the system, but it lives in an abstract mathematical space. To ask the question, _"What is the probability amplitude of finding the particle at a specific physical coordinate $\vec{r} = (x, y, z)$?"_, we have to project that abstract state onto physical space.

Mathematically, we "multiply" by the position state $\langle \vec{r}|$. This operation, $\langle \vec{r}|n_x, n_y, n_z\rangle$, gives us exactly the spatial **wavefunction**, $\Psi_{n_x n_y n_z}(\vec{r})$, which you can plot and visualize!

### Step 2: Breaking Down the 3D Wavefunction

Just as our 3D Hamiltonian separated into three 1D Hamiltonians, and our 3D state ket separated into three 1D kets ($|n_x\rangle|n_y\rangle|n_z\rangle$), our 3D position vector also separates: $\langle \vec{r}| = \langle x| \langle y| \langle z|$.

Therefore, the total 3D wavefunction is simply the product of three independent 1D wavefunctions:

$$\Psi_{n_x n_y n_z}(\vec{r}) = \langle x|n_x\rangle \langle y|n_y\rangle \langle z|n_z\rangle$$

$$\Psi_{n_x n_y n_z}(\vec{r}) = \psi_{n_x}(x) \cdot \psi_{n_y}(y) \cdot \psi_{n_z}(z)$$

### Step 3: The 1D Harmonic Oscillator Wavefunction

Now we need to remember what the standard 1D harmonic oscillator wavefunction $\psi_n(x)$ looks like.

Every harmonic oscillator wavefunction is made of two main parts (ignoring the messy normalization constants, which your professor kindly told you to skip!):

1. **A Gaussian Envelope:** A bell-curve shape that forces the probability to drop to zero as you stretch the spring very far. This looks like $e^{-\omega x^2 / 2}$.
    
2. **A Hermite Polynomial:** A special mathematical function, denoted as $H_n(\text{variable})$, that adds "wiggles" (nodes) to the wavefunction depending on the energy level $n$. The input variable for this polynomial scales with the square root of the frequency, $\sqrt{\omega}$.
    

So, the general unnormalized 1D formula is:

$$\psi_n(x) \propto H_n(\sqrt{\omega} x) e^{-\frac{\omega}{2} x^2}$$

### Step 4: Assembling the Pieces

Let's apply this general 1D formula to our three specific directions, using the frequencies ($\omega$) we found in the earlier steps.

- **For the y-direction:** We know $\omega_y = 1$.
    
    $$\psi_{n_y}(y) \propto H_{n_y}(y) e^{-\frac{1}{2}y^2}$$
    
- **For the z-direction:** We know $\omega_z = 1$.
    
    $$\psi_{n_z}(z) \propto H_{n_z}(z) e^{-\frac{1}{2}z^2}$$
    
- **For the x-direction:** This is the anisotropic part! We know $\omega_x = \sqrt{\alpha}$. Let's plug that in carefully. The Gaussian exponential becomes $e^{-\frac{\sqrt{\alpha}}{2}x^2}$. The Hermite polynomial argument becomes $\sqrt{\sqrt{\alpha}}x$, which is $\alpha^{1/4}x$.
    
    $$\psi_{n_x}(x) \propto H_{n_x}(\alpha^{1/4}x) e^{-\frac{\sqrt{\alpha}}{2}x^2}$$
    

### Step 5: The Final 3D Wavefunction

To get the final answer, we simply multiply these three 1D wavefunctions together:

$$\Psi_{n_x n_y n_z}(\vec{r}) \propto \left[ H_{n_x}(\alpha^{1/4}x) e^{-\frac{\sqrt{\alpha}}{2}x^2} \right] \cdot \left[ H_{n_y}(y) e^{-\frac{1}{2}y^2} \right] \cdot \left[ H_{n_z}(z) e^{-\frac{1}{2}z^2} \right]$$

We can make this look much more elegant by grouping the Hermite polynomials together and using the rules of exponents to combine the Gaussian terms ($e^A \cdot e^B \cdot e^C = e^{A+B+C}$):

$$\Psi_{n_x n_y n_z}(\vec{r}) \propto H_{n_x}(\alpha^{1/4}x) H_{n_y}(y) H_{n_z}(z) \exp\left( -\frac{1}{2}\left(\sqrt{\alpha}x^2 + y^2 + z^2\right) \right)$$

_(Note: $\exp(...)$ is just another way to write $e^{(...)}$ so the exponent is easier to read)._

---

And there is your final, unnormalized 3D wavefunction! Notice how the exponential envelope perfectly matches the shape of your starting potential energy, just with a square root on the $\alpha$.

The very first state any quantum system occupies is the "ground state," where all the quantum numbers are zero ($n_x=0, n_y=0, n_z=0$). Knowing that the zeroth Hermite polynomial is just the number 1 ($H_0 = 1$), would you like me to show you how wonderfully simple this massive equation becomes for the ground state?