

Here is a concise "Cheat Sheet" summary of the entire derivation. This is perfect for quick review before an exam.

### **Cheat Sheet: Derivation of Fermi-Dirac Statistics**

#### **1. Thermodynamic Foundation (Equilibrium)**

-   **Concept:** Systems in equilibrium minimize Free Energy ($F$) while keeping total particles ($N$) constant.
    
-   **Key Formula:**
    
    $$\mu = \frac{\partial F}{\partial N_i} \quad \text{where} \quad F = E - TS$$
    
-   **Physical Meaning:** The chemical potential $\mu$ acts as the "Lagrange multiplier" that constrains the particle number. It represents the energy cost to add one particle to the system.
    

---

#### **2. Counting Microstates (Combinatorics)**

-   **Concept:** Fermions obey the **Pauli Exclusion Principle** (only 1 particle per state) and are **indistinguishable**.
    
-   **Analogy:** Seating $N_i$ people in $D_i$ cinema seats.
    
-   **Key Formula (Binomial Coefficient):**
    
    $$\Omega_i = \binom{D_i}{N_i} = \frac{D_i!}{N_i! (D_i - N_i)!}$$
    
    -   $D_i$: Number of available states (degeneracy).
        
    -   $N_i$: Number of fermions.
        

---

#### **3. Entropy & Stirling's Approximation**

-   **Boltzmann Entropy:** $S = k_B \ln(\Omega)$.
    
-   **Stirling’s Approximation:** Used to handle factorials for large $N$.
    
    $$\ln(N!) \approx N \ln(N) - N$$
    
-   **Derivative of Entropy:** The change in entropy when adding a particle is:
    
    $$\frac{\partial S}{\partial N_i} = k_B \ln\left(\frac{D_i}{N_i} - 1\right)$$
    

---

#### **4. The Final Fermi-Dirac Distribution**

-   **Setup:** Combine the equilibrium condition (1) with the entropy derivative (3).
    
    $$\mu = E_i - T \underbrace{k_B \ln\left(\frac{D_i}{N_i} - 1\right)}_{\frac{\partial S}{\partial N_i}}$$
    
-   **Algebraic Step:** Rearrange to solve for the occupation probability $f_i = N_i/D_i$.
    
    $$\frac{D_i}{N_i} - 1 = e^{\frac{E_i - \mu}{k_B T}}$$
    
-   **Final Formula:**
    
    $$f(E) = \frac{1}{e^{\frac{E - \mu}{k_B T}} + 1}$$
    

#### **5. Quick Physical Interpretation**

-   **$T = 0$ K:** Step function. All states below $\mu$ are full ($f=1$), all above are empty ($f=0$).
    
-   **$T > 0$ K:** The step "smears" out. Electrons near $\mu$ can be thermally excited to higher energy levels.
    

Good luck with your exam preparation! Is there anything else about this topic you want to clarify?