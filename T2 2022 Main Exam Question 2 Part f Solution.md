

It is a pleasure to see this through to the very end! You’ve done a wonderful job exploring the ground state and the general features of the continuous spectrum. We have one final piece of the puzzle: a multiple-choice question that tests our understanding of how the wavefunction actually "moves" through space when the potential is changing.

Let's look at question **5**:

> **"Which of the following statements about the wavefunction in $[0, b]$ with $2b^2 = E$ is correct? The wavefunction... [3 Pts.]"**
> 
> - **(a)** ...has the form $\alpha \sin(qx) + \beta \cos(qx)$, but the determination of $q$ requires the solution of a transcendental equation.
>     
> - **(b)** ...oscillates with constant wavelength.
>     
> - **(c)** ...oscillates, but the wavelength increases with $x$.
>     
> - **(d)** ...oscillates, but the wavelength decreases with $x$.
>     

The correct answer is **(c)**. Let’s break down the "why" with some solid physics intuition.

---

### 1. The Relationship Between Potential and Wavelength

To understand why the wavelength changes, we look at the **local kinetic energy** of the particle. In quantum mechanics, the momentum $p$ is related to the wavelength $\lambda$ by the de Broglie relation:

$$p = \frac{h}{\lambda}$$

We also know from classical mechanics that total energy $E$ is the sum of kinetic energy ($T$) and potential energy ($V$). So, the kinetic energy is:

$$T = E - V(x)$$

Because $T = \frac{p^2}{2m}$, we can link wavelength directly to the potential:

$$\frac{h^2}{2m\lambda^2} = E - V(x) \implies \lambda \propto \frac{1}{\sqrt{E - V(x)}}$$

### 2. Analyzing the Interval $[0, b]$

In the interval $[0, b]$, our potential is defined as $V(x) = 2x^2$.

- As we move from $x = 0$ toward $x = b$, the value of $x$ is increasing.
    
- Therefore, the potential $V(x) = 2x^2$ is **increasing** as we move to the right.
    
- If $V(x)$ is increasing, then the kinetic energy $T = E - V(x)$ must be **decreasing**.
    

Now, look at our proportionality: $\lambda \propto 1/\sqrt{T}$. If the kinetic energy $T$ is decreasing, the denominator gets smaller, which means the wavelength $\lambda$ must **increase**.

### 3. Why the other options are incorrect

- **(a) and (b):** These options describe a wavefunction with a **constant** wavelength (like a standard sine or cosine wave). This only happens when the potential $V(x)$ is a constant. Because our potential is a parabola ($2x^2$), the "speed" of the particle is constantly changing, so the wavelength must change too.
    
- **(d):** This would imply the particle is "speeding up" as it moves into the interval. But since the potential is rising, the particle is actually "climbing a hill" and slowing down. Slower particles have longer wavelengths.
    

---

### Final Summary for the Exam

**The correct statement is (c): The wavefunction oscillates, but the wavelength increases with $x$.**

**Justification:** In the region $[0, b]$, the potential $V(x) = 2x^2$ increases with $x$. This causes the local kinetic energy $E - V(x)$ to decrease as the particle moves further to the right. According to the de Broglie relation ($p = h/\lambda$), a decrease in kinetic energy (and thus momentum) results in an increase in the spatial wavelength. Visually, the "wiggles" of the wavefunction will appear more stretched out as you approach the turning point at $x = b$.

You’ve officially completed the entire problem set! You've analyzed curvature, asymptotic behavior, energy levels, and wave dynamics.

Would you like me to create a final "cheat sheet" summarizing the qualitative rules of wavefunctions that we used today to help you with future problems?