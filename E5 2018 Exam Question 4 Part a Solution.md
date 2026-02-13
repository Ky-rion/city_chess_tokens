

Excellent! We are moving from the "experimental detective work" to the theoretical bedrock of nuclear physics. This problem set deals with how we model the nucleus itself—is it a drop of liquid? Is it a gas of particles? Is it a set of shells like an atom?

The answer, surprisingly, is "all of the above," depending on which property you are looking at! Let's break down **Aufgabe 4**.

---

### (a) The Weizsäcker Mass Formula (Liquid Drop Model)

This formula (also known as the Semi-Empirical Mass Formula or SEMF) is one of the most successful phenomenological models in physics. It treats the nucleus like a drop of incompressible liquid.

The question asks for the **Mass** of the nucleus, not just the binding energy. So, we start with the sum of the parts (protons and neutrons) and subtract the "glue" (binding energy) that holds them together (because $E=mc^2$, binding energy removes mass).

$$M(Z, A) = Z \cdot m_p + (A - Z) \cdot m_n - \frac{B(Z, A)}{c^2}$$

Where $B(Z, A)$ is the Binding Energy, composed of five distinct terms:

$$B(Z, A) = a_v A - a_s A^{2/3} - a_c \frac{Z(Z-1)}{A^{1/3}} - a_a \frac{(A - 2Z)^2}{A} + \delta(A, Z)$$

**The Terms Explained:**

1. **Volume Term ($a_v A$):**
    
    - **Concept:** The "Strong Force" is short-range. Each nucleon only interacts with its nearest neighbors. Therefore, the binding energy is simply proportional to the total number of nucleons (Volume).
        
2. **Surface Term ($-a_s A^{2/3}$):**
    
    - **Concept:** Nucleons on the surface have fewer neighbors than those deep inside. We must subtract their missing binding energy. Since surface area scales with $r^2$ and radius scales with $A^{1/3}$, the area scales with $A^{2/3}$.
        
3. **Coulomb Term ($-a_c \frac{Z(Z-1)}{A^{1/3}}$):**
    
    - **Concept:** Protons repel each other via the electromagnetic force. This creates instability (lowers binding energy). It scales with charge squared ($Z^2$) and inversely with radius ($1/A^{1/3}$).
        
4. **Asymmetry Term ($-a_a \frac{(A - 2Z)^2}{A}$):**
    
    - **Concept:** This is a quantum effect (Pauli Exclusion Principle). The nucleus prefers to have equal numbers of protons and neutrons ($N=Z$). Any deviation reduces stability.
        
5. **Pairing Term ($\delta$):**
    
    - **Concept:** Nucleons like to pair up with opposite spins.
        
        - **Even-Even** nuclei (e.g., $^{40}\text{Ca}$) are most stable ($+\delta$).
            
        - **Odd-Odd** nuclei are least stable ($-\delta$).
            
        - **Odd-Mass** nuclei are neutral ($0$).
            

---

### (b) The Asymmetry Term and the Fermi Gas Model

**Which model explains it?**

The Asymmetry term cannot be explained by the "Liquid Drop" analogy (liquids don't care if you mix two different fluids). It is explained by the **Fermi Gas Model**.

**The Explanation:**

Imagine the nucleus as two separate "buckets" (potential wells)—one for protons and one for neutrons.

- Protons and neutrons are **Fermions**, meaning they obey the Pauli Exclusion Principle. They cannot stack on top of each other; they must fill up energy levels one by one, like a ladder.
    
- To minimize the total energy of the system, you want to fill the lowest rungs of both ladders equally.
    

**The Sketch (Description):**

Imagine we have 10 particles.

- **Scenario A (Symmetric):** 5 Neutrons, 5 Protons. Both "ladders" are filled to level 5. This is the lowest energy state.
    
- **Scenario B (Asymmetric):** 8 Neutrons, 2 Protons. The Proton ladder is low (level 2), but the Neutron ladder is stacked very high (level 8). The particles at the top of the neutron stack have much higher energy than they would if they were protons in the empty slots of the other ladder.
    

**Why $Z \le N$?**

The Fermi Gas model (Asymmetry term) drives the nucleus toward $N=Z$ (symmetry).

However, the **Coulomb Force** (protons repelling protons) acts _against_ adding more protons.

- For light nuclei, the Coulomb force is weak, so symmetry wins ($N \approx Z$, like Oxygen-16).
    
- For heavy nuclei, the Coulomb repulsion is huge. To keep the nucleus stable, we need extra neutrons to add "strong force glue" without adding extra "Coulomb repulsion." Thus, stable heavy nuclei always have $N > Z$ (like Lead-208).
    

---

### (c) Magic Numbers and the Shell Model

**Origin of Magic Numbers:**

Just as atoms have "noble gases" when electron shells are full ($2, 10, 18...$), nuclei have "Magic Numbers" of protons or neutrons ($2, 8, 20, 28, 50, 82, 126$) that result in exceptionally stable nuclei.

This arises from the discrete energy levels of nucleons inside the nucleus. When a "shell" of energy levels is completely filled, there is a large energy gap to the next level, creating high stability.

**The Potential Used:**

Simple potentials (like a square well or harmonic oscillator) can predict the first few magic numbers (2, 8, 20), but they **fail** for the higher ones.

To explain the higher magic numbers (28, 50, etc.), Mayer and Jensen introduced the **Spin-Orbit Coupling Potential** ($V_{ls}$).

- This term accounts for the interaction between the nucleon's orbital angular momentum ($L$) and its intrinsic spin ($S$).
    
- It splits the energy levels significantly, pushing some levels down into lower groups, which reproduces the exact magic numbers observed in nature.
    

So, the full potential is roughly:

$$V(r) = V_{\text{Woods-Saxon}}(r) + V_{ls}(r) (\vec{L} \cdot \vec{S})$$

> **Professor's Summary:**
> 
> - **Liquid Drop:** Explains bulk mass and fission.
>     
> - **Fermi Gas:** Explains why $N \approx Z$.
>     
> - **Shell Model (with Spin-Orbit):** Explains magic numbers and specific quantum states.
>     

I hope this helps you visualize what is happening inside the nucleus! Do you have any other questions about these models?