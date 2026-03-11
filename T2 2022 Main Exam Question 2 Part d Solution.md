

Welcome back! Let's crack the final pieces of this puzzle together. These last two questions shift our focus from the shape of the wavefunction to the energy levels of the system. This is where quantum mechanics gets really powerful!

First, let's translate the questions so we know exactly what we are tackling:

- **Question 2:** Spectrum of $\hat{H}$: At what energy does the continuous spectrum begin? [1 Pkt.]
    
- **Question 3:** Is $E_0$ higher or lower than the ground state energy of the finite potential well with $V_{\text{topf}}(x) = 0$ for $-1 \le x \le 1$, and $2$ otherwise? Justify your answer. [2 Pkt.]
    

Let's break these down one by one with plenty of detail.

---

### Part 2: The Continuous Spectrum

In quantum mechanics, a system's energy spectrum can be divided into two main types:

1. **Discrete Spectrum (Bound States):** The particle is trapped in a potential well. It cannot escape to infinity, and its energy is restricted to specific, quantized levels (like steps on a ladder).
    
2. **Continuous Spectrum (Scattering States):** The particle has enough energy to overcome the potential barriers and escape to infinity. Its energy is not restricted to specific values; it can take on any value above a certain threshold.
    

To find where the continuous spectrum begins, we need to ask: **"How much energy does the particle need to escape to infinity?"**

Let's look at the asymptotic behavior (what happens as $x$ gets extremely large) of our original potential $V(x)$:

- As $x \rightarrow +\infty$, the potential $V(x) = 2x^2$ grows to $+\infty$. The particle can _never_ escape to the right, no matter how much energy it has. It will always eventually hit a wall.
    
- As $x \rightarrow -\infty$, the potential flattens out to a constant barrier: $V(x) = 2$.
    

If the particle has an energy $E < 2$, it bounces back from the left barrier and is trapped (a bound state). But, the moment the particle's energy reaches $E = 2$, it can "surf" over the left barrier and travel off to $-\infty$ as a free wave.

Therefore, the continuous spectrum begins exactly at the lowest asymptotic value of the potential.

**Answer for your exam:** The continuous spectrum begins at **$E = 2$**.

---

### Part 3: Comparing Ground State Energies

This is a fantastic question that tests your understanding of the **Variational Principle**, or simply your physical intuition about how confining a particle affects its energy.

We are asked to compare the ground state energy of our original system ($E_0$) with the ground state energy of a new, finite potential well (let's call it $E_{\text{topf}}$).

Let's compare the shapes of the two "rooms" the particle can live in:

**The New "Topf" (Well) Potential, $V_{\text{topf}}(x)$:**

- $x < -1$: $V = 2$
    
- $-1 \le x \le 1$: $V = 0$ (A nice, wide, flat floor)
    
- $x > 1$: $V = 2$
    

**Our Original Potential, $V(x)$:**

- $x < -1$: $V = 2$
    
- $-1 \le x \le 0$: $V = 0$ (A narrower flat floor)
    
- $0 < x \le 1$: $V = 2x^2$ (A sloping wall that grows from 0 to 2)
    
- $x > 1$: $V = 2x^2$ (Continues to grow past 2)
    

Notice what happens when we lay them on top of each other.

- On the left side ($x \le 0$), the two potentials are identical.
    
- On the right side ($x > 0$), our original potential $V(x)$ slopes up immediately, whereas the new potential $V_{\text{topf}}$ stays flat at $0$ all the way to $x=1$ before jumping up.
    

Mathematically, this means that for every single point in space, our original potential is greater than or equal to the new potential:

$$V(x) \ge V_{\text{topf}}(x)$$

**The Physical Justification:**

Because $V(x)$ is "tighter" and "steeper" than $V_{\text{topf}}(x)$, it restricts the particle more. According to the Heisenberg Uncertainty Principle, if you squeeze a particle into a smaller space (less uncertainty in position), its momentum must fluctuate more wildly (greater uncertainty in momentum), which directly increases its kinetic energy. Furthermore, because the potential energy function itself is physically higher, the average potential energy is also higher.

There is a rigorous theorem in quantum mechanics that states: if you add a positive perturbation to a potential, the energy levels must increase. Since we can think of $V(x)$ as $V_{\text{topf}}(x)$ plus some extra positive "padding" on the right side, the energy must go up.

**Answer for your exam:** $E_0$ is **higher** than the ground state energy of the finite potential well. This is because the original potential $V(x)$ is everywhere greater than or equal to $V_{\text{topf}}(x)$. The original potential "pinches" the wave function more on the right side (where $2x^2 > 0$ for $x \in (0,1]$ and $2x^2 > 2$ for $x>1$), resulting in tighter spatial confinement and higher average potential energy, both of which raise the total ground state energy.

---

Would you like to review how to apply the variational principle mathematically to prove this energy shift, or shall we move on to a completely new quantum system?