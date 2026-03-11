

It has been a pleasure being your "AI Professor" for this lesson! You've navigated some of the most fundamental concepts in quantum mechanics—from the curvature of wavefunctions to the nature of energy spectra.

To help you prepare for your exam, here is a structured "Cheat Sheet" summarizing the logic we used to solve these problems.

---

## 🧠 The Quantum Qualitative Cheat Sheet

### 1. The Master Equation for Curvature

To understand the shape of a wavefunction $\Phi(x)$, always look at the Time-Independent Schrödinger Equation rearranged for the second derivative:

$$\Phi''(x) = 2(V(x) - E)\Phi(x)$$

Assuming the ground state $\Phi(x)$ is positive:

- **Classically Allowed ($E > V$):** $\Phi''(x)$ and $\Phi(x)$ have opposite signs. The function is **concave** (curves toward the axis), creating oscillations or a "hump".
    
- **Classically Forbidden ($E < V$):** $\Phi''(x)$ and $\Phi(x)$ have the same sign. The function is **convex** (curves away from the axis), creating exponential decay.
    
- **Turning Point ($E = V$):** $\Phi''(x) = 0$. This is an **inflection point** where the curvature flips.
    

---

### 2. Asymptotic Behavior (The "Tails")

Wavefunctions must be normalizable, meaning they must go to zero at infinity.

- **Constant Potential Barrier ($V = V_0$):** Simple exponential decay: $\Phi(x) \approx A e^{-\kappa |x|}$, where $\kappa = \sqrt{2(V_0 - E)}$.
    
- **Harmonic/Parabolic Potential ($V \propto x^2$):** Rapid Gaussian decay: $\Phi(x) \approx C e^{-cx^2}$.
    

---

### 3. Wavelength and Amplitude Dynamics

In the continuous spectrum ($E > V_{\text{min}}$):

| Feature | Physical Cause | Mathematical Relation |

| :--- | :--- | :--- |

| **Wavelength ($\lambda$)** | High kinetic energy = more wiggles | $\lambda \propto \frac{1}{\sqrt{E - V(x)}}$ |

| **Amplitude ($A$)** | Faster particles are less likely to be "found" in one spot | $A \propto \frac{1}{\sqrt[4]{E - V(x)}}$ |

- **Rule of Thumb:** If $V(x)$ increases, the particle slows down $\rightarrow$ $\lambda$ increases and $A$ increases.
    

---

### 4. Energy and Spectra

- **Continuous Spectrum:** Begins at the lowest value of $V(x)$ as $x \rightarrow \pm\infty$. If $E$ is above this limit, the particle can escape to infinity.
    
- **Ground State Energy ($E_0$):** Always sits above the minimum of the potential ($E_0 > V_{\text{min}}$) due to the Uncertainty Principle.
    
- **Comparison Rule:** If you make a potential well narrower or shallower (increasing $V(x)$ somewhere), the energy levels will shift **upward**.
    

---

### 5. Symmetry and Maxima

- **Ground State:** Always has **zero nodes** (never crosses the x-axis).
    
- **Peak Position:** The maximum of the wavefunction "prefers" the region with the lowest potential energy.
    
- **Derivative Logic:** If the peak is to the left of a point (like $x=0$), the derivative at that point must be negative as the function decays toward the right.
    

---

**Would you like me to generate a practice problem with a different potential shape so you can test your "cheat sheet" logic?**