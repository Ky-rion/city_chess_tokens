

Creating a cheat sheet is a brilliant idea. A huge part of mastering theoretical physics is organizing your toolkit so you don't have to derive every single formula from scratch during an exam.

Here is a consolidated summary of all the key formulas, tricks, and concepts we used to conquer this problem set. I have bolded the absolute most important takeaways.

---

### 1. Quantum Numbers & Energy (in Atomic Units)

Atomic units are your best friend here. They set fundamental constants (like the electron mass and Planck's constant) to 1, stripping away the clutter.

- **Energy Levels of Hydrogen:**
    
    $$E_n = -\frac{1}{2n^2}$$
    
- **Principal Quantum Number ($n$):** Determines the energy level or "shell".
    
    Allowed values: $n = 1, 2, 3, \dots$
    
- **Orbital/Azimuthal Quantum Number ($l$):** Determines the 3D shape of the orbital.
    
    Allowed values: $l = 0, 1, 2, \dots, (n - 1)$
    
- **Magnetic Quantum Number ($m$):** Determines the orientation of the orbital in space.
    
    Allowed values: $m = -l, \dots, 0, \dots, +l$
    

### 2. Quantum Integrals & Expectation Values

When you are asked for an expectation value (average), you are integrating over a probability distribution.

- **General Expectation Value Formula:**
    
    $$\langle A \rangle = \int_{\text{all space}} \Psi^*(\vec{r}) \hat{A} \Psi(\vec{r}) \, dV$$
    
- **Spherical Coordinates Volume Element ($dV$):** You cannot just use $dx \, dy \, dz$ for round atoms!
    
    $$dV = r^2 \sin\theta \, dr \, d\theta \, d\phi$$
    
    _(Integration limits: $r$ from $0$ to $\infty$, $\theta$ from $0$ to $\pi$, $\phi$ from $0$ to $2\pi$)_
    
- **The "Handy" Gamma Integral:** Memorize this! It saves you from doing integration by parts multiple times.
    
    $$\int_0^\infty x^n e^{-ax} \, dx = \frac{n!}{a^{n+1}}$$
    

### 3. The Power of Spherical Symmetry

If the problem specifies an **s-orbital** (where $l=0$, like the ground state), the electron cloud is a perfect sphere. The physics in the $x, y$, and $z$ directions are entirely identical.

- **Position Shortcut:**
    
    $$r^2 = x^2 + y^2 + z^2 \implies \langle x^2 \rangle = \frac{\langle r^2 \rangle}{3}$$
    
- **Momentum Shortcut:**
    
    $$\vec{P}^2 = \hat{P}_x^2 + \hat{P}_y^2 + \hat{P}_z^2 \implies \langle \hat{P}_x^2 \rangle = \frac{\langle \vec{P}^2 \rangle}{3}$$
    
- **Symmetric Averages:** Because the electron is equally likely to be at $+x$ as $-x$, or move left vs. right, the linear averages are always zero:
    
    $\langle x \rangle = 0$ and $\langle \hat{P}_x \rangle = 0$
    

### 4. Energy & The Virial Theorem

The Virial Theorem is the ultimate shortcut for relating kinetic and potential energy in bound systems without doing any calculus.

- **Total Energy Equation:**
    
    $$E = \langle \hat{T} \rangle + \langle \hat{V} \rangle$$
    
- **The Virial Theorem (for Coulomb potentials):**
    
    $$2\langle \hat{T} \rangle = -\langle \hat{V} \rangle$$
    
- **The Virial Shortcut:** Substituting the theorem into the energy equation always yields:
    
    $$E = -\langle \hat{T} \rangle$$
    
- **Kinetic Energy to Momentum:** In atomic units (where mass $m=1$), kinetic energy relates to momentum perfectly:
    
    $$\langle \hat{T} \rangle = \frac{\langle \vec{P}^2 \rangle}{2}$$
    

### 5. The Heisenberg Uncertainty Principle

"Uncertainty" in quantum mechanics is strictly defined as the standard deviation of a set of measurements.

- **Quantum Uncertainty Formula:**
    
    $$\Delta A = \sqrt{\langle \hat{A}^2 \rangle - \langle \hat{A} \rangle^2}$$
    
- **Position-Momentum Uncertainty Limit:**
    
    $$\Delta x \Delta p_x \ge \frac{\hbar}{2}$$
    
    _(Note: In atomic units, $\hbar = 1$, so the absolute minimum limit is simply $1/2$.)_
    

---

This sheet contains virtually everything you need to navigate standard hydrogen atom expectation value problems!

Would you like me to generate a brand new, unseen practice question right now so you can test drive this cheat sheet and see how it holds up?