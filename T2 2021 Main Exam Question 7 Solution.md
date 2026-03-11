

Welcome back to my virtual office! You are doing incredibly well. This question steps into the beautiful and highly abstract territory of symmetries in quantum mechanics. Symmetries are the secret to solving the most complex problems in physics because they tell us what is conserved!

Let's start by translating the German text to ensure our definitions are perfectly aligned.

> **Given a Hamiltonian operator $\hat{H}$ and a unitary symmetry transformation $\hat{S}$. Which of the following statements are correct?**
> 
> _Select all correct answers. Selecting wrong answers gives a point deduction._
> 
> _Text input required: Justify your answer(s) in the text box._
> 
> - a. The eigenfunctions of $\hat{H}$ are invariant under $\hat{S}$.
>     
> - b. $\hat{S}$ can also have a non-real spectrum.
>     
> - c. $\hat{S}$ has either the spectrum $\sigma(\hat{S}) = \{0, 1\}$ or $\sigma(\hat{S}) = \{-1, 1\}$.
>     
> - d. In the case $\sigma(\hat{S}) = \{0, 1\}$, one constructs projectors onto the eigenstates as $\hat{H}_\pm = 1 \pm \hat{S}$.
>     
> - e. $\sigma(\hat{S}) = \{-1, 1\}$ can only occur in a 2-dimensional Hilbert space.
>     

### The Physics: What is a Unitary Symmetry Transformation?

Before looking at the options, we must define what the prompt tells us about $\hat{S}$.

1. **It is a symmetry:** This means $\hat{S}$ commutes with the Hamiltonian, $[\hat{H}, \hat{S}] = 0$. Because they commute, they can share a set of simultaneous eigenfunctions.
    
2. **It is unitary:** This means its adjoint is its inverse, $\hat{S}^\dagger \hat{S} = \hat{S}\hat{S}^\dagger = \hat{I}$. This is crucial because it dictates the possible eigenvalues (the spectrum) of $\hat{S}$. If $\hat{S}|\psi\rangle = \lambda|\psi\rangle$, then the unitarity condition requires that the magnitude of the eigenvalue is exactly 1 ($|\lambda|^2 = 1$). Therefore, any eigenvalue must have the form $\lambda = e^{i\phi}$ for some real number $\phi$.
    

Let's test the options with these two golden rules.

---

### Statement (a): Invariance of eigenfunctions

**No. (This statement is FALSE).**

- **The Physics:** While $\hat{H}$ and $\hat{S}$ share a set of eigenfunctions, applying $\hat{S}$ to an eigenfunction $|\psi\rangle$ does not necessarily leave it "invariant" (which would mean $\hat{S}|\psi\rangle = |\psi\rangle$). It scales the function by its eigenvalue: $\hat{S}|\psi\rangle = \lambda|\psi\rangle$.
    
- For example, consider the parity operator $\hat{P}$ (which flips space, $x \to -x$) in a symmetric potential. It is a unitary symmetry. If you apply it to an _odd_ eigenfunction, you get a minus sign: $\hat{P}|\psi_{\text{odd}}\rangle = -|\psi_{\text{odd}}\rangle$. The function is multiplied by $-1$, so it is not invariant! Furthermore, if $\hat{H}$ has degenerate energy levels, applying a symmetry operator might mix those degenerate states together into a new state.
    

### Statement (b): Non-real spectrum

**Yes. (This statement is CORRECT).**

- **The Physics:** As we proved above, the eigenvalues of a unitary operator are of the form $\lambda = e^{i\phi}$. Unless $\phi = 0$ or $\pi$ (which give $1$ and $-1$), the eigenvalue will be a complex number (e.g., if $\phi = \pi/2$, $\lambda = i$). Because complex numbers are "non-real," a unitary operator absolutely can have a non-real spectrum. A classic example is the spatial translation operator!
    

### Statement (c): Restricted spectrum $\{0, 1\}$ or $\{-1, 1\}$

**No. (This statement is FALSE).**

- **The Physics:** A unitary operator _cannot_ have $0$ in its spectrum. If an eigenvalue were $0$, then $|\lambda|^2 = 0$, violating the unitary requirement that $|\lambda|^2 = 1$. The spectrum $\{-1, 1\}$ is valid for _some_ unitary operators (specifically involutions, where applying it twice gets you back to where you started, like parity or spin-flips), but it is not a general rule for _all_ unitary symmetries.
    

### Statement (d): Projectors for spectrum $\{0, 1\}$

**No. (This statement is FALSE).**

- **The Physics:** First, as we just established, a unitary operator cannot have an eigenvalue of $0$, so the premise $\sigma(\hat{S}) = \{0, 1\}$ is impossible from the start. Second, the operators $\frac{1}{2}(1 \pm \hat{S})$ act as projectors only when $\hat{S}^2 = 1$ (which corresponds to a spectrum of $\{-1, 1\}$, not $\{0, 1\}$).
    

### Statement (e): Dimension restrictions on spectrum $\{-1, 1\}$

**No. (This statement is FALSE).**

- **The Physics:** The spectrum $\{-1, 1\}$ simply means the operator acts like a mirror or a flip ($\hat{S}^2 = 1$). This has nothing to do with the size of the Hilbert space. Think about a particle in an infinite 1D potential well (a box). The Hilbert space is infinite-dimensional (there are infinitely many energy levels). Yet, the parity operator $\hat{P}$ is a valid symmetry for this system, and its eigenvalues are strictly $+1$ (for even states) and $-1$ (for odd states).
    

---

### Summary for your Exam

You should only check box **b**.

For the required text box justification, here is a strong, mathematically rigorous summary:

> _"a is false because applying $\hat{S}$ to an eigenfunction multiplies it by an eigenvalue $\lambda$ (which could be $-1$ or $e^{i\phi}$), so the state is not necessarily invariant. b is correct because unitary operators have eigenvalues satisfying $|\lambda|^2 = 1$, meaning $\lambda = e^{i\phi}$, which generally yields non-real (complex) numbers. c and d are false because a unitary operator must be invertible, meaning $0$ can never be part of its spectrum. e is false because a symmetry with $\sigma(\hat{S}) = \{-1, 1\}$ (like the Parity operator) commonly exists in infinite-dimensional Hilbert spaces (e.g., the harmonic oscillator)."_

We just tackled some heavy abstract algebra concepts there. Would you like me to show you a concrete example of how we use the Parity operator ($\hat{P}$) to immediately simplify the calculation of expectation values without having to do complex integrals?