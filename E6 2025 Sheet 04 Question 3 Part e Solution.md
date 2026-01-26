

![[Pasted image 20260125184051.png]]

Welcome to the final practical application! Now that we have derived the fancy formula, we get to be engineers and crunch the numbers. This step connects the abstract math to reality.

Part (e) asks us to calculate the specific number of defects ($n$) for a **Silver Bromide (AgBr)** crystal of volume $1 \text{ mm}^3$ at two very different temperatures: **100 K** (very cold) and **900 K** (very hot).

Let’s break down the professor's solution image (Image 2) step-by-step.

---

### Step 1: Finding $N$ (Total Possible Sites)

Before we can find the number of "holes" ($n$), we need to know the number of "seats" ($N$) available in the theater.

**The Professor's Logic:**

> _"Pro Einheitszelle können jeweils 4 Anionen/Kationen ... daher $N_{EZ} = 4$."_

**Explanation:**

1.  **Structure:** AgBr crystallizes in a "Rock Salt" (NaCl) structure. In this specific crystal layout, there are **4 formula units** (4 Cations + 4 Anions) inside every single Unit Cell. That means there are 4 possible spots for a defect to occur per cube.
    
2.  **Volume of one Cell:** The problem gives the lattice constant $a = 580 \text{ pm}$. The volume of one tiny unit cell is $a^3$.
    
3.  **Total Cells:** How many tiny boxes fit in our big $1 \text{ mm}^3$ crystal?
    
    $$\text{Number of Cells} = \frac{V_{\text{total}}}{a^3}$$
    
4.  **Total Sites ($N$):** Multiply the number of cells by the number of sites per cell (4).
    
    $$N = \frac{V}{a^3} \cdot 4$$
    

---

### Step 2: The Master Formula

We take the formula we derived in Part (d):

$$\frac{n}{N} = \exp\left( -\frac{\Delta H_S}{2 k_B T} \right)$$

And rearrange it to solve for $n$ (Equation 23 in the solution):

$$n \approx \left( \frac{V}{a^3} \cdot 4 \right) \cdot \exp\left( -\frac{\Delta H_S}{2 k_B T} \right)$$

---

### Step 3: The Calculation (Watch your Units!)

This is where students often lose points on exams. You must convert everything to standard units (**Meters**).

-   **Volume ($V$):** $1 \text{ mm}^3 = (10^{-3} \text{ m})^3 = 10^{-9} \text{ m}^3$.
    
-   **Lattice Constant ($a$):** $580 \text{ pm} = 580 \cdot 10^{-12} \text{ m} = 5.8 \cdot 10^{-10} \text{ m}$.
    
-   **Energy ($\Delta H_S$):** $2.76 \cdot 10^{-19} \text{ J}$.
    
-   **Boltzmann Constant ($k_B$):** $\approx 1.38 \cdot 10^{-23} \text{ J/K}$.
    

---

### Step 4: The Results & Physics Interpretation

Let's look at the numbers the professor calculated. They tell a fascinating story about how temperature controls matter.

#### Case 1: The Deep Freeze ($T = 100 \text{ K}$)

$$n(100 \text{ K}) \approx 8 \cdot 10^{-25}$$

**Wait, what?**

How can you have $10^{-25}$ of a defect? You can't have 0.000...001 of a hole!

-   **Physics Meaning:** This number is essentially **Zero**.
    
-   The probability is so astronomically low that in a crystal of this size ($1 \text{ mm}^3$), you will never find a single defect. The crystal is "perfect" because it doesn't have enough thermal energy to pay the "energy bill" to create even one hole.
    

#### Case 2: The Oven ($T = 900 \text{ K}$)

$$n(900 \text{ K}) \approx 3 \cdot 10^{14}$$

**The Explosion:**

Just by heating it up, we went from **Zero** to **300 Trillion** defects!

-   **Physics Meaning:** The exponential term ($\exp$) is incredibly sensitive to temperature. At 900 K, the thermal vibrations are strong enough that atoms are constantly popping out of their spots.
    
-   Even though $3 \cdot 10^{14}$ sounds huge, compared to the total number of atoms ($\approx 10^{19}$), it is still a small fraction (about 1 in 100,000 atoms is missing). But this is enough to completely change the electrical conductivity of the material.
    

---

### Final Summary

This entire problem walked you through the lifecycle of Solid State Physics:

1.  **Visualize** the defect (Part a).
    
2.  **Explain** why it happens using Thermodynamics ($G = H - TS$) (Part b).
    
3.  **Quantify** the chaos using Combinatorics ($S = k \ln W$) (Part c).
    
4.  **Derive** the master equation (Part d).
    
5.  **Calculate** real-world numbers to see the power of Temperature (Part e).
    

You have now mastered Schottky Defects! Is there anything else about this topic (or a new problem) you'd like to discuss?