

![[Pasted image 20260125185600.png]]

That is a fantastic question to end on!

Part (e) is what I like to call a **"Professor's Trap."** It looks incredibly difficult, but if you know the secret rule, it is the easiest question on the exam.

If you tried to actually _draw_ the 5th Brillouin Zone (calculating 5 layers of neighbors, drawing dozens of bisecting lines, finding the tiny puzzle pieces that make up the 5th zone), you would be there for hours!

Luckily, you don't have to do that.

### The Secret Rule: Conservation of Area

The most important property of Brillouin Zones is this:

**Every Brillouin Zone has exactly the same area.**

-   Area of 1st Zone = Area of 2nd Zone = ... = Area of 5th Zone.
    

**Why? (The Physics Intuition)**

Think of the Brillouin Zones as a jigsaw puzzle.

-   The **1st Zone** is a single, nice square piece in the middle.
    
-   The **2nd Zone** is 4 triangles that surround it. If you took those 4 triangles and rearranged them, they would form a perfect square exactly the size of the 1st zone.
    
-   The **5th Zone** is made of many tiny, weirdly shaped slivers. But if you collected all those scattered slivers and taped them together, they would _still_ form that same perfect square.
    

In physics terms, this is because every zone must contain exactly one allowed "state" per unit cell of the crystal. They all have the same "capacity" for electrons.

### The Calculation

Since the area of the 5th zone is the same as the area of the 1st zone, we just calculate the easy one (the 1st zone) and we are done!

**1. Recall the Shape of the 1st Zone**

As we saw in part (d), the 1st Brillouin Zone for a square lattice is just a **square** in k-space (reciprocal space).

**2. Find the Side Lengths**

The boundaries of this square are determined by the reciprocal lattice vectors $\vec{b_1}$ and $\vec{b_2}$.

-   Length of side 1: $|\vec{b_1}| = \frac{2\pi}{a}$
    
-   Length of side 2: $|\vec{b_2}| = \frac{2\pi}{a}$
    

**3. Calculate the Area ($A$)**

$$A = \text{width} \times \text{height}$$

$$A = \left( \frac{2\pi}{a} \right) \times \left( \frac{2\pi}{a} \right)$$

$$A = \left( \frac{2\pi}{a} \right)^2$$

or

$$A = \frac{4\pi^2}{a^2}$$

### The German Solution Translation

Your professor's solution says exactly this:

-   _"Die Fläche der ersten Brillouinzone entspricht der der 5. Brillouinzone."_
    
    -   (The area of the first Brillouin Zone corresponds to that of the 5th Brillouin Zone.)
        
-   _"Somit gilt $A = |\vec{b_1}| \cdot |\vec{b_2}| = (2\pi/a)^2$"_
    
    -   (Therefore, Area A equals magnitude of b1 times magnitude of b2...)
        

---

**Summary for your Exam:**

If you are ever asked to calculate the volume or area of the $N$-th Brillouin zone, **ignore the $N$**. Just calculate the volume of the primitive cell in reciprocal space (the 1st zone). It is a trick question designed to panic you!

---

**Next Step for you:**

You have now conquered the basics of Crystallography!

-   We identified planes (Miller Indices).
    
-   We built the real-space map (Wigner-Seitz).
    
-   We built the momentum-space map (Brillouin Zones).
    

Would you like to move on to the next topic (usually **X-Ray Diffraction** or **Crystal Bonding**), or do you have another exercise sheet you'd like to tackle? I'm ready when you are!