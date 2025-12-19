

Here is a focused cheat sheet summarizing the formulas, definitions, and theorems you would need to solve this problem in an exam setting.

### **1. Core Definitions & Given Conditions**

-   **The Critical Point ($T_c, P_c, V_c$):** The specific state where the liquid and gas phases become indistinguishable.
    
-   The First Derivative Condition (Given):
    
    At the critical point, the isotherm has a horizontal inflection point:
    
    $$\frac{\partial P}{\partial V}\bigg|_{T_c} = 0$$
    
    1
    

---

### **2. Thermodynamic Potentials**

You need to know how to relate Energy to Pressure.

-   Helmholtz Free Energy ($F$):
    
    $$F = U - TS$$
    
    Differential form (at constant $T$):
    
    $$dF = -P dV \quad \Rightarrow \quad P = - \left( \frac{\partial F}{\partial V} \right)_T$$
    
    2
    
-   Gibbs Free Energy ($G$):
    
    Used for stability analysis at constant $P$ and $T$.
    
    $$G = F + PV$$
    
    3
    

---

### **3. Method A: The Stability Argument (Taylor Expansion)**

This method uses the condition that energy must be at a minimum for stability.

-   Change in Gibbs Energy ($\delta G$):
    
    For a fluctuation $\delta V$ around the critical volume $V_c$:
    
    $$\delta G = F(T_c, V_c + \delta V) - F(T_c, V_c) + P_c \delta V$$
    
    4
    
-   Taylor Expansion of Free Energy ($F$):
    
    Expand $F$ up to the 4th order. Remember to swap $F$-derivatives for $P$-derivatives (since $\frac{\partial F}{\partial V} = -P$):
    
    $$F(V_c + \delta V) \approx F(V_c) - P_c \delta V - \frac{1}{2}\frac{\partial P}{\partial V}\delta V^2 - \frac{1}{6}\frac{\partial^2 P}{\partial V^2}\delta V^3$$
    
    555
    
-   **Simplification:**
    
    -   The linear terms cancel ($P_c \delta V - P_c \delta V = 0$).
        
    -   The quadratic term vanishes because $\frac{\partial P}{\partial V} = 0$.
        
    -   You are left with the lowest-order surviving term:
        
        $$\delta G \approx - \frac{1}{6} \frac{\partial^2 P}{\partial V^2}\bigg|_{T_c} \delta V^3$$
        
        6
        
-   The Stability Constraint:
    
    For the system to be stable, $\delta G$ must be positive (energy minimum).
    
    -   If the cubic term exists ($\delta V^3$), it will change sign depending on if $\delta V$ is positive or negative.
        
    -   To prevent instability ($\delta G < 0$), the coefficient must vanish:
        
        $$\frac{\partial^2 P}{\partial V^2}\bigg|_{T_c} = 0$$
        
        7
        

---

### **4. Method B: The Geometric Argument (Rolle's Theorem)**

This method uses the shape of the isotherms below the critical temperature.

-   Sub-critical Isotherms ($T < T_c$):
    
    The pressure curve has two extrema (a max and a min) where the slope is zero:
    
    $$\frac{\partial P}{\partial V} \bigg|_{V_{I1}} = 0 \quad \text{and} \quad \frac{\partial P}{\partial V} \bigg|_{V_{I2}} = 0$$
    
    8888
    
-   Rolle's Theorem (Mean Value Theorem):
    
    If a differentiable function ($f(x) = \frac{\partial P}{\partial V}$) is zero at two points ($x_1, x_2$), then its derivative ($f'(x) = \frac{\partial^2 P}{\partial V^2}$) must be zero somewhere between them.
    
    9999
    
-   The Limit:
    
    As $T \to T_c$, the two points $V_{I1}$ and $V_{I2}$ merge into the single critical volume $V_c$.
    
    $$V_{I1} \to V_c \leftarrow V_{I2}$$
    
    Therefore, the point where the second derivative is zero is "squeezed" to exactly $V_c$:
    
    $$\frac{\partial^2 P}{\partial V^2}\bigg|_{V_c} = 0$$
    
    10
    

---

### **5. Final Result**

At the critical point of a van der Waals-like gas:

1.  **Slope is zero:** $\frac{\partial P}{\partial V} = 0$
    
2.  **Curvature is zero:** $\frac{\partial^2 P}{\partial V^2} = 0$
    
3.  **Lowest non-zero derivative:** usually the third derivative $\frac{\partial^3 P}{\partial V^3} < 0$.