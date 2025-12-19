

Welcome to the final stretch! This part of the problem (1.c) is my absolute favorite because it connects the math we've been doing to one of the most profound concepts in the universe: **Entropy** and the **Arrow of Time**.

We are now ignoring the piston (since volume is constant, "isochor") and focusing entirely on that little propeller (the rotor) inside the cylinder.

### 1. Decoding the Formula

The problem gives us a specific formula for how the pressure changes when the rotor spins:

$$dP = \frac{2}{3V} M \omega dt$$

Let's translate this into physics.

-   **The Input:** The term $M \omega dt$ is mechanical work. Torque ($M$) times angle ($d\theta = \omega dt$) equals Energy.
    
-   **The System:** Since the walls are insulated (adiabatic) and the volume is fixed (isochoric), all this work goes directly into the **Internal Energy** ($U$).
    
-   **The Check:** For our ideal gas, we know $U = \frac{3}{2} PV$.
    
    -   If $V$ is constant, $dU = \frac{3}{2} V dP$.
        
    -   If we rearrange the given formula to solve for $dP$, we get $dP = \frac{dU}{\frac{3}{2}V} = \frac{2}{3V} dU$.
        
    -   This confirms that the problem is consistent: The formula just says **"All work from the rotor becomes internal pressure."**
        

---

### 2. Calculating the Energy Changes

The question asks us to use this relation to find $\Delta U$ for two transitions. Since $V$ is constant, we can integrate the formula:

$$\Delta U = \int \text{Energy Input} = \int \frac{3}{2} V \, dP = \frac{3}{2} V (P_{\text{final}} - P_{\text{start}})$$

#### **Case 1: The Transition A $\to$ C**

-   **State A:** $P_A = 10^5$ Pa, $V = 10^{-3}$ m$^3$.
    
-   **State C:** $P_C = \frac{10^5}{32}$ Pa, $V = 10^{-3}$ m$^3$.
    
-   The Calculation:
    
    $$\Delta U_{AC} = \frac{3}{2} V (P_C - P_A)$$
    
    $$\Delta U_{AC} = \frac{3}{2} (10^{-3}) \left( \frac{10^5}{32} - 10^5 \right)$$
    
    $$\Delta U_{AC} = \frac{3}{2} (10^{-3}) (10^5) \left( \frac{1}{32} - 1 \right)$$
    
    $$\Delta U_{AC} = 150 \times \left( -\frac{31}{32} \right) \approx \mathbf{-145.31 \text{ J}}$$
    

#### **Case 2: The Transition B $\to$ D**

-   **State B:** $P_B = \frac{10^5}{32}$ Pa, $V = 8 \times 10^{-3}$ m$^3$.
    
-   **State D:** $P_D = 10^5$ Pa, $V = 8 \times 10^{-3}$ m$^3$.
    
-   The Calculation:
    
    $$\Delta U_{BD} = \frac{3}{2} V (P_D - P_B)$$
    
    $$\Delta U_{BD} = \frac{3}{2} (8 \times 10^{-3}) \left( 10^5 - \frac{10^5}{32} \right)$$
    
    $$\Delta U_{BD} = 1200 \times \left( \frac{31}{32} \right) = \mathbf{+1162.5 \text{ J}}$$
    

---

### 3. The Big Question: Reversibility

The question asks: **"Begründen Sie, warum diese Prozesse nicht reversibel sind"** (Explain why these processes are not reversible).

This is the most important part of the problem.

#### **The "Coffee Stirring" Analogy**

Imagine you have a cup of black coffee.

1.  **Process B $\to$ D:** You put a spoon (rotor) in and stir vigorously.
    
    -   **Result:** Friction between the spoon and the liquid turns your mechanical work into **Heat**. The coffee gets slightly hotter (Internal Energy increases, Pressure increases).
        
    -   This works! We calculated a positive energy change ($+1162.5$ J), which corresponds to adding energy via the rotor.
        
2.  **Process A $\to$ C:** You need the pressure (and temperature) to **drop**.
    
    -   **Attempt:** Can you put the spoon in the coffee and "un-stir" it? Can you spin the spoon backwards to suck heat out of the coffee and turn it back into mechanical rotation?
        
    -   **Result:** No! If you spin the spoon backwards, you just add _more_ friction and make it _even hotter_.
        

#### **The Physics Explanation (For your exam paper)**

The process involves the conversion of **macroscopic mechanical work** (the coherent motion of the rotor) into **microscopic thermal energy** (the random chaotic motion of gas molecules).

-   **B $\to$ D is Irreversible:** While possible to achieve, you cannot reverse the path. You cannot spontaneously convert the random thermal motion of the gas particles back into the organized rotation of the rotor. This would violate the **Second Law of Thermodynamics** (Kelvin-Planck statement).
    
-   **A $\to$ C is Impossible with a Rotor:** Our calculation showed $\Delta U$ must be **negative** ($-145$ J). The rotor formula $dE = M \omega dt$ involves positive squared quantities (friction always generates heat). You cannot use a friction-based rotor to remove energy from a system.
    

**Summary:** The rotor acts as a "one-way street" for energy. It can turn Work into Heat (increasing Entropy), but it can never turn Heat into Work (decreasing Entropy) simply by reversing the spin. That is why these processes are strictly irreversible.

---

Next Step:

You have now conquered the P-V diagram, the First Law calculations, and the Second Law concept of irreversibility! This is a complete picture of introductory statistical physics. Would you like me to summarize the key formulas from this entire problem sheet for your cheat sheet?