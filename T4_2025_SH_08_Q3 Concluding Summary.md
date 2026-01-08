

Of course! A cheat sheet is a brilliant idea. In statistical mechanics, having the core arguments condensed into a few lines is often the difference between a panic attack and a solved problem.

Here is a summary of the key concepts and formulas from the "Ice Entropy" problem, formatted so you can easily copy it onto your exam preparation sheet.

### **Cheat Sheet: Residual Entropy of Ice (Pauling's Model)**

**1. The Physical Model**

-   **Structure:** Water ice is a lattice where every Oxygen ($O$) is at the center of a tetrahedron.
    
-   **Coordination:** Each $O$ has **4** neighbors (connected by hydrogen bonds).
    
-   **The "Ice Rule":** To maintain the molecule as $H_2O$, every Oxygen must have exactly **2 protons close ("in")** and **2 protons far ("out")**.
    

**2. Single Tetrahedron Entropy (Micro)**

-   **Problem:** How many ways can we arrange 4 protons on a single $O$ atom to satisfy the Ice Rule?
    
-   Calculation: We need to choose 2 positions out of 4 to be the "in" positions.
    
    $$\Omega_{single} = \binom{4}{2} = \frac{4!}{2!(4-2)!} = 6$$
    
-   Entropy:
    
    $$S_{single} = k_B \ln(6)$$
    

**3. Crystal Entropy (Macro) - The Pauling Approximation**

-   **Problem:** What is the entropy of a crystal with $N$ molecules?
    
-   **Total Bonds:** A crystal with $N$ atoms has $2N$ bonds (since each bond is shared by 2 atoms).
    
-   Unconstrained States: If there were no rules, each of the $2N$ bonds has 2 states (+ or -).
    
    $$\Omega_{raw} = 2^{2N} = 4^N$$
    
-   Probability of Validity: The probability that any single vertex satisfies the rule is the valid states divided by total states for one vertex ($2^4 = 16$).
    
    $$P_{valid} = \frac{6}{16} = \frac{3}{8}$$
    
-   Total Microstates ($\Omega$): Assumes independence of probabilities.
    
    $$\Omega_{crystal} = \Omega_{raw} \times (P_{valid})^N = 4^N \times \left(\frac{3}{8}\right)^N = \left(\frac{3}{2}\right)^N$$
    

**4. The Final Result & Interpretation**

-   Residual Entropy Formula:
    
    $$S = k_B \ln \left[ \left(\frac{3}{2}\right)^N \right] = N k_B \ln(1.5)$$
    
    (Specific entropy per molecule: $s = k_B \ln(1.5)$)
    
-   **Third Law Exception:**
    
    -   **Third Law:** usually states $S \to 0$ as $T \to 0$.
        
    -   **Ice Exception:** $S_{T=0} \neq 0$.
        
    -   **Why?** The ground state is **degenerate**. There is no unique lowest-energy configuration; the protons are "frozen" in a random pattern.
        

**5. Useful Math Helper**

-   Stirling's Approximation: (Use if you need to calculate factorials for large $N$)
    
    $$\ln N! \approx N \ln N - N$$
    

---

**Would you like me to create a quick practice quiz for you to test if you've really memorized these steps?**