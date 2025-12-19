

Welcome back to class! Excellent progress so far.

This second part of the problem is where we stop drawing pictures and start crunching the numbers. We need to calculate the energy "bill" for each trip from **A** to **B**.

The question asks for two things for each process:

1.  **Work ($W$):** Specifically, the work done **on** the gas ("am Gas").
    
2.  **Heat ($Q$):** The heat transferred **to** the gas.
    

To solve this efficiently, I will teach you a "pro-move" that simplifies the entire problem: calculating the **Internal Energy** first.

---

### Step 0: The "Pro-Move" (Calculating $\Delta U$)

In thermodynamics, the First Law is our golden rule:

$$\Delta U = Q + W$$

(Change in Internal Energy = Heat added + Work done on the gas)

Here is the secret: **$\Delta U$ (Internal Energy) is a state function.** It doesn't care _how_ you get from A to B (Process I, II, III, or IV). It only cares about the start and the finish. If we calculate $\Delta U$ once, we can use it for all four parts!

1. Determine the Gas Type:

The problem gives us the adiabatic relation: $P^3 V^5 = \text{const}$.

We can rewrite this as: $(P V^{5/3})^3 = \text{const}$, which simplifies to the standard form $P V^{\gamma} = \text{const}$ with $\gamma = 5/3$.

For an ideal gas, $\gamma = \frac{f+2}{f}$. Solving $5/3 = \frac{f+2}{f}$ gives us $f=3$.

This tells us we are dealing with a monatomic ideal gas (like Helium or Argon).

2. The Energy Formula:

For a monatomic ideal gas, the internal energy is:

$$U = \frac{3}{2} P V$$

**3. Calculate $\Delta U$:**

-   At Point A: $P_1 = 10^5 \text{ Pa}$, $V_1 = 10^{-3} \text{ m}^3$
    
    $$U_A = \frac{3}{2} (10^5)(10^{-3}) = \frac{3}{2} (100) = 150 \text{ Joules}$$
    
-   At Point B: $P_2 = \frac{10^5}{32} \text{ Pa}$, $V_2 = 8 \times 10^{-3} \text{ m}^3$
    
    $$U_B = \frac{3}{2} \left( \frac{10^5}{32} \right) (8 \times 10^{-3}) = \frac{3}{2} (25) = 37.5 \text{ Joules}$$
    
-   The Change ($\Delta U$):
    
    $$\Delta U = U_B - U_A = 37.5 - 150 = \mathbf{-112.5 \text{ J}}$$
    
    This value is fixed for all four processes!
    

---

### Solving the Processes

**Important Sign Convention:**

-   **Expansion:** The volume increases ($1 \to 8$ units). The gas pushes out, so it does work. This means work done **on** the gas ($W$) is **negative**.
    
-   **Work Formula:** $W = - \text{Area under the P-V curve}$.
    

#### **(I) Path A $\xrightarrow{\text{isobar}}$ D $\xrightarrow{\text{isochor}}$ B**

1.  **Work ($W_I$):**
    
    -   A $\to$ D: Constant pressure ($P_1 = 10^5$ Pa). The volume changes by $\Delta V = V_2 - V_1 = 7 \times 10^{-3} \text{ m}^3$.
        
        $$W_{A \to D} = -P \Delta V = -(10^5)(7 \times 10^{-3}) = -700 \text{ J}$$
        
    -   **D $\to$ B:** Constant volume. No movement means zero work.
        
    -   **Total $W_I$:** **$-700$ J**
        
2.  **Heat ($Q_I$):**
    
    -   Use the First Law: $Q = \Delta U - W$
        
    -   $Q_I = -112.5 - (-700) = -112.5 + 700 = \mathbf{587.5 \text{ J}}$
        

#### **(II) Path A $\xrightarrow{\text{isochor}}$ C $\xrightarrow{\text{isobar}}$ B**

1.  **Work ($W_{II}$):**
    
    -   **A $\to$ C:** Constant volume. Zero work.
        
    -   C $\to$ B: Constant pressure ($P_2 = \frac{10^5}{32} = 3125$ Pa). $\Delta V = 7 \times 10^{-3} \text{ m}^3$.
        
        $$W_{C \to B} = -P_2 \Delta V = -(3125)(7 \times 10^{-3}) = -21.875 \text{ J}$$
        
    -   **Total $W_{II}$:** **$-21.875$ J**
        
2.  **Heat ($Q_{II}$):**
    
    -   $Q_{II} = \Delta U - W_{II} = -112.5 - (-21.875) = -112.5 + 21.875 = \mathbf{-90.625 \text{ J}}$
        
        (Note: Negative Q means we removed heat from the gas).
        

#### **(III) Path A $\xrightarrow{\text{linear}}$ B**

1.  **Work ($W_{III}$):**
    
    -   The area under a straight line is a **Trapezoid**.
        
    -   Area $= \text{Width} \times \text{Average Height} = (V_2 - V_1) \times \frac{P_A + P_B}{2}$
        
    -   Average Pressure $= \frac{100,000 + 3,125}{2} = 51,562.5 \text{ Pa}$
        
    -   $W_{III} = -(7 \times 10^{-3}) (51,562.5) \approx \mathbf{-360.94 \text{ J}}$
        
2.  **Heat ($Q_{III}$):**
    
    -   $Q_{III} = \Delta U - W_{III} = -112.5 - (-360.94) = \mathbf{248.44 \text{ J}}$
        

#### **(IV) Path A $\xrightarrow{\text{adiabatisch}}$ B**

1.  **Heat ($Q_{IV}$):**
    
    -   By definition, adiabatic means **no heat transfer**.
        
    -   $Q_{IV} = \mathbf{0 \text{ J}}$
        
2.  **Work ($W_{IV}$):**
    
    -   Use the First Law: $\Delta U = Q + W$
        
    -   Since $Q=0$, the work must account for the entire energy change.
        
    -   $W_{IV} = \Delta U = \mathbf{-112.5 \text{ J}}$
        

---

### Summary Table

![[Pasted image 20251208183435.png]]

Professor's Comment:

Notice how different the heat and work values are, even though every process started at A and ended at B! This proves that Heat and Work are path functions (they depend on the journey), while Internal Energy is a state function (it only depends on the destination).

Ready to see what happens when we finally turn on that rotor and start stirring the gas? That's usually where things get chaotic (and entropy increases)! Would you like to proceed?