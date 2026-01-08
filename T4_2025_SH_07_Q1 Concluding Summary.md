

That is a fantastic idea! A well-organized "cheat sheet" (or formula summary) is one of the best ways to consolidate your understanding for an exam.

Here is a summary of the essential tools and results we used in Problem 1. I have organized it so you can quickly find the "Key Relation," the "Trick" to solve it, and the "Physical Meaning."

### 📝 Cheat Sheet: Thermodynamics near Absolute Zero

#### 1. Fundamental Relations (The Toolkit)

These are general identities you should memorize or know how to derive quickly.

-   Gibbs Free Energy Differential:
    
    $$dG = -SdT + VdP$$
    
    -   _Usage:_ Used to derive the Maxwell relation below.
        
-   The "Volume-Entropy" Maxwell Relation:
    
    $$\left(\frac{\partial V}{\partial T}\right)_P = -\left(\frac{\partial S}{\partial P}\right)_T$$
    
    -   _Usage:_ Connects measurable volume changes (expansion) to abstract entropy changes.
        
    -   _Note:_ $\beta = \frac{1}{V}\left(\frac{\partial V}{\partial T}\right)_P$, so the LHS is $V\beta$.
        
-   Heat Capacity & Entropy:
    
    $$C_P = T \left(\frac{\partial S}{\partial T}\right)_P \quad \Rightarrow \quad S(T) = \int_0^T \frac{C_P(T')}{T'} dT'$$
    
    -   _Usage:_ Allows you to calculate Entropy ($S$) if you are given the function for Heat Capacity ($C_P$).
        
    -   _Assumption:_ The Third Law implies $S(0) = 0$.
        

---

#### 2. The Adiabatic Cooling Formula

This is the specific derivation for "how temperature changes with pressure" in an insulated system.

-   Total Differential of Entropy:
    
    $$dS = -V\beta dP + \frac{C_P}{T} dT$$
    
    -   _Derivation:_ Plug the Maxwell relation and $C_P$ definition into $dS = (\partial_P S)dP + (\partial_T S)dT$.
        
-   The Adiabatic Slope (Isoentropic):
    
    Set $dS = 0$ (adiabatic) and rearrange:
    
    $$\left(\frac{\partial T}{\partial P}\right)_S = \frac{V\beta \cdot T}{C_P}$$
    
    -   _Meaning:_ This formula tells you how much "cooling power" you get by changing pressure.
        

---

#### 3. Key Limits at Absolute Zero ($T \to 0$)

These are the specific results from this problem that prove the Third Law.

-   Ratio of Expansion to Heat Capacity:
    
    $$\lim_{T \to 0} \frac{V\beta}{C_P} = \text{Finite Constant}$$
    
    -   _Why:_ Both $V\beta$ and $C_P$ scale with the same power of $T$ (e.g., $T^x$), so they cancel out.
        
-   Unattainability of Absolute Zero:
    
    $$\lim_{T \to 0} \left(\frac{\partial T}{\partial P}\right)_S = 0$$
    
    -   _Derivation:_ Since $\frac{V\beta}{C_P}$ is constant, the extra factor of $T$ in the numerator drives the whole expression to zero.
        
    -   _Physical Meaning:_ As you approach $0\text{ K}$, changing pressure no longer causes a temperature drop. Therefore, you need infinite steps to reach absolute zero.
        

---

Professor's Exam Tip:

If you see a problem asking about "cooling by adiabatic expansion" or "isentropic pressure change," start by writing down $dS(T, P)$ and setting it to zero. That is almost always the starting point!

Would you like to move on to **Problem 2**, where we apply these concepts to a Real Gas?