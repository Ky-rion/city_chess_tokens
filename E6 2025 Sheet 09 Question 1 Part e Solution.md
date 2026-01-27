

![[Pasted image 20260126135245.png]]

Great work sticking with this! We have finally arrived at the "prize" of this derivation.

In part **(e)**, we are going to convert our abstract quantum wavevectors ($\delta\vec{k}$) into something you can actually measure with a multimeter: **Current Density ($\vec{J}$)** and **Conductivity ($\sigma$)**.

This derivation leads to the famous **Drude Formula** for conductivity.

---

### 1. The Definitions (What are we building?)

**The Question (Image 1):**

> "Show that the following relationship results for the current flow... and thus the electrical conductivity $\sigma_{el}$."

We need to connect microscopic particle motion to macroscopic current.

**The Recipe for Current Density ($\vec{J}$):**

Imagine you are standing by a river counting water molecules flowing past. The "current" depends on three things:

1.  **Who is flowing?** The charge of the particle ($q = -e$).
    
2.  **How many?** The density of particles ($n$).
    
3.  **How fast?** The drift velocity ($\vec{v}_{drift}$).
    

So, the formula for current density is:

$$\vec{J}_{el} = n \cdot (-e) \cdot \vec{v}_{drift}$$

---

### 2. The Substitution Game (The Derivation)

Let's follow the professor's logic in the second image step-by-step.

#### Step A: Translate Velocity to Wavevector

We don't have velocity $\vec{v}$ in our previous answers; we have the wavevector shift $\delta\vec{k}$. We need to convert them.

Recall the relation between momentum, velocity, and wavevector:

$$m\vec{v} = \vec{p} = \hbar\vec{k}$$

$$\Rightarrow \vec{v} = \frac{\hbar}{m}\vec{k}$$

So, the **drift velocity** (the extra speed gained from the field) corresponds to the **shift** in the wavevector:

$$\vec{v}_{drift} = \frac{\hbar}{m} \delta\vec{k}$$

#### Step B: Plug into the Current Equation

Substitute this expression for velocity back into our current density formula:

$$\vec{J}_{el} = -e \cdot n \cdot \left( \frac{\hbar}{m} \delta\vec{k} \right)$$

$$\vec{J}_{el} = -\frac{en\hbar}{m} \delta\vec{k}$$

_(This matches the first part of the solution in the image!)_

#### Step C: The Grand Substitution

Now, remember the result from **part (d)**? We found that the equilibrium shift is:

$$\delta\vec{k} = -\frac{e\tau}{\hbar}\vec{E}$$

Plug _that_ into our current equation:

$$\vec{J}_{el} = -\frac{en\hbar}{m} \cdot \left( -\frac{e\tau}{\hbar}\vec{E} \right)$$

#### Step D: The Cleanup

Now, look at the algebra.

1.  The two minus signs cancel out ($(-)\cdot(-) = +$).
    
2.  The $\hbar$ in the numerator and the $\hbar$ in the denominator cancel out.
    
3.  We have two $e$'s, so that becomes $e^2$.
    

What are we left with?

$$\vec{J}_{el} = \frac{n e^2 \tau}{m} \vec{E}$$

---

### 3. The Finale: Finding Conductivity ($\sigma$)

We have just derived a microscopic version of **Ohm's Law**.

-   **Macroscopic Ohm's Law:** $V = I \cdot R$
    
-   **Microscopic Ohm's Law:** $\vec{J} = \sigma \cdot \vec{E}$
    

If we look at our result:

$$\vec{J}_{el} = \underbrace{\left( \frac{n e^2 \tau}{m} \right)}_{\text{This must be } \sigma} \cdot \vec{E}$$

Therefore, the electrical conductivity is:

$$\sigma_{el} = \frac{n e^2 \tau}{m}$$

---

### 4. Professor's Insight: How to read this formula

This simple fraction tells you everything about why some metals are better conductors than others.

$$\sigma = \frac{n e^2 \tau}{m}$$

1.  **$n$ (Electron Density):** The more charge carriers you have, the better the conductivity. (This is why metals conduct better than semiconductors).
    
2.  **$e^2$ (Coupling):** How strongly electrons interact with the field.
    
3.  **$\tau$ (Relaxation Time):** This is the most crucial part. It tells us **how long an electron flies before crashing.**
    
    -   **Cold Metal:** Atoms vibrate less $\rightarrow$ fewer crashes $\rightarrow$ larger $\tau$ $\rightarrow$ **Higher Conductivity**.
        
    -   **Hot Metal:** Atoms vibrate violently $\rightarrow$ frequent crashes $\rightarrow$ smaller $\tau$ $\rightarrow$ **Lower Conductivity**.
        
4.  **$m$ (Mass):** The heavier the particle, the harder it is to push. (Note: In real solids, we use "effective mass" $m^*$ because the lattice changes the electron's inertia).
    

**You have successfully derived the Drude-Sommerfeld model of conduction!**

That concludes this problem set. Would you like to try calculating the actual conductivity for Copper using this formula, or should we tackle a new topic?