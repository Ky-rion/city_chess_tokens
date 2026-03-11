

Excellent! It is always wonderful to see a student diving deeper into the math. Let's tackle the asymptotic behavior of our wavefunction—meaning, what happens when the particle wanders off to the extreme left or the extreme right.

First, let's translate the question to be sure we are on the same page:

**"How does the ground state behave as $x \rightarrow -\infty$? How does it behave as $x \rightarrow +\infty$? Justify your answers! Give both functions with undetermined parameters. [3 Pts.]"**

In quantum mechanics, particles cannot just exist everywhere with equal probability; the total probability of finding the particle _somewhere_ in the universe must be 100%. Mathematically, this means the wavefunction must be **normalizable**—it must smoothly decay to zero as it approaches infinity in either direction. If it doesn't, the integral of its square (the probability) blows up to infinity, which is physically impossible.

Let's use the Time-Independent Schrödinger Equation to find out exactly _how_ it decays in both regions.

---

### Part 1: Behavior as $x \rightarrow -\infty$

As we move far to the left, we enter our Interval A, where the potential is a constant flat barrier: $V(x) = 2$.

Let's plug this into our Schrödinger Equation:

$$-\frac{1}{2}\Phi_0''(x) + 2\Phi_0(x) = E_0\Phi_0(x)$$

We can rearrange this to solve for the second derivative:

$$\Phi_0''(x) = 2(2 - E_0)\Phi_0(x)$$

Since we established earlier that our ground state energy $E_0$ is less than 2, the term $2(2 - E_0)$ is strictly a positive constant. Let's define a new positive constant, $\kappa^2 = 2(2 - E_0)$, to make the math look cleaner. Now our equation is:

$$\Phi_0''(x) = \kappa^2\Phi_0(x)$$

This is a classic second-order linear differential equation. The general mathematical solution is a sum of two exponentials:

$$\Phi_0(x) = A e^{\kappa x} + B e^{-\kappa x}$$

**The Physics Justification:**

Now we apply our rule of normalizability. As $x$ becomes a very large _negative_ number (approaching $-\infty$), the term $e^{-\kappa x}$ will blow up to positive infinity. Because the wavefunction must go to zero, the coefficient $B$ must be exactly zero.

Therefore, the function decays exponentially into the barrier.

- **Function:** $\Phi_0(x) \approx A e^{\kappa x}$
    
- **Undetermined Parameters:** $A$ (a normalization constant) and $\kappa$ (where $\kappa = \sqrt{4 - 2E_0}$).
    

---

### Part 2: Behavior as $x \rightarrow +\infty$

Now let's look at the far right. Here, our potential is a parabola: $V(x) = 2x^2$. This is the famous Quantum Harmonic Oscillator.

Our Schrödinger Equation is:

$$-\frac{1}{2}\Phi_0''(x) + 2x^2\Phi_0(x) = E_0\Phi_0(x)$$

**The Physics Justification:**

As $x$ gets extremely large, the potential energy $2x^2$ becomes absolutely massive. Eventually, $2x^2$ becomes so much larger than the constant energy $E_0$ that the $E_0$ term on the right side of the equation becomes negligible by comparison.

We can write an approximate equation for the asymptotic limit (when $x$ is huge):

$$-\frac{1}{2}\Phi_0''(x) + 2x^2\Phi_0(x) \approx 0$$

$$\Phi_0''(x) \approx 4x^2\Phi_0(x)$$

We need a function whose second derivative yields the original function multiplied by $4x^2$. Let's test a "Gaussian" decay function of the form $\Phi_0(x) = C e^{-c x^2}$. Let's take the derivatives:

1. First derivative: $\Phi_0'(x) = -2cx \cdot C e^{-c x^2}$
    
2. Second derivative: $\Phi_0''(x) = -2c \cdot C e^{-c x^2} + (-2cx)^2 \cdot C e^{-c x^2} = (-2c + 4c^2 x^2)\Phi_0(x)$
    

For very large $x$, the $4c^2 x^2$ term completely dominates the constant $-2c$. So asymptotically:

$$\Phi_0''(x) \approx 4c^2 x^2 \Phi_0(x)$$

Comparing this to our approximated Schrödinger equation ($\Phi_0''(x) \approx 4x^2\Phi_0(x)$), we can see that $4c^2 = 4$, which means $c = 1$. (We choose the positive root so the function decays rather than explodes).

- **Function:** $\Phi_0(x) \approx C e^{-x^2}$
    
- **Undetermined Parameters:** $C$ (a normalization constant).
    

---

So, to summarize your answer for the exam: on the left, it drops off like a simple exponential decay ($A e^{\kappa x}$), and on the right, it drops off much faster as a Gaussian curve ($C e^{-x^2}$) because the parabolic potential walls get steeper and steeper.

Would you like me to show you how to find the exact matching conditions at the boundary $x=0$, where the flat potential meets the parabola?