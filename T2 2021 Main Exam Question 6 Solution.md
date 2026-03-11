

Welcome back! Let's dive right into this next question. This one is brilliant because it tests whether you have a solid conceptual grasp of quantum principles—like the Uncertainty Principle and the Virial Theorem—rather than just memorizing formulas.

As always, let's translate the German text first to ensure we are looking at the exact same physics:

> **Which of the following statements are correct?**
> 
> _Select all correct answers. Selecting wrong answers gives a point deduction._
> 
> _Text input required: Justify your answer(s) in the text box._
> 
> - a. One cannot assign an exact momentum to a bound state.
>     
> - b. The expectation value of momentum in the ground state is always determined by the virial theorem $\langle \hat{T} \rangle = -\frac{1}{2} \langle \hat{V} \rangle$.
>     
> - c. For an arbitrary state of the infinitely high potential well, the momentum $p$ is constant at all $x$.
>     
> - d. In the hydrogen atom, the virial theorem $\langle \hat{T} \rangle = -\frac{1}{2} \langle \hat{V} \rangle$ holds for arbitrary states.
>     

Let's dissect these one by one!

---

### Statement (a): Exact momentum of a bound state

**Yes. (This statement is CORRECT).**

- **The Physics:** This is a direct consequence of **Heisenberg's Uncertainty Principle** ($\Delta x \Delta p \ge \hbar/2$). By definition, a bound state means the particle is confined to a specific, finite region of space (e.g., trapped in a well or bound to a nucleus). Because it is spatially confined, its position uncertainty $\Delta x$ is finite.
    
- If a state had an _exact_ momentum, its momentum uncertainty $\Delta p$ would be zero. According to Heisenberg, this would require $\Delta x$ to be infinite! Mathematically, a state with exact momentum is a plane wave ($\psi(x) \propto e^{ikx}$), which stretches evenly across the entire universe from $-\infty$ to $+\infty$. Such a state is fundamentally unbound. Therefore, a confined, bound state can never have an exact momentum.
    

### Statement (b): Momentum expectation and the Virial Theorem

**No. (This statement is FALSE).**

- **The Physics:** There are two major flaws in this statement. First, the virial theorem relates the expectation value of kinetic **energy** ($\langle \hat{T} \rangle$), not momentum. The expectation value of momentum $\langle \hat{p} \rangle$ for any stationary bound state is actually always zero (the particle isn't traveling away anywhere!).
    
- Second, the specific formula $\langle \hat{T} \rangle = -\frac{1}{2} \langle \hat{V} \rangle$ is not "always" true. That specific fraction only appears for potentials that are proportional to $1/r$ (like the Coulomb potential). If you were looking at a quantum harmonic oscillator, for example, the virial theorem states that $\langle \hat{T} \rangle = \langle \hat{V} \rangle$.
    

### Statement (c): Constant momentum in an infinite well

**No. (This statement is FALSE).**

- **The Physics:** When a particle is trapped in an infinitely high potential well, the allowed wavefunctions are standing waves (like the sine waves on a plucked guitar string).
    
- A standing wave does not move in one direction; mathematically, Euler's formula tells us that a standing wave like $\sin(kx)$ is actually a superposition (a sum) of a wave moving to the right ($+p$) and a wave moving to the left ($-p$). Therefore, the particle does not have a single, constant momentum. Furthermore, stating that momentum has a specific value "at all $x$" implies a classical trajectory, which violates the probabilistic nature of quantum mechanics.
    

### Statement (d): Virial Theorem for arbitrary states

**No. (This statement is FALSE).**

- **The Physics:** The key word here is "arbitrary" (beliebige). The generalized virial theorem in quantum mechanics dictates how the expectation values change over time. It states that $2\langle \hat{T} \rangle - \langle \vec{r} \cdot \nabla\hat{V} \rangle = \frac{d}{dt}\langle \vec{r} \cdot \hat{p} \rangle$.
    
- For **stationary states** (energy eigenstates), the properties of the system do not change over time, so the right side is zero, leaving us with the familiar $\langle \hat{T} \rangle = -\frac{1}{2} \langle \hat{V} \rangle$ for the hydrogen atom. However, for an _arbitrary_ state (like a superposition of different energy levels), the state evolves and sloshes around over time. Because the time derivative is no longer zero, that simple relationship does not hold universally at every given instant.
    

---

### Summary for your Exam

You should only check box **a**.

For your text box justification, here is a clear and concise summary:

> _"a is correct because a bound state implies spatial confinement (finite $\Delta x$), meaning $\Delta p > 0$ via the Uncertainty Principle; thus momentum cannot be exactly known. b is false because the virial theorem determines the expectation value of kinetic energy, not momentum, and the specific relation $\langle \hat{T} \rangle = -1/2\langle \hat{V} \rangle$ only applies to $1/r$ potentials, not all ground states. c is false because states in an infinite well are standing waves, which are superpositions of $+p$ and $-p$, not a single constant momentum. d is false because the simple form of the virial theorem strictly applies to stationary states (eigenstates) where time derivatives of expectation values vanish, not to arbitrary, time-evolving superposition states."_

Would you like me to walk you through the math of how we use the commutator to prove that the time derivative of an expectation value is zero for stationary states?