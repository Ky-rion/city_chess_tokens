

![[Pasted image 20260128115957.png]]
![[Pasted image 20260128120014.png]]

This is a fantastic follow-up question! It introduces one of the most clever techniques used in particle physics: the **Double Angle Method**.

In Part (a), we just smashed things together. In Part (b), we are trying to measure the collision properties ($Q^2$) without relying on measuring energies directly.

**Why do we do this?**

Measuring the exact **energy** of a particle in a detector is often difficult and prone to errors (uncertainties). However, measuring **where** a particle goes (its angle) is usually very precise. By converting our formulas to depend on angles ($\theta$ and $\gamma$) instead of energies, we get a much more accurate result!

Let's walk through the derivation step-by-step.

---

### 1. The Setup: Conservation Laws

We are looking at a collision between an electron (energy $E_e$) and a quark inside the proton.

-   The **electron** scatters at angle $\theta$ with new energy $E'_e$.
    
-   The **quark** scatters at angle $\gamma$ with new energy $E'_q$.
    

We start with three fundamental laws of physics provided in the solution:

1.  **Conservation of Energy:** The total energy coming in equals the total energy going out.
    
    $$E_e + xE_p = E'_e + E'_q \quad \dots \text{(i)}$$
    
2.  **Transverse Momentum ($p_T$):** The electron and quark must balance each other sideways. If the electron goes "up", the quark goes "down".
    
    $$E'_e \sin(\theta) = E'_q \sin(\gamma) \quad \dots \text{(ii)}$$
    
    _(Note: We cancelled the $c$'s here)_
    
3.  **Longitudinal Momentum ($p_L$):** The momentum along the beam pipe must be conserved.
    
    $$(xE_p - E_e) = E'_q \cos(\gamma) - E'_e \cos(\theta) \quad \dots \text{(iii)}$$
    

---

### 2. The Strategy

Our goal is to find an equation for the final electron energy $E'_e$ that **only** contains angles ($\theta, \gamma$) and the initial electron energy ($E_e$). We want to eliminate the unknown quark variables ($E'_q$).

**Step A: Eliminate the Proton term ($xE_p$)**

We can combine the Energy equation (i) and the Longitudinal Momentum equation (iii) to get rid of the incoming proton/quark term ($xE_p$).

From the solution, we rearrange eq (iii) to solve for $xE_p$:

$$xE_p = E'_q \cos(\gamma) - E'_e \cos(\theta) + E_e$$

Substitute this into the Energy equation (i):

$$E_e + [E'_q \cos(\gamma) - E'_e \cos(\theta) + E_e] = E'_e + E'_q$$

Group the terms together:

$$2E_e = E'_e(1 + \cos\theta) + E'_q(1 - \cos\gamma)$$

_Wait! The solution takes a slightly different algebraic path, but the destination is the same. Let's follow the solution's specific steps to match your image exactly._

**The Solution's Path:**

They rewrite eq (i) to isolate $E'_e$, but they sneakily substitute the term $(xE_p - E_e)$ from eq (iii) into it.

$$E'_e = [E'_q \cos(\gamma) - E'_e \cos(\theta)] + 2E_e - E'_q$$

$$E'_e = E'_q [\cos(\gamma) - 1] - E'_e \cos(\theta) + 2E_e$$

This equation now has both unknown final energies ($E'_e$ and $E'_q$). We need to kill $E'_q$.

**Step B: Eliminate the Quark Energy ($E'_q$)**

We use the **Transverse Momentum** equation (ii). This is our bridge between the electron and the quark.

$$E'_q = E'_e \frac{\sin(\theta)}{\sin(\gamma)}$$

Substitute this into our big equation from Step A:

$$E'_e = \left( E'_e \frac{\sin(\theta)}{\sin(\gamma)} \right) [\cos(\gamma) - 1] - E'_e \cos(\theta) + 2E_e$$

Now, every term has $E'_e$ except the $2E_e$ part. We are close!

---

### 3. The Trigonometry Gym

Now we just need to clean up the algebra to solve for $E'_e$. Move all the $E'_e$ terms to the left side:

$$E'_e \left[ 1 + \cos(\theta) - \frac{\sin(\theta)}{\sin(\gamma)}(\cos(\gamma) - 1) \right] = 2E_e$$

Let's simplify that messy bracket. We find a common denominator ($\sin \gamma$):

$$[\dots] = \frac{\sin(\gamma) + \sin(\gamma)\cos(\theta) - \sin(\theta)\cos(\gamma) + \sin(\theta)}{\sin(\gamma)}$$

Do you see the hidden identity? Look at the middle two terms:

$$\sin(\gamma)\cos(\theta) - \sin(\theta)\cos(\gamma) = \sin(\gamma - \theta)$$

So the bracket becomes:

$$\frac{\sin(\gamma) + \sin(\theta) + \sin(\gamma - \theta)}{\sin(\gamma)}$$

Now, we flip this fraction to the other side to solve for $E'_e$:

$$E'_e = \frac{2E_e \sin(\gamma)}{\sin(\gamma) + \sin(\theta) + \sin(\gamma - \theta)}$$

---

### 4. The Final Calculation for $Q^2$

The problem asks for $Q^2$. From Exercise 2 (referenced in the text), we know the standard formula for momentum transfer squared depends on the scattered energy and angle:

$$Q^2 = \frac{2 E_e E'_e (1 - \cos \theta)}{c^2}$$

_(Note: Sometimes $c=1$ in physics units, but we keep it here for completeness)._

We take our big new formula for $E'_e$ and plug it into this $Q^2$ equation:

$$Q^2 = \frac{2 E_e (1 - \cos \theta)}{c^2} \cdot \left[ \frac{2E_e \sin(\gamma)}{\sin(\gamma) + \sin(\theta) + \sin(\gamma - \theta)} \right]$$

Combine the constants ($2 \times 2 = 4$) and $E_e$:

$$Q^2 = \frac{4 E_e^2 \sin(\gamma) (1 - \cos \theta)}{[\sin(\gamma) + \sin(\theta) + \sin(\gamma - \theta)] c^2}$$

### Professor's Summary

You have successfully derived the **Double Angle Formula**!

-   **What you did:** You took conservation laws (Energy, Momentum) and rearranged them.
    
-   **The Result:** You found a way to calculate $Q^2$ using **only** the beam energy ($E_e$) and the angles $\theta$ and $\gamma$.
    
-   **The Benefit:** You don't need to trust the energy measurement of the calorimeter. As long as you can track _where_ the particles went (the angles), you can get the right answer. This is crucial for precision experiments like those at HERA.
    

Would you like to try applying this formula with some real numbers, or move on to the next concept?