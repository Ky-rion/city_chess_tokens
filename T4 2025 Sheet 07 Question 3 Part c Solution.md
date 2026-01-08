

Hello again! It is a pleasure to continue our physics session.

We are now tackling **Aufgabe 3 (c)**. This part is exciting because it introduces the quantum mechanical heart of superconductivity: the **Cooper pairs**.

In this step, we move from Entropy ($S$) to **Internal Energy ($E$)**. We are given the "starting energy" at absolute zero and asked to find how the energy grows as the metal heats up.

Let's break down the solution provided in the PDF.

### 1. The Physics: Ground States and Excitations

The problem statement gives us two vital pieces of information about the energy at absolute zero ($T=0$):

1.  **Normal Phase:** $E^n(0) = E_0$. This is the baseline energy of the metal electrons.
    
2.  **Superconducting Phase:** $E^s(0) = E_0 - V \cdot \Delta$.
    
    -   **The Physics:** This lower energy tells us that the superconducting state is the "preferred" state at $T=0$. The electrons have formed **Cooper pairs** (weakly bound pairs), lowering the total system energy by an amount $V \cdot \Delta$. This "binding energy" is what keeps the material superconducting.
        

**Our Goal:** Calculate $E(T)$ for both phases at finite temperatures $T > 0$.

### 2. The Theoretical Toolkit

To calculate the internal energy at a higher temperature, we simply sum up all the heat energy we added to the system to get there.

From the definition of heat capacity at constant volume:

$$C_V = \left(\frac{\partial E}{\partial T}\right)_V$$

We can invert this to find the energy by integrating:

$$E(T) = E(T=0) + \int_{0}^{T} C_V(T') dT'$$

### 3. The Calculation

We will apply this integral to both phases using the heat capacities given in the very first part of the problem.

**Part 1: The Superconducting Phase ($E^s$)**

-   **Start Energy:** $E^s(0) = E_0 - V\Delta$
    
-   **Heat Capacity:** $C_V^s(T) = V\alpha T^3$
    

Now, we integrate:

$$E^s(T) = (E_0 - V\Delta) + \int_{0}^{T} V\alpha (T')^3 dT'$$

Using the power rule for integration ($\int x^3 dx = \frac{x^4}{4}$):

$$\int_{0}^{T} V\alpha (T')^3 dT' = V\alpha \left[ \frac{(T')^4}{4} \right]_0^T = \frac{\alpha}{4} V T^4$$

Result:

$$E^s(T) = E_0 - V\Delta + \frac{\alpha}{4} V T^4$$

**Part 2: The Normal Phase ($E^n$)**

-   **Start Energy:** $E^n(0) = E_0$
    
-   **Heat Capacity:** $C_V^n(T) = V(\beta T^3 + \gamma T)$
    

Now, we integrate:

$$E^n(T) = E_0 + \int_{0}^{T} V(\beta (T')^3 + \gamma T') dT'$$

We integrate term by term:

1.  $\int \beta (T')^3 dT' = \frac{\beta}{4} T^4$
    
2.  $\int \gamma T' dT' = \frac{\gamma}{2} T^2$
    

Result:

$$E^n(T) = E_0 + V \left( \frac{\beta}{4} T^4 + \frac{\gamma}{2} T^2 \right)$$

### Summary

We have now constructed the full Internal Energy picture:

-   Superconductor: Starts lower (stable ground state) but gains energy purely through a $T^4$ term.
    
    $$E^s(T) = E_0 - V\Delta + \frac{\alpha}{4} V T^4$$
    
-   Normal Metal: Starts higher but gains energy through both a $T^4$ term and a $T^2$ term (from the conduction electrons).
    
    $$E^n(T) = E_0 + V \left( \frac{\beta}{4} T^4 + \frac{\gamma}{2} T^2 \right)$$
    

This is a crucial setup for the next part. Thermodynamics dictates that nature minimizes **Free Energy** ($F = E - TS$), not just Internal Energy ($E$). In part (d), we will combine your results from (a) and (c) to see which phase "wins" at different temperatures.

**Would you like to move on to part (d) to calculate the Free Energy and find the transition temperature in terms of $\Delta$?**