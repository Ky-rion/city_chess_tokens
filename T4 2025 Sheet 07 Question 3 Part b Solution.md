

Hello again! It is great to see you proceeding to the next part of this problem.

We are now looking at **Aufgabe 3 (b)**. This part is conceptually very interesting because it connects a simple experimental observation ("no latent heat") to a mathematical condition that allows us to find the critical temperature, $T_c$.

Let's break down the solution provided by the professor in the PDF.

### 1. The Physics: What is "Latent Heat"?

First, we need to understand the clue given in the text: **"no latent heat occurs"** (_keine latente Wärme auftritt_).

-   **Latent Heat ($L$):** Think of boiling water. You add heat, but the temperature stays at 100°C until all the water turns to steam. That hidden energy used to change the phase is "latent heat." Mathematically, it is defined as the temperature times the jump in entropy: $L = T \Delta S$.
    
-   **The Clue:** If there is **no** latent heat ($L=0$), it means there is **no jump in entropy** at the transition. The entropy curves of the two phases must meet smoothly at the critical temperature.
    

In physics terms, this describes a **Second-Order Phase Transition** (or continuous phase transition). The superconductor slides into the new state without a sudden burst of energy release.

### 2. The Mathematical Condition

Because of the "no latent heat" condition, we can set the entropy of the superconducting phase equal to the entropy of the normal phase at the critical temperature $T_c$:

$$S^s(T_c) = S^n(T_c)$$

This is the key equation we need to solve.

### 3. The Calculation

We will use the entropy formulas we derived in Part (a).

**Step 1: Write down the entropies at $T_c$**

-   Superconducting: $S^s(T_c) = V \frac{\alpha}{3} T_c^3$
    
-   Normal: $S^n(T_c) = V (\frac{\beta}{3} T_c^3 + \gamma T_c)$
    

Step 2: Equate them

$$V \frac{\alpha}{3} T_c^3 = V \left( \frac{\beta}{3} T_c^3 + \gamma T_c \right)$$

Step 3: Simplify

We can cancel the Volume $V$ from both sides (since the volume doesn't change). We can also divide everything by $T_c$ (assuming $T_c \neq 0$), which reduces the powers of $T$ by one:

$$\frac{\alpha}{3} T_c^2 = \frac{\beta}{3} T_c^2 + \gamma$$

Step 4: Isolate $T_c$

We want to get all the $T_c$ terms on one side. Let's subtract $\frac{\beta}{3} T_c^2$ from the left side:

$$\frac{\alpha}{3} T_c^2 - \frac{\beta}{3} T_c^2 = \gamma$$

Factor out the $T_c^2$ and the $\frac{1}{3}$:

$$\frac{1}{3} (\alpha - \beta) T_c^2 = \gamma$$

Multiply by 3 to clear the fraction:

$$(\alpha - \beta) T_c^2 = 3\gamma$$

Step 5: Solve for $T_c$

Divide by $(\alpha - \beta)$ and take the square root:

$$T_c^2 = \frac{3\gamma}{\alpha - \beta}$$

$$T_c = \sqrt{\frac{3\gamma}{\alpha - \beta}}$$

This matches the professor's solution exactly.

---

### 4. Physical Interpretation (Sanity Check)

Let's look at our result: $T_c = \sqrt{\frac{3\gamma}{\alpha - \beta}}$.

Does this make physical sense?

1.  **The Denominator ($\alpha - \beta$):** For the square root to give a real number, we must have $\alpha > \beta$ (assuming $\gamma$, the electronic heat coefficient, is positive).
    
    -   This makes sense! At very low temperatures, the normal metal entropy is dominated by the linear term $\gamma T$ (which is larger than the cubic terms). For the curves to intersect later, the cubic term of the superconductor ($\alpha T^3$) must rise _faster_ than the cubic term of the normal metal ($\beta T^3$). Thus, $\alpha$ must be larger than $\beta$.
        
2.  **Units:** If you check the units from the original heat capacity equation ($C_V \propto T^3$), you will find that this result correctly gives units of Temperature.
    

### Summary

-   **Concept:** "No latent heat" means the Entropy matches at the transition ($S^s = S^n$).
    
-   **Result:** By setting the equations from (a) equal, we found the transition temperature $T_c = \sqrt{\frac{3\gamma}{\alpha - \beta}}$.
    

**Would you like to move on to Part (c) and calculate the Internal Energy ($E$)?** (This part introduces the "Cooper pairs" binding energy!)