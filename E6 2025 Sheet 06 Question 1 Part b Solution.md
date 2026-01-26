

![[Pasted image 20260125184216.png]]
![[Pasted image 20260125184222.png]]

That is a fantastic follow-up question. In physics, we often look at "limits"—what happens when things get extremely cold ($T \to 0$) or extremely hot ($T \to \infty$).

In part (a), we saw that the Einstein and Debye models look very different at low temperatures. However, **part (b)** asks us to explain why they suddenly agree when things get hot.

Let's break down the solution provided in the image.

---

### 1. The Name of the Limit

First, to answer the specific question _"How is this limit designated?"_:

This constant value is called the **Dulong-Petit Law**.

> **Historical Note:** Pierre Dulong and Alexis Petit discovered this experimentally in 1819, long before quantum mechanics existed. They noticed that for almost all simple solids, the heat capacity was roughly the same number (about $25 \text{ J}/(\text{mol}\cdot\text{K})$).

---

### 2. The Explanation ("Why do they agree?")

The German solution text gives the core physical reasoning. Let's translate it and then unpack the physics.

**Translation of the Solution:**

> _"At high temperatures, every degree of freedom of the crystal possesses the same mean energy, and every degree of freedom (both according to the Einstein model and in the Debye model) is occupied/excited. The total number of existing degrees of freedom is identical for both models, so that according to Dulong-Petit, the same high-temperature limit of the specific heat capacity results."_

**The Professor's Deep Dive:**

To understand this, we need to understand the concept of **"Degrees of Freedom"** and the **"Equipartition Theorem."**

**A. Degrees of Freedom**

Imagine a crystal made of $N$ atoms.

-   Each atom can move in 3 directions: up-down, left-right, forward-back ($x, y, z$).
    
-   Therefore, the total number of ways the system can vibrate (the total "degrees of freedom") is **$3N$**.
    
-   **Crucial Point:** Both Einstein and Debye agree on this. Whether you treat them as independent springs (Einstein) or sound waves (Debye), you cannot create or destroy movement modes. You always have exactly $3N$ modes of vibration.
    

**B. The "High Temperature" Washout**

Quantum mechanics says that energy comes in steps (quanta).

-   **At Low T:** It's hard to get up the first "step" of energy. High-frequency modes stay "frozen out" (stuck in the ground state). This is where the models differ—Debye handles the "easy" low steps better than Einstein.
    
-   **At High T:** There is so much thermal energy available that the "steps" look tiny. It’s like walking up a staircase that is so small it feels like a smooth ramp. The quantum differences disappear, and classical physics takes over.
    

**C. The Equipartition Theorem**

This is a classical rule that says: _If you heat a system up enough, every single degree of freedom gets an equal share of energy._

-   That share is exactly $k_B T$ (Boltzmann constant $\times$ Temperature) per vibration mode.
    

**D. Putting it together**

Since both models have the same number of modes ($3N$), and at high temperatures, every single mode gets filled with the same energy ($k_B T$), the total energy $U$ becomes:

$$U = (\text{Total Modes}) \times (\text{Energy per Mode})$$

$$U = 3N \times k_B T$$

Now, calculate the Heat Capacity ($C_V$), which is just the change in energy with temperature ($\frac{dU}{dT}$):

$$C_V = \frac{d}{dT} (3N k_B T) = 3N k_B$$

Since $N k_B = R$ (the Gas Constant), this equals **$3R$**.

---

### Summary for your notes

1.  **The Limit:** It is called the **Dulong-Petit Law**.
    
2.  **The Reason:**
    
    -   Both models conserve the total number of **degrees of freedom ($3N$)**.
        
    -   At high temperatures, there is enough thermal energy to excite **all** these modes fully.
        
    -   The specific details of the frequencies (whether they are all the same like Einstein, or distributed like Debye) stop mattering because **every mode contributes equally** ($k_B T$) to the energy.
        

**Professor's Check-in:** Does the idea that "high heat makes quantum steps look like a smooth ramp" help visualize why the two models converge? We can move on to part c) whenever you are ready!