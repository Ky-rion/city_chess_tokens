

This is an excellent idea! Making a cheat sheet is one of the best ways to study because synthesizing the material forces your brain to organize the concepts logically.

As your professor, I am happy to help you condense our marathon problem-solving session into a high-yield study guide. I have organized this by conceptual themes so you can quickly find what you need during an exam.

---

### 1. Wavefunctions & 1D Potentials

- **Continuity Rules:** * The wavefunction $\psi(x)$ is **always** continuous.
    
    - The first derivative $\psi'(x)$ is continuous as long as $V(x)$ is finite (no infinite walls or delta functions).
        
    - The second derivative $\psi''(x)$ directly mirrors the continuity of $V(x)$ via the Schrödinger equation.
        
- **Bound States ($E < V_{\text{asymptotic}}$):** * Energy levels are discrete.
    
    - In 1D, bound states are strictly **non-degenerate**.
        
    - They are spatially confined (finite $\Delta x$), so by Heisenberg's Uncertainty Principle, they cannot have an exact momentum ($\Delta p > 0$).
        
- **Scattering States ($E > V_{\text{asymptotic}}$):** * Energy levels are continuous.
    
    - If a particle can only escape to one side (e.g., hitting a tall step), the state is non-degenerate. If it can escape to both $+\infty$ and $-\infty$, the state is **doubly degenerate**.
        

### 2. Operator Vocabulary

- **Hermitian ($O = O^\dagger$):** Represents physical observables (e.g., position, momentum, Hamiltonian). Eigenvalues are real.
    
- **Unitary ($U^\dagger U = U U^\dagger = I$):** Preserves probability (e.g., time evolution, spatial translation, symmetry transformations). Eigenvalues take the form $\lambda = e^{i\phi}$ (can be complex).
    
- **Normal ($O^\dagger O = O O^\dagger$):** Commutes with its adjoint. (Both Hermitian and Unitary operators are normal).
    
- **Projector ($P^2 = P$ and $P^\dagger = P$):** Projects a state onto a specific subspace.
    
- **Creation/Annihilation Operators:** $a^\dagger \neq a$. They are neither Hermitian nor Normal because they do not commute: $[a, a^\dagger] = 1$.
    

### 3. Time Evolution & Dynamics

- **Time Evolution Operator:** For a time-dependent Hamiltonian, use the time-ordered Dyson series:
    
    $$\hat{U}(t, t_0) = T\left[\exp\left(-i\int_{t_0}^t \hat{H}(\tau) d\tau\right)\right]$$
    
    _Note: An explicitly time-dependent $\hat{H}$ breaks time-translation symmetry._
    
- **Heisenberg Equation of Motion:** Dictates how expectation values change over time:
    
    $$\frac{d}{dt}\langle A\rangle = \frac{i}{\hbar}\langle[\hat{H}, \hat{A}]\rangle$$
    
- **2-Level Revival Time:** The time to return to an initial state depends inversely on the energy gap:
    
    $$T_{\text{rev}} = \frac{2\pi\hbar}{\Delta E}$$
    
- **Time-Energy Uncertainty:** $\Delta E \Delta t \ge \frac{\hbar}{2}$. Time is a parameter, not an operator. For a resonance, this relates the energy width $\Gamma$ to the lifetime $\tau$:
    
    $$\tau = \frac{\hbar}{\Gamma}$$
    
- **Virial Theorem (Stationary States):** Relates kinetic and potential energy expectation values: $2\langle \hat{T} \rangle = \langle \vec{r} \cdot \nabla\hat{V} \rangle$. For $1/r$ potentials (like the Hydrogen atom), this simplifies to $\langle \hat{T} \rangle = -\frac{1}{2}\langle \hat{V} \rangle$.
    

### 4. Angular Momentum & Spin

- **Spherical Harmonics ($Y_l^m$):** Eigenfunctions of angular momentum.
    
    $$\hat{L}^2 Y_l^m = l(l+1) Y_l^m \quad \text{and} \quad \hat{L}_z Y_l^m = m Y_l^m$$
    
    _Note: If a state has no azimuthal ($\phi$) dependence, $m = 0$._
    
- **Spin Addition:** When adding two spins ($s_1$ and $s_2$), total spin goes from $|s_1 - s_2|$ to $s_1 + s_2$. For two spin-1/2 particles, $s = 0$ (Singlet, antisymmetric) and $s = 1$ (Triplet, symmetric).
    
- **Commutators:** $[\hat{S}^2, \hat{S}_z] = 0$. This guarantees that states with different $s_z$ eigenvalues do not mix when applying $\hat{S}^2$.
    

### 5. Scattering & Perturbation Theory

- **Fermi's Golden Rule:** Calculates the transition rate (decay width $\Gamma$) from a discrete state to a continuum in lowest-order perturbation theory (with $\hbar = 1$):
    
    $$\Gamma = 2\pi |\langle f | V | i \rangle|^2 \rho(E)$$
    
- **First Born Approximation:** Calculates the scattering amplitude $f^{(1)}$ using a Fourier transform of the potential (with $m=1, \hbar=1$):
    
    $$f^{(1)}(\theta, \phi) = -\frac{1}{2\pi} \int d^3r e^{-i\vec{q}\cdot\vec{r}} V(\vec{r})$$
    
- **Momentum Transfer ($\vec{q}$):** $\vec{q} = \vec{p}_{\text{out}} - \vec{p}_{\text{in}}$. For elastic scattering ($|\vec{p}_{\text{in}}| = |\vec{p}_{\text{out}}| = p$), the magnitude squared is:
    
    $$q^2 = 2p^2(1 - \cos\theta)$$
    
- **Total Cross-Section:** The integral of the probability density over all solid angles:
    
    $$\sigma_{\text{tot}} = \int |f(\theta, \phi)|^2 d\Omega$$
    

### 6. Solid State & Wave Packets

- **Dispersion Relations:** When looking at an energy band $\hat{H}(p) = E(p)$:
    
    - **Effective Mass ($m^*$):** Defined by the inverse curvature of the energy band.
        
        $$m^* = \left( \frac{\partial^2 E}{\partial p^2} \right)^{-1}$$
        
    - **Group Velocity ($v_g$):** The speed at which the wave packet envelope moves.
        
        $$v_g = \frac{\partial E}{\partial p}$$
        

---

You have built a truly impressive foundation here. When you sit down for your exam, remember to trust your physics intuition first, and let the math follow.

Would you like me to generate a mock exam question combining a few of these concepts so you can test your new cheat sheet?