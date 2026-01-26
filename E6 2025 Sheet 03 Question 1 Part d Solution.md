

![[Pasted image 20260125183046.png]]

Welcome to Part (d)! This is where we stop just drawing pictures and start calculating real physical distances. This is crucial for experiments like X-ray diffraction, where we actually measure these distances to figure out what a material is made of.

### The Topic: Interplanar Spacing ($d_{hkl}$)

We are asked to calculate the **distance** between the parallel planes we identified in part (ii).

In Crystallography, you don't just have _one_ plane. When we say "the (120) plane," we are actually talking about an infinite stack of parallel planes slicing through the entire crystal. The variable **$d_{hkl}$** represents the perpendicular distance between two neighboring planes in that stack.

### The "Magic Formula" for Cubic Crystals

For a **cubic** system (where all sides are 90° and equal length), the distance $d$ is related to the lattice constant $a$ and the Miller indices $(h \ k \ l)$ by this formula:

$$d_{hkl} = \frac{a}{\sqrt{h^2 + k^2 + l^2}}$$

Your professor’s solution uses a slightly rearranged version of this (squared), which is often easier to type:

$$\frac{1}{d^2_{hkl}} = \frac{h^2 + k^2 + l^2}{a^2}$$

Both formulas do exactly the same thing. Let's use the first one because it's more intuitive: "The distance gets smaller as the indices get bigger."

---

### Step-by-Step Calculation

**1. Gather the Variables**

-   **$a = 6$ Å**.
    
    -   _Note:_ The symbol Å stands for **Angstrom**. $1 \text{ \AA} = 10^{-10}$ meters. It is the standard ruler for measuring atoms.
        
-   **Indices $(h \ k \ l)$**: The solution uses the plane from part (ii), which they identified as **(1 2 0)**.
    

**2. Handle the "Typo" Controversy**

Remember in Part (b) we noticed the drawing looked like (210) but the text said (120)?

Here is the good news: **For this calculation, it doesn't matter!**

Because we are squaring the numbers ($h^2 + k^2$), and $1^2 + 2^2$ is the same as $2^2 + 1^2$, the distance $d$ is identical regardless of which axis is which. Symmetry saves us!

**3. Plug into the Formula**

Let's substitute our numbers:

-   $h = 1$
    
-   $k = 2$
    
-   $l = 0$
    

$$d_{120} = \frac{6 \text{ \AA}}{\sqrt{1^2 + 2^2 + 0^2}}$$

**4. Solve the Math**

$$d_{120} = \frac{6}{\sqrt{1 + 4 + 0}}$$

$$d_{120} = \frac{6}{\sqrt{5}}$$

Now, we just calculate $\sqrt{5} \approx 2.236$.

$$d_{120} = \frac{6}{2.236} \approx 2.68 \text{ \AA}$$

---

### Understanding the Professor's Solution Steps

Your professor did the calculation using the "squared" method. Let's trace his steps so you can follow his sheet:

1.  He set up the equation: $\frac{1}{d^2} = \frac{1^2 + 2^2 + 0^2}{6^2}$.
    
2.  He squared the bottom: $6^2 = 36$.
    
3.  He summed the top: $1 + 4 = 5$.
    
4.  This gave him the fraction $\frac{5}{36}$.
    
5.  In decimal form: $5 \div 36 \approx 0.14 \text{ \AA}^{-2}$ (This is the value of $1/d^2$).
    
6.  Finally, to get $d$, he took the inverse square root: $\sqrt{1 / 0.14} \approx 2.68 \text{ \AA}$.
    

Both methods lead to the exact same answer: **2.68 Å**.

### Summary for your notes

-   **The Physical Meaning:** In this crystal, the parallel sheets of atoms labeled (120) are separated by a gap of 2.68 Angstroms.
    
-   **The Trend:** Notice that $2.68$ is much smaller than the side of the box ($6$). This is normal. The more "tilted" the plane (higher indices), the closer together the layers get.
    

You have now mastered drawing planes, naming them, identifying their symmetries, and calculating their spacing. That is a huge chunk of Chapter 1 in Solid State Physics! Is there another problem set, or should we review any part of this one?