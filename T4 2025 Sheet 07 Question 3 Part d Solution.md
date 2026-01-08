

Hello! It is great to see you again. We are making excellent progress through this thermodynamics problem.

We are now on **Aufgabe 3 (d)**. This is the pivotal moment where we combine everything we have calculated so far—Entropy ($S$) from part (a) and Internal Energy ($E$) from part (c)—to determine the **Helmholtz Free Energy ($F$)**.

Thermodynamics tells us that systems at constant temperature and volume do not just minimize their internal energy; they minimize their _Free Energy_. This balance between "wanting low energy" and "wanting high entropy" determines the phase transition.

Let's walk through the solution step-by-step.

### 1. The Theoretical Toolkit

Definition: The Helmholtz Free Energy is defined as:

$$F = E - TS$$

The Condition: The phase transition occurs when the Free Energies of the two phases are equal. Below $T_c$, the superconductor has lower free energy; above $T_c$, the normal metal does.

$$F^s(T_c) = F^n(T_c)$$

### 2. The Calculation

We need to calculate $F$ for both phases using your previous results.

Step 1: Free Energy of the Superconductor ($F^s$)

From previous parts, we have:

-   $E^s(T) = E_0 - V\Delta + \frac{\alpha}{4} V T^4$
    
-   $S^s(T) = \frac{\alpha}{3} V T^3$
    

Now, construct $F^s = E^s - T S^s$:

$$F^s(T) = \left( E_0 - V\Delta + \frac{\alpha}{4} V T^4 \right) - T \left( \frac{\alpha}{3} V T^3 \right)$$

Combine the $T^4$ terms ($\frac{1}{4} - \frac{1}{3} = -\frac{1}{12}$):

$$F^s(T) = E_0 - V\Delta - \frac{\alpha}{12} V T^4$$

Step 2: Free Energy of the Normal Metal ($F^n$)

From previous parts, we have:

-   $E^n(T) = E_0 + V(\frac{\beta}{4} T^4 + \frac{\gamma}{2} T^2)$
    
-   $S^n(T) = V(\frac{\beta}{3} T^3 + \gamma T)$
    

Construct $F^n = E^n - T S^n$:

$$F^n(T) = \left( E_0 + V\left(\frac{\beta}{4} T^4 + \frac{\gamma}{2} T^2\right) \right) - T \left( V\left(\frac{\beta}{3} T^3 + \gamma T\right) \right)$$

Group the terms by power of $T$:

-   $T^4$ terms: $\frac{\beta}{4} - \frac{\beta}{3} = -\frac{\beta}{12}$
    
-   $T^2$ terms: $\frac{\gamma}{2} - \gamma = -\frac{\gamma}{2}$
    

$$F^n(T) = E_0 - V\left( \frac{\beta}{12} T^4 + \frac{\gamma}{2} T^2 \right)$$

Step 3: Equate Free Energies to find $T_c$

At the critical temperature $T_c$, $F^s = F^n$.

$$E_0 - V\Delta - \frac{\alpha}{12} V T_c^4 = E_0 - \frac{\beta}{12} V T_c^4 - \frac{\gamma}{2} V T_c^2$$

Cancel $E_0$ and $V$ from both sides:

$$-\Delta - \frac{\alpha}{12} T_c^4 = - \frac{\beta}{12} T_c^4 - \frac{\gamma}{2} T_c^2$$

Rearrange to isolate $\Delta$:

$$\Delta = - \frac{\alpha}{12} T_c^4 + \frac{\beta}{12} T_c^4 + \frac{\gamma}{2} T_c^2$$

$$\Delta = - \frac{(\alpha - \beta)}{12} T_c^4 + \frac{\gamma}{2} T_c^2$$

Step 4: Substitution

The question asks for $T_c$ in terms of $\Delta$ and $\gamma$. We need to eliminate $\alpha$ and $\beta$.

Recall our result from part (b):

$$(\alpha - \beta) T_c^2 = 3\gamma$$

Substitute this expression into the first term of our $\Delta$ equation:

$$\text{Term 1: } - \frac{(\alpha - \beta) T_c^2}{12} \cdot T_c^2 \rightarrow - \frac{3\gamma}{12} T_c^2 = - \frac{\gamma}{4} T_c^2$$

Now the equation for $\Delta$ becomes purely in terms of $\gamma$ and $T_c$:

$$\Delta = - \frac{\gamma}{4} T_c^2 + \frac{\gamma}{2} T_c^2$$

Combine the fractions ($-\frac{1}{4} + \frac{1}{2} = \frac{1}{4}$):

$$\Delta = \frac{\gamma}{4} T_c^2$$

Step 5: Solve for $T_c$

$$T_c^2 = \frac{4\Delta}{\gamma}$$

$$T_c = \sqrt{\frac{4\Delta}{\gamma}} = 2\sqrt{\frac{\Delta}{\gamma}}$$

### 3. Physical Interpretation

This is a beautiful result! Let's interpret the variables:

-   $\Delta$ represents the **energy gain from forming Cooper pairs** (essentially how "glue-like" the superconducting state is).
    
-   $\gamma$ represents the **density of normal electrons** (electronic heat capacity coefficient).
    

The equation $T_c \propto \sqrt{\Delta}$ tells us that the stronger the Cooper pair binding energy ($\Delta$), the higher the temperature needed to break them apart and destroy superconductivity.

**Would you like to move on to the final part (e), where we introduce Magnetic Fields ($B$) and calculate the Critical Field?**