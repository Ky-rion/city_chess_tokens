

Hello! It is wonderful to see you again for the final part of this problem. You have done an excellent job navigating through entropy, internal energy, and free energy.

Now, we arrive at **Aufgabe 3 (e)**, which introduces the **Magnetic Field ($B$)**. This is where things get very real for superconductors. The interaction with magnetic fields is arguably the most famous property of superconductors (the **Meissner Effect**).

Let's break down the solution step-by-step.

### 1. The Physics: The Meissner Effect

The problem statement tells us a crucial fact: **"A superconductor is magnetic field free in the interior."**.

In a normal metal, magnetic field lines pass right through. But when a material becomes a superconductor, it actively expels magnetic fields from its interior. It does this by creating a surface current that generates an opposing magnetization ($M^s$).

However, expelling a magnetic field takes **work**. You have to fight against the magnetic field to push it out. This means the Superconducting state gains extra potential energy when placed in a magnetic field. Eventually, if the field ($B$) gets too strong, the energy cost is too high, and the material gives up—it snaps back to the Normal phase. This limit is called the **Critical Field ($B_c$)**.

### 2. Step 1: Calculating the Magnetic Energy Cost

We need to calculate how much free energy is added to the superconductor by this magnetization work.

-   **The Work Formula:** The problem gives us the differential work: $dW = -B dM$.
    
-   **The Magnetization:** The problem states that to cancel the field, the magnetization must be $M^s = -\frac{V}{4\pi}B$.
    

Let's integrate this to find the total magnetic energy required to build up the field from $0$ to $B$.

First, find the relationship between $dM$ and $dB$:

$$M = -\frac{V}{4\pi} B \quad \Rightarrow \quad dM = -\frac{V}{4\pi} dB$$

Now substitute this into the work integral:

$$W_{mag} = \int - B (dM) = \int_{0}^{B} -B \left( -\frac{V}{4\pi} dB' \right)$$

$$W_{mag} = \frac{V}{4\pi} \int_{0}^{B} B' dB'$$

Performing the integral ($\int x dx = \frac{1}{2}x^2$):

$$W_{mag} = \frac{V}{4\pi} \left[ \frac{B'^2}{2} \right]_0^B = \frac{V B^2}{8\pi}$$

**Physical Meaning:** This term $\frac{V B^2}{8\pi}$ is positive. It represents the energy penalty added to the superconductor's Free Energy because it is expelling the field.

### 3. Step 2: The New Equilibrium Condition

Now we update our Free Energy comparison.

-   **Superconductor:** $F^s(B) = F^s(B=0) + \frac{V B^2}{8\pi}$
    
-   **Normal Metal:** The problem states $M^n=0$, so it does not interact with the field (in this approximation). $F^n(B) = F^n(B=0)$.
    

The **Critical Field $B_c(T)$** is the specific field strength where the superconductor's energy rises so much that it exactly equals the normal metal's energy. At this point, the phase transition happens.

$$F^s(B_c) = F^n$$

$$F^s(0) + \frac{V B_c^2}{8\pi} = F^n(0)$$

Rearranging to isolate the magnetic term:

$$\frac{V B_c^2}{8\pi} = F^n(0) - F^s(0)$$

### 4. Step 3: Substitution and Algebra

We already calculated the difference $F^n(0) - F^s(0)$ in Part (d)!

Recall that $F^n - F^s = V\Delta + \frac{\alpha-\beta}{12}VT^4 - \frac{\gamma}{2}VT^2$ (from rearranging eq 104 in the solution).

Substituting this into our magnetic equation (and cancelling the Volume $V$):

$$\frac{B_c^2}{8\pi} = \Delta + \frac{\alpha - \beta}{12} T^4 - \frac{\gamma}{2} T^2$$

Now, we need to eliminate the Greek letters ($\alpha, \beta, \gamma$) to get the answer in the form requested ($B_0$ and $T_c$). We use the relationships we found in previous parts:

1.  **From Part (b):** $(\alpha - \beta) = \frac{3\gamma}{T_c^2}$.
    
2.  **From Part (d):** $\gamma = \frac{4\Delta}{T_c^2}$ (derived from $\Delta = \frac{\gamma}{4}T_c^2$).
    

**Let's substitute:**

First, replace $(\alpha - \beta)$:

$$\frac{B_c^2}{8\pi} = \Delta + \frac{1}{12} \left( \frac{3\gamma}{T_c^2} \right) T^4 - \frac{\gamma}{2} T^2$$

$$\frac{B_c^2}{8\pi} = \Delta + \frac{\gamma}{4} \frac{T^4}{T_c^2} - \frac{\gamma}{2} T^2$$

Next, replace $\gamma$ with $\frac{4\Delta}{T_c^2}$:

$$\frac{B_c^2}{8\pi} = \Delta + \frac{1}{4} \left( \frac{4\Delta}{T_c^2} \right) \frac{T^4}{T_c^2} - \frac{1}{2} \left( \frac{4\Delta}{T_c^2} \right) T^2$$

Simplify the fractions:

$$\frac{B_c^2}{8\pi} = \Delta + \Delta \frac{T^4}{T_c^4} - 2\Delta \frac{T^2}{T_c^2}$$

Factor out $\Delta$:

$$\frac{B_c^2}{8\pi} = \Delta \left( 1 - 2\frac{T^2}{T_c^2} + \left(\frac{T^2}{T_c^2}\right)^2 \right)$$

Do you recognize the term in the parentheses? It is a perfect square: $(1 - x)^2 = 1 - 2x + x^2$, where $x = \frac{T^2}{T_c^2}$.

$$\frac{B_c^2}{8\pi} = \Delta \left( 1 - \frac{T^2}{T_c^2} \right)^2$$

### 5. Final Result

Now, solve for $B_c$ by taking the square root of both sides:

$$B_c(T) = \sqrt{8\pi\Delta} \left( 1 - \frac{T^2}{T_c^2} \right)$$

The problem asks us to identify $B_0$ from the form $B_c(T) = B_0 (1 - \frac{T^2}{T_c^2})$.

Comparing the two equations, we can clearly see:

$$B_0 = \sqrt{8\pi\Delta}$$

### Summary

-   We calculated the energy cost of expelling the magnetic field: $\frac{B^2}{8\pi}$.
    
-   We equated the Free Energies to find the "tipping point" (Critical Field).
    
-   We used our previous results to simplify the math into a clean parabola formula.
    
-   **Result:** The critical field at absolute zero is determined purely by the Cooper pair binding energy: $B_0 = \sqrt{8\pi\Delta}$.
    

Congratulations! You have just solved a complete, multi-stage problem modeling the thermodynamics of a superconductor. This is real, high-level physics derived from first principles!