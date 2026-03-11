

It is an absolute pleasure to help you consolidate this! You have tackled some of the most fundamental and historically significant mechanics in quantum theory today. While I always encourage my students to understand the derivations (which you now do!), having a quick reference sheet is a very smart strategy for exams.

Here is a summarized "cheat sheet" of the core concepts and formulas we derived and used across this problem set. I have included the reduced Planck constant ($\hbar$) in these formulas, as it is standard for exams, but remember you can set it to **1** if your specific exam uses natural units.

### 1. Fundamental Properties of Observables

- **Hermiticity:** Any operator representing a physical observable (like angular momentum components $\hat{L}_x$, $\hat{L}_y$, $\hat{L}_z$) is equal to its own adjoint: $\hat{A}^\dagger = \hat{A}$.
    
- **Positivity of Squared Operators:** For any Hermitian operator, the expectation value of its square is always non-negative: $\langle \hat{A}^2 \rangle \ge 0$.
    
- **Norm of a State:** The inner product of any state with itself represents a probability or length squared and is strictly non-negative: $\langle \psi | \psi \rangle \ge 0$.
    

---

### 2. Angular Momentum Algebra & Commutators

This is the algebraic engine of quantum rotations.

|**Concept**|**Formula**|**Description**|
|---|---|---|
|**Fundamental Commutator**|$[\hat{L}_j, \hat{L}_k] = i\hbar\epsilon_{jkl}\hat{L}_l$|Defines the algebra. $\epsilon_{jkl}$ is the Levi-Civita symbol.|
|**Specific Commutators**|$[\hat{L}_x, \hat{L}_y] = i\hbar\hat{L}_z$|Cyclic permutations yield a positive $i\hbar$ times the third component.|
|**Ladder Operators**|$\hat{L}_\pm = \hat{L}_x \pm i\hat{L}_y$|Complex operators used to step $m$ states up or down.|
|**Ladder Commutator**|$[\hat{L}_z, \hat{L}_\pm] = \pm \hbar\hat{L}_\pm$|Proves that $\hat{L}_\pm$ changes the $z$-component of angular momentum by $\pm \hbar$.|

---

### 3. Addition of Angular Momentum (2 Particles)

When dealing with two separate particles, we combine their individual angular momenta into a total angular momentum $\hat{J}$.

- **Total Operators:** * $\hat{J}_z = \hat{L}_{1z} + \hat{L}_{2z}$
    
    - $\hat{J}^2 = (\hat{\vec{L}}_1 + \hat{\vec{L}}_2)^2 = \hat{L}_1^2 + \hat{L}_2^2 + 2\hat{L}_{1z}\hat{L}_{2z} + \hat{L}_{1+}\hat{L}_{2-} + \hat{L}_{1-}\hat{L}_{2+}$
        
- **The Uncoupled Basis:** Written as $|l_1, m_1; l_2, m_2\rangle$. It is formed by the simple tensor product of the two individual particle states.
    
- **Eigenstate Rules:**
    
    - The uncoupled state **is** an eigenstate of $\hat{J}_z$ with eigenvalue $(m_1 + m_2)\hbar$.
        
    - The uncoupled state **is NOT** generally an eigenstate of $\hat{J}^2$ because the ladder operator cross-terms ($\hat{L}_{1+}\hat{L}_{2-}$ and $\hat{L}_{1-}\hat{L}_{2+}$) mix states with different $m$ values.
        
- **Expectation Value of $\hat{J}^2$:**
    
    - $\langle \hat{J}^2 \rangle = \left[ l_1(l_1 + 1) + l_2(l_2 + 1) + 2m_1m_2 \right] \hbar^2$
        
    - _Exam Tip:_ This works because the expectation values of the ladder cross-terms are strictly zero due to the orthogonality of different eigenstates ($\langle l, m | l, m \pm 1 \rangle = 0$).
        

---

You have built a very solid theoretical foundation today. Since we briefly touched on the fact that uncoupled states are not eigenstates of $\hat{J}^2$, would you like to see a quick example of how we use Clebsch-Gordan coefficients to build the states that _are_ true eigenstates of the total angular momentum?