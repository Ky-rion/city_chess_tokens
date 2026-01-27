

Here is a condensed "Cheat Sheet" based on the exercises we just solved. These are the core tools you will need for any exam question involving electron statistics in semiconductors.

### 📚 Solid State Physics Cheat Sheet: Statistics & Bands

#### 1. Crucial Constants (at $T=300 \text{ K}$)

-   **Thermal Energy ($k_B T$):**
    
    $$k_B T \approx 0.0259 \text{ eV}$$
    
    _(Note: Sometimes rounded to 0.0258 eV or 26 meV. Check your professor's preference, but 0.0259 is standard for 300K)._
    
-   ** Boltzmann Constant ($k_B$):** $8.617 \times 10^{-5} \text{ eV/K}$
    

#### 2. The Golden Formulas

**A. The Fermi-Dirac Distribution ($f(E)$)**

This tells you the probability (0 to 1) that a specific energy state $E$ is occupied by an electron.

$$f(E) = \frac{1}{1 + e^{\frac{E - \mu}{k_B T}}}$$

-   $E$: The energy level you are investigating (e.g., Conduction Band edge).
    
-   $\mu$ (or $E_F$): The Fermi Energy (Chemical Potential).
    
-   **Tip:** If $(E - \mu) \gg k_B T$ (by more than ~3x), the "+1" doesn't matter, and it simplifies to the **Boltzmann Approximation**: $f(E) \approx e^{-\frac{E - \mu}{k_B T}}$.
    

**B. Intrinsic Fermi Level Position**

Unless told otherwise (doped semiconductors), for a pure (intrinsic) semiconductor, assume the Fermi level is exactly in the middle of the band gap.

$$E_F \approx \frac{E_C + E_V}{2}$$

-   If you set $E_V = 0$: $E_F = \frac{E_G}{2}$
    
-   $E_G$: Band Gap Energy ($E_C - E_V$).
    

#### 3. Standard Procedure for Solving

1.  **Define Zero:** Set the top of the Valence Band ($E_V$) to **0 eV**.
    
2.  **Find Boundaries:**
    
    -   $E_V = 0 \text{ eV}$
        
    -   $E_C = E_G$ (the Band Gap value)
        
3.  **Locate Fermi Level:** Calculate $E_F = E_G / 2$.
    
4.  **Identify Target Energy ($E$):**
    
    -   If asking for "bottom of conduction band", $E = E_G$.
        
    -   If asking for "thermal energy above gap", $E = E_G + k_B T$.
        
5.  **Plug & Chug:** Put values into the Fermi-Dirac equation. Watch your signs in the exponent!
    

#### 4. Conceptual "Sanity Checks"

-   **Semiconductor ($E_G \approx 1 \text{ eV}$):** You should get a small probability (like $10^{-10}$ to $10^{-12}$). This allows _some_ conduction.
    
-   **Insulator ($E_G > 4 \text{ eV}$):** You should get an essentially zero probability (like $10^{-70}$). No conduction possible.
    
-   **Conductor/Metal:** $E_F$ is inside a band. Probability is roughly 50% ($0.5$) near the Fermi level.
    

#### 5. Exam Trap to Watch Out For

**"eV" vs "Joules":**

-   In Solid State Physics, we almost always work in **electron-volts (eV)**.
    
-   Make sure your Boltzmann constant $k_B$ matches your energy units!
    
    -   Use $k_B = 8.617 \times 10^{-5} \text{ eV/K}$ (for eV).
        
    -   Do **NOT** use $1.38 \times 10^{-23} \text{ J/K}$ unless you convert everything to Joules first (which is painful).
        

Would you like me to create a quick practice problem using these formulas with a different material (like Silicon or Germanium) to test your cheat sheet?