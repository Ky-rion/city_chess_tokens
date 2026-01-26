

![[Pasted image 20260125184243.png]]

Welcome back to class! We are moving from the abstract theory to a concrete calculation. This is where physics gets real—we are going to calculate a number you could actually measure in a lab.

We are answering **Part (c)**: _"Calculate the high-temperature limit of the heat capacity of a piece of Gold (6 g)."_

Let's break down the solution provided by your other professor. It involves three simple steps, but there is a **small typo** in the solution image that I will help you spot!

---

### Step 1: Establish the "Molar" Heat Capacity

First, we need the "standard" value for one mole of atoms. As we learned in part (b), at high temperatures, the Einstein and Debye models both agree on the **Dulong-Petit law**.

The solution states that the Molar Heat Capacity ($C_{V,m}$) is:

$$C_{V,m} = 3 \cdot N_A \cdot k_B = 3R$$

Where:

-   $N_A$ is Avogadro's constant.
    
-   $k_B$ is the Boltzmann constant.
    
-   $R$ is the universal gas constant ($R \approx 8.314 \text{ J}/(\text{mol}\cdot\text{K})$).
    

So, for **any** simple solid element at room temperature (or higher), the heat capacity per mole is roughly:

$$C_{V,m} \approx 24.94 \text{ J}/(\text{mol}\cdot\text{K})$$

---

### Step 2: How much Gold do we have?

We don't have one mole; we have **6 grams**. We need to find out what fraction of a mole this is.

To do this, we look at the Periodic Table (or the data provided in the solution) to find the **Molar Mass ($M$)** of Gold (Au).

-   **Molar Mass of Gold:** $M = 196.97 \text{ g/mol}$.
    

Now we calculate the number of moles ($n$):

$$n = \frac{\text{mass} (m)}{\text{Molar Mass} (M)} = \frac{6 \text{ g}}{196.97 \text{ g/mol}} \approx 0.0305 \text{ mol}$$

---

### Step 3: The Calculation (and the Typo Alert!)

Now we just multiply the amount of substance (moles) by the heat capacity per mole.

$$C_V = n \cdot 3R = \frac{6 \text{ g}}{196.97 \text{ g/mol}} \cdot 24.94 \frac{\text{J}}{\text{mol}\cdot\text{K}}$$

$$C_V \approx 0.76 \text{ J/K}$$

**⚠️ Professor's Note on the Solution Image Typo:**

If you look closely at the red text in the solution equation (2), it writes:

$$3R \frac{0.006\text{g}}{196.97}$$

**This is a mistake.** If you calculate that literally, the answer would be tiny ($0.00076$). The author likely converted 6g to 0.006 **kg** in their head but wrote "g" and kept the molar mass in g/mol.

To get the correct answer of **0.76 J/K**, you must use **6g** in the numerator to match the **g/mol** in the denominator.

---

### Step 4: Understanding the Graph

The solution includes a scatter plot that is very important for your intuition.

-   **X-axis:** Atomic Number (Ordnungszahl).
    
-   **Y-axis:** Molar Heat Capacity.
    
-   **The Line:** Notice the horizontal line labeled **3R** (at approx 25 J/mol K).
    
-   **The Data Points:** Look at how all the different elements (Li, Al, Cu, Ag, and **Au** for Gold) cluster right around that line!
    

**The Takeaway:**

The text below the graph makes a crucial point: _"The underlying crystal structure (sc, bcc, fcc...) of the elements does not have to be considered separately."_

This means that at high temperatures, it doesn't matter if your atoms are stacked in cubes (sc) or face-centered patterns (fcc). Heat is just random jiggling, and the Dulong-Petit law ($3R$) is a universal rule that ignores these structural details.

**Ready for the next question? Or would you like to verify the units of that calculation together?**