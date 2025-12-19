

This is the grand finale! You have done the hard work of setting up the Schrödinger equation and solving it. Now, you get to apply that theory to a specific "what if" scenario.

The question asks: **"What is the ground state energy if one doubles the width of the potential well in the x-direction?"**

To prove this mathematically, we need to generalize the energy formula we derived in Part (3c).

### 1. The General Formula for a Rectangular Box

In Part (3c), we derived the energy for a square box where $L_x = a$ and $L_y = a$.

$$E_{m,n} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{m^2}{a^2} + \frac{n^2}{a^2} \right)$$

However, if we look back at our separation of variables in Part (3b), we recall that the energy contributions from $x$ and $y$ are independent.

$$E = E_x + E_y$$

The general formula for a **rectangular** box with width $L_x$ and height $L_y$ is:

$$E_{m,n} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{m^2}{L_x^2} + \frac{n^2}{L_y^2} \right)$$

This is the key theoretical formula you need to argue your case. It shows that energy is **inversely proportional to the square of the width**. In simpler terms: **Wider box = Lower energy.**

---

### 2. Applying the Changes

Now, let's plug in the specific changes from the question text.

-   **Original Setup:** $L_x = a$ and $L_y = a$.
    
-   **New Setup:** The problem states we double the width in the x-direction.
    
    -   New $L_x = 2a$
        
    -   New $L_y = a$ (unchanged)
        

We are looking for the Ground State, which means the lowest possible energy. This occurs when the quantum numbers are the smallest possible integers:

$$m = 1, \quad n = 1$$

---

### 3. The Calculation

Substitute the new dimensions and quantum numbers into our general formula:

$$E'_{1,1} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{1^2}{(2a)^2} + \frac{1^2}{a^2} \right)$$

Let's simplify the term inside the parenthesis. Note that $(2a)^2 = 4a^2$.

$$E'_{1,1} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{1}{4a^2} + \frac{1}{a^2} \right)$$

To add these fractions, find a common denominator (which is $4a^2$):

$$E'_{1,1} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{1}{4a^2} + \frac{4}{4a^2} \right)$$

$$E'_{1,1} = \frac{\hbar^2 \pi^2}{2M} \left( \frac{5}{4a^2} \right)$$

Now, pull the constants together to match the format of your previous answers:

$$\boxed{E'_{1,1} = \frac{5}{4} \frac{\hbar^2 \pi^2}{2Ma^2}}$$

---

### 4. Interpretation (The "Physics" Check)

Does this make sense? Let's compare it to the original ground state energy.

-   **Original Energy:** $E_{1,1} = \frac{\hbar^2 \pi^2}{2Ma^2} (1 + 1) = \mathbf{2} \cdot [\text{constants}]$
    
-   **New Energy:** $E'_{1,1} = \mathbf{1.25} \cdot [\text{constants}]$
    

The energy went down (from 2 units to 1.25 units). This matches our physical intuition: **Confining a quantum particle requires energy.** If you relax the confinement (by making the box wider), the "pressure" drops, and the energy decreases. Specifically, the energy associated with the x-motion dropped to $1/4$ of its original value, while the y-energy stayed the same.

### Summary

You have successfully completed the entire problem set!

1.  **3a:** You built the Hamiltonian operator.
    
2.  **3b:** You separated the variables.
    
3.  **3c:** You found the wavefunctions and energy formula.
    
4.  **3d:** You calculated the energy levels and degeneracy.
    
5.  **3e:** You visualized the probability distribution.
    
6.  **3f:** You applied the theory to a modified geometry.
    

**That concludes our session on the 2D infinite well! Would you like a quick summary sheet of all the final formulas we derived, or are you ready to tackle a new topic?**