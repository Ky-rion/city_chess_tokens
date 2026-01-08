

Hello! It is a pleasure to welcome you to the world of statistical physics. Don't worry if this feels dense at first; what we are looking at here—the **Ehrenfest Equations**—is actually a beautiful way to describe how matter changes state when the transition is "subtle."

In your previous studies, you might have seen the **Clausius-Clapeyron equation**. That applies to what we call **First-Order Phase Transitions** (like ice melting into water). In those cases, there is a sudden jump in entropy (latent heat) and volume.

However, the problem you uploaded deals with **Second-Order Phase Transitions**. In these transitions, the material doesn't suddenly absorb heat or change size. Instead, its _properties_—like how "stiff" it is or how much it expands when heated—change abruptly. Because the "jumps" in volume and entropy are zero, the Clausius-Clapeyron equation gives us a mathematical error ($0/0$). We need a new tool. That tool is the Ehrenfest equations.

Let’s walk through the solution provided by your other professor, step-by-step.

---

### 1. The Setup: Gibbs Free Energy

To understand this derivation, we start with the **Gibbs Free Energy** ($G$), which depends on Temperature ($T$) and Pressure ($P$).

The professor's notes begin by defining what a "Second-Order Phase Transition" actually is:

-   **First derivatives of G** (Volume $V$ and Entropy $S$) are **continuous** (no jumps).
    
-   **Second derivatives of G** ($C_P$, $\alpha$, $\kappa_T$) have **discontinuities** (jumps).
    

The notes list these crucial "Response Coefficients" (second derivatives) on Page 7:

-   Isothermal Compressibility ($\kappa_T$): How much the volume shrinks under pressure.
    
    $$\kappa_T = - \frac{1}{V} \left( \frac{\partial^2 G}{\partial P^2} \right)_T$$
    
-   Thermal Expansion ($\alpha$): How much the volume grows with heat.
    
    $$\alpha = \frac{1}{V} \frac{\partial}{\partial T} \left( \frac{\partial G}{\partial P} \right)_T = \frac{1}{V} \left( \frac{\partial V}{\partial T} \right)_P$$
    
-   Specific Heat Capacity ($C_P$): How much energy it takes to raise the temperature.
    
    $$C_P = -T \left( \frac{\partial^2 G}{\partial T^2} \right)_P$$
    

---

### 2. Deriving the First Equation (Entropy)

We want to find a relationship for the jump in Heat Capacity, $\Delta C_P$.

Step A: Continuity of Entropy

Since this is a second-order transition, Entropy ($S$) does not jump. This means that right on the coexistence line (the boundary between Phase 1 and Phase 2), the entropy of Phase 1 ($S_1$) equals the entropy of Phase 2 ($S_2$).

If we move a tiny step along this phase boundary, the change in entropy for both phases must stay equal:

$$dS_1 = dS_2$$

or

$$dS_1 - dS_2 = 0 \quad \Rightarrow \quad \Delta(dS) = 0$$

Step B: Expanding the Differential

We expand the total change in entropy ($dS$) in terms of $T$ and $P$:

$$dS = \left( \frac{\partial S}{\partial T} \right)_P dT + \left( \frac{\partial S}{\partial P} \right)_T dP$$

Using Maxwell relations and definitions (where $\frac{\partial S}{\partial T}|_P = \frac{C_P}{T}$ and $\frac{\partial S}{\partial P}|_T = -\frac{\partial V}{\partial T}|_P$), the professor rewrites this as:

$$dS = \frac{C_P}{T} dT - \left( \frac{\partial V}{\partial T} \right)_P dP$$

Step C: Equating the Phases

Now, we apply the condition $\Delta(dS) = 0$. This means the change for Phase 2 minus Phase 1 is zero:

$$\frac{\Delta C_P}{T} dT - \Delta \left( \frac{\partial V}{\partial T} \right)_P dP = 0$$

Rearranging this to solve for the slope of the phase boundary ($\frac{dP}{dT}$), we get the **First Ehrenfest Equation** (Eq 3 in your image):

$$\Delta C_P = T \frac{dP}{dT} \Delta \left( \frac{\partial V}{\partial T} \right)_P$$

---

### 3. Deriving the Second Equation (Volume)

Next, we look at the Volume ($V$).

Step A: Continuity of Volume

Just like entropy, in a second-order transition, the volume is the same for both phases at the transition point. So, $V_1 = V_2$.

As we move along the boundary, the change in volume must also be identical:

$$dV_1 = dV_2 \quad \Rightarrow \quad \Delta(dV) = 0$$

Step B: Expanding the Differential

We write the total differential for Volume:

$$dV = \left( \frac{\partial V}{\partial T} \right)_P dT + \left( \frac{\partial V}{\partial P} \right)_T dP$$

Step C: Equating the Phases

Since $\Delta(dV) = 0$, the difference between the phases is zero:

$$\Delta \left( \frac{\partial V}{\partial T} \right)_P dT + \Delta \left( \frac{\partial V}{\partial P} \right)_T dP = 0$$

Rearranging this gives us the **Second Ehrenfest Equation** (Eq 4 in your image):

$$\Delta \left( \frac{\partial V}{\partial T} \right)_P = - \frac{dP}{dT} \Delta \left( \frac{\partial V}{\partial P} \right)_T$$

---

### 4. Deriving the Third Equation ($\alpha$ and $\kappa_T$)

Finally, we want to express this in terms of the coefficients $\alpha$ (expansion) and $\kappa_T$ (compressibility).

The professor uses the definitions we wrote down in the Setup:

1.  $\left( \frac{\partial V}{\partial T} \right)_P = V \alpha$
    
2.  $\left( \frac{\partial V}{\partial P} \right)_T = -V \kappa_T$
    

Now, substitute these into the result we just found in Section 3:

$$\Delta (V \alpha) = - \frac{dP}{dT} \Delta (-V \kappa_T)$$

Since $V$ is continuous and the same for both phases at the boundary, we can factor it out and cancel it. We are left with:

$$\Delta \alpha = \frac{dP}{dT} \Delta \kappa_T$$

Solving for the slope $\frac{dP}{dT}$, we get the **Third Ehrenfest Equation** (Eq 5 in your image):

$$\frac{dP}{dT} = \frac{\Delta \alpha}{\Delta \kappa_T}$$

---

### Professor's Summary

So, what have we achieved?

We found that for a second-order phase transition, we cannot use the heat of transformation (Latent Heat) to define the transition curve because there isn't any!

Instead, we proved that the slope of the phase boundary line ($\frac{dP}{dT}$) is determined by the ratio of the "jumps" in the material properties:

1.  The jump in **Thermal Expansion** ($\Delta \alpha$)
    
2.  The jump in **Compressibility** ($\Delta \kappa_T$)
    

This is a powerful result because it links thermodynamic theory directly to quantities we can measure in the lab.

**A quick next step for you:** Try to verify the units in the final equation $\frac{dP}{dT} = \frac{\Delta \alpha}{\Delta \kappa_T}$. Checking if the units on the left match the units on the right is a great way to build intuition for these physical quantities! Would you like me to help you with that?