

Welcome back to our theoretical physics sessions! This is an absolutely beautiful problem because it takes a very abstract mathematical concept (the spectral representation of a Hamiltonian) and applies it to a very physical phenomenon: the decay of a quantum state.

Let's begin by translating the German text into English so we can dissect the physics together:

> **The Hamiltonian operator in spectral representation**
> 
> $$\hat{H}_0 = |b\rangle E_b \langle b| + \int_0^\infty dE |E\rangle E \langle E|, \quad E_b > 0$$
> 
> **describes a bound state in $L^2(dx, [0, \infty))$ with**
> 
> $\langle x|b\rangle = \sqrt{2}e^{-x}$, **which is embedded in a continuum of states** $\langle x|E\rangle = (2\pi)^{-1/2}e^{iEx}$. **Under the influence of a perturbation**
> 
> $$V(x) = 1 \text{ for } |x| < 1, \quad = 0 \text{ otherwise}$$
> 
> **$|b\rangle$ decays. Calculate the decay width $\Gamma$ for the energy $E = E_b$ in lowest order of perturbation theory.**

Let's break this down into manageable steps.

---

### Step 1: The Physics of Fermi's Golden Rule

The problem asks for the decay width $\Gamma$ in the lowest order of perturbation theory. Whenever you hear "decay rate" or "transition to a continuum" in lowest order perturbation theory, your brain should immediately shout: **Fermi's Golden Rule!**

In natural units ($\hbar = 1$), Fermi's Golden Rule states that the transition rate (which is equal to the decay width $\Gamma$) from an initial discrete state $|b\rangle$ to a final continuum state $|E\rangle$ is:

$$\Gamma = 2\pi |\langle E | V | b \rangle|^2 \rho(E)$$

evaluated at the energy of the initial state ($E = E_b$).

_A crucial observation here:_ The prompt writes the continuum part of the Hamiltonian as $\int dE |E\rangle E \langle E|$. Because the integral is directly over $dE$, this tells us the continuum states $|E\rangle$ are _already_ normalized with respect to energy. Therefore, the density of states factor is simply $\rho(E) = 1$.

Our working formula for the decay width is exactly:

$$\Gamma = 2\pi |\langle E_b | V | b \rangle|^2$$

### Step 2: Setting up the Matrix Element Integral

To find $\langle E_b | V | b \rangle$, we need to calculate the overlap integral in position space. Let's look closely at the spatial domain defined in the problem:

1. **The Space:** The problem explicitly states we are in $L^2(dx, [0, \infty))$. This is a very important detail! It means our particle only exists for $x \ge 0$. Any spatial integral we do must have a lower limit of $0$.
    
2. **The Perturbation:** $V(x) = 1$ for $|x| < 1$. Because our space starts at $x=0$, the perturbation is effectively $V(x) = 1$ for the region $x \in [0, 1]$, and zero everywhere else.
    

Now we can set up the integral by inserting a complete set of position states $\int |x\rangle\langle x| dx = 1$:

$$\langle E_b | V | b \rangle = \int_0^\infty \langle E_b | x \rangle V(x) \langle x | b \rangle dx$$

Remember that $\langle E_b | x \rangle$ is the complex conjugate of $\langle x | E_b \rangle$:

$$\langle E_b | x \rangle = \left( \frac{1}{\sqrt{2\pi}} e^{iE_bx} \right)^* = \frac{1}{\sqrt{2\pi}} e^{-iE_bx}$$

Applying the limits of our perturbation $V(x)$, the integral becomes:

$$\langle E_b | V | b \rangle = \int_0^1 \left( \frac{1}{\sqrt{2\pi}} e^{-iE_bx} \right) (1) \left( \sqrt{2} e^{-x} \right) dx$$

### Step 3: Evaluating the Integral

Let's pull the constants out front. The $\sqrt{2}$ in the numerator and denominator combine nicely:

$$\frac{\sqrt{2}}{\sqrt{2\pi}} = \frac{1}{\sqrt{\pi}}$$

Now we combine the exponentials:

$$\langle E_b | V | b \rangle = \frac{1}{\sqrt{\pi}} \int_0^1 e^{-iE_bx - x} dx = \frac{1}{\sqrt{\pi}} \int_0^1 e^{-(1 + iE_b)x} dx$$

This is a straightforward exponential integral $\int e^{cx} dx = \frac{1}{c}e^{cx}$:

$$\langle E_b | V | b \rangle = \frac{1}{\sqrt{\pi}} \left[ \frac{-1}{1 + iE_b} e^{-(1 + iE_b)x} \right]_0^1$$

Evaluate at the limits (upper limit $x=1$, lower limit $x=0$):

$$\langle E_b | V | b \rangle = \frac{1}{\sqrt{\pi}} \left( \frac{-1}{1 + iE_b} e^{-(1 + iE_b)} - \frac{-1}{1 + iE_b} e^0 \right)$$

$$\langle E_b | V | b \rangle = \frac{1}{\sqrt{\pi}} \frac{1 - e^{-(1 + iE_b)}}{1 + iE_b}$$

### Step 4: Calculating the Magnitude Squared

Fermi's Golden Rule requires the absolute square of this matrix element: $|\langle E_b | V | b \rangle|^2$.

To find the absolute square of a complex number $z$, we multiply it by its complex conjugate $z^*$.

$$|z|^2 = \frac{1}{\pi} \left| \frac{1 - e^{-1}e^{-iE_b}}{1 + iE_b} \right|^2$$

Let's do the denominator first, which is easy:

$$|1 + iE_b|^2 = 1^2 + (E_b)^2 = 1 + E_b^2$$

Now for the numerator. Let's use Euler's formula to expand the exponential: $e^{-iE_b} = \cos(E_b) - i\sin(E_b)$.

$$\text{Numerator} = 1 - e^{-1}(\cos E_b - i\sin E_b) = (1 - e^{-1}\cos E_b) + i(e^{-1}\sin E_b)$$

The absolute square of this is the real part squared plus the imaginary part squared:

$$|\text{Numerator}|^2 = (1 - e^{-1}\cos E_b)^2 + (e^{-1}\sin E_b)^2$$

$$= 1 - 2e^{-1}\cos E_b + e^{-2}\cos^2 E_b + e^{-2}\sin^2 E_b$$

Since $\cos^2 \theta + \sin^2 \theta = 1$, the last two terms simplify to $e^{-2}$:

$$|\text{Numerator}|^2 = 1 - 2e^{-1}\cos(E_b) + e^{-2}$$

Putting it all back together, the squared matrix element is:

$$|\langle E_b | V | b \rangle|^2 = \frac{1}{\pi} \left( \frac{1 - 2e^{-1}\cos(E_b) + e^{-2}}{1 + E_b^2} \right)$$

### Step 5: Final Result

Now we just plug this back into our Fermi's Golden Rule formula from Step 1:

$$\Gamma = 2\pi |\langle E_b | V | b \rangle|^2$$

$$\Gamma = 2\pi \cdot \frac{1}{\pi} \left( \frac{1 - 2e^{-1}\cos(E_b) + e^{-2}}{1 + E_b^2} \right)$$

The $\pi$ cancels out perfectly, leaving us with the final answer:

$$\Gamma = 2 \left( \frac{1 - 2e^{-1}\cos(E_b) + e^{-2}}{1 + E_b^2} \right)$$

---

This is a very elegant result! You can see how the finite width of the perturbation $V(x)$ results in an oscillating term $\cos(E_b)$ in the decay width, which is a classic signature of quantum interference at a sharp boundary.

Would you like me to walk you through how we might interpret that oscillating cosine term physically, perhaps by relating it to diffraction or scattering?