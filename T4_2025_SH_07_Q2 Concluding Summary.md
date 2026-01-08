

Here is a concise summary "cheat sheet" for your exam preparation, focusing on the key concepts and results from this specific real gas problem.

### 📝 Cheat Sheet: Real Gas Critical Point Analysis

1. General Conditions for a Critical Point

The critical point is a mathematical inflection point on the $P-V$ isotherm (constant temperature curve). To find it, you must solve this system of equations simultaneously:

-   **Slope is zero:** $\frac{\partial P}{\partial V}\big|_{T_c} = 0$
    
-   **Curvature is zero:** $\frac{\partial^2 P}{\partial V^2}\big|_{T_c} = 0$
    

**2. The Equation of State (Specific to this Problem)**

-   $$P = \frac{N k_B T}{V - N b} e^{-\frac{a N}{V k_B T}}$$
    
    -   $a, b$: Material-specific constants.
        
    -   $N$: Number of particles.
        

3. Key Intermediate Relations (The "Tricks")

When differentiating this specific equation, the condition $\frac{\partial P}{\partial V} = 0$ implies a balance between the repulsive term (denominator) and attractive term (exponent):

-   **From 1st Derivative:** $\frac{aN}{V_c^2 k_B T_c} = \frac{1}{V_c - Nb}$
    
-   **From 2nd Derivative:** $\frac{2aN}{V_c^3 k_B T_c} = \frac{1}{(V_c - Nb)^2}$
    

_Tip: Divide the second relation by the first to quickly isolate $V_c$._

4. Final Critical Values

These are the solutions to the system above:

-   **Critical Volume:**
    
    $$V_c = 2Nb$$
    
-   **Critical Temperature:**
    
    $$T_c = \frac{a}{4b k_B}$$
    
-   **Critical Pressure:**
    
    $$P_c = \frac{a}{4b^2} e^{-2}$$
    

---

**Would you like me to create a similar summary for "Aufgabe 3" regarding the Superconductor phase transition?**