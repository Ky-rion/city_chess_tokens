

![[Pasted image 20260125185657.png]]

Excellent! Let’s jump into Part (b).

In Part (a), we counted the atoms. Now, in Part (b), we are going to measure how "stiff" the bonds between these atoms are.

### 1. Translating the Problem

**German:** _"Berechnen Sie die Federkonstante $K$ des Systems. (Nehmen Sie an: $m_{Atom} = 7 \times 10^{-27}$ kg)"_

**English:** "Calculate the spring constant $K$ of the system. (Assume the mass of an atom is $m_{Atom} = 7 \times 10^{-27}$ kg)."

**The Goal:** Find $K$.

In solid-state physics, we imagine the bonds between atoms as tiny springs.

-   If $K$ is **high**, the spring is stiff (hard material, like diamond).
    
-   If $K$ is **low**, the spring is loose (soft material, like lead or solid helium).
    

---

### 2. The Missing Variable: The "Lattice Constant" ($a$)

Look at the formula provided in the solution snippet:

$$v_s = a \sqrt{\frac{K}{m}}$$

We know:

-   $v_s = 796$ m/s (Speed of sound, given in part a)
    
-   $m = 7 \times 10^{-27}$ kg (Mass of one atom, given in part b)
    
-   $K$ is what we want to find.
    

**But what is $a$?**

The variable $a$ is called the **Lattice Constant**. It is simply the distance between two neighboring atoms in our chain.

The problem doesn't give us $a$ directly, but we can calculate it easily using the result from Part (a)!

Imagine you have a chain of length $L$ and it is made of $N$ atoms. The distance between each atom is just the total length divided by the number of atoms.

$$a = \frac{L}{N}$$

Using the values we have:

-   $L = 0.30$ m (30 cm)
    
-   $N = 10^9$ (Answer from Part a)
    

$$a = \frac{0.30 \text{ m}}{10^9} = 3.0 \times 10^{-10} \text{ m}$$

_(Note: $10^{-10}$ meters is 1 Ångström, or 0.1 nanometers. So $a = 0.3$ nm. This is a very typical spacing for atoms in a solid!)_

---

### 3. The Algebra: Isolating $K$

Now we go back to the speed of sound formula and rearrange it to solve for $K$.

$$v_s = a \sqrt{\frac{K}{m}}$$

**Step 1:** Divide both sides by $a$.

$$\frac{v_s}{a} = \sqrt{\frac{K}{m}}$$

**Step 2:** Square both sides to get rid of the square root.

$$\left(\frac{v_s}{a}\right)^2 = \frac{K}{m}$$

**Step 3:** Multiply by $m$ to get $K$ by itself.

$$K = m \left(\frac{v_s}{a}\right)^2$$

---

### 4. The Calculation

Now we plug in our numbers. Be careful with the scientific notation!

$$K = (7 \times 10^{-27} \text{ kg}) \times \left( \frac{796 \text{ m/s}}{3.0 \times 10^{-10} \text{ m}} \right)^2$$

Let's do the part inside the parentheses first (the frequency):

$$\frac{796}{3.0 \times 10^{-10}} \approx 265.33 \times 10^{10} = 2.65 \times 10^{12} \text{ Hz}$$

Now square that result:

$$(2.65 \times 10^{12})^2 \approx 7.02 \times 10^{24}$$

Finally, multiply by the mass $m$:

$$K \approx (7 \times 10^{-27}) \times (7.02 \times 10^{24})$$

$$K \approx 49 \times 10^{-3} \text{ N/m}$$

$$K \approx 4.9 \times 10^{-2} \text{ N/m}$$

**Final Answer:**

$$K = 4.93 \times 10^{-2} \text{ N/m}$$

---

### 5. Professor's Insight: What does this number mean?

The answer is **$0.049$ N/m**.

To give you some context:

-   The spring in a clicky pen has a constant of about $100$ N/m.
    
-   A typical chemical bond in a standard metal (like Copper) has a "spring constant" of about $10$ to $100$ N/m.
    

Our result ($0.049$ N/m) is **extremely small**. This means the bonds between these atoms are very, very weak.

**Why?** Look at the mass. $7 \times 10^{-27}$ kg is approximately the mass of a **Helium** atom. Helium interacts very weakly (Van der Waals forces). It is so weak that it usually doesn't even form a solid unless you cool it to near absolute zero and apply pressure. This problem is likely modeling a very soft, quantum crystal like solid Helium!

**Ready for the next step?**

We have counted the atoms ($N$) and measured the springs ($K$). Usually, the next step in these problems is to calculate the **Heat Capacity** or the **Total Energy**. Shall we move on?