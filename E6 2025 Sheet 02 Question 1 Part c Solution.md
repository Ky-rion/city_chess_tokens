

![[Pasted image 20260125182155.png]]
![[Pasted image 20260125182204.png]]

Welcome to the next level! We have defined the **Lattice** and the **Basis**. Now we need to define the "Box."

In solid-state physics, we hate dealing with infinity. We don't want to describe an infinite number of atoms. We want to describe just *one small box* that, if we repeat it over and over, creates the whole universe (or at least the whole crystal).

This box is called the **Unit Cell**. But specifically, **Question 1c** asks for the **Primitive Unit Cell** ("Primitive Gitterzelle").

***

### Step 1: The Definition (Translating the Solution)

**The Solution Text:**
> *"Primitive Gitterzelle enthält einen Punkt. Abbildung links mit ein-atomiger Basis, Beispiel rechts mit zwei-atomiger Basis. Muss durch Gittertranslation mit enthaltener Basis die Kristallstruktur wiedergeben."*

**The Professor's Translation & Breakdown:**
1.  **"Primitive lattice cell contains one point."**
    This is the mathematical definition. A **Primitive** cell is the smallest possible area (in 2D) or volume (in 3D) that can build the crystal. It contains exactly **1 Lattice Point**.
2.  **"Must reproduce the crystal structure..."**
    If you take this cell and shift it (translate it) by the lattice vectors, you must perfectly cover the entire plane without gaps or overlaps.

***

### Step 2: How to Count "One Point"
You might look at the solution boxes and say, "Wait, Professor! The box on the left connects *four* red atoms. How is that *one* point?"

This is the **Corner Rule**:
*   If an atom sits on the corner of a square/parallelogram, it is shared by 4 neighboring boxes.
*   Therefore, it only "belongs" $1/4$ to the box we are looking at.
*   Math: **4 Corners $\times$ ($1/4$ atom per corner) = 1 Atom total.**

So, a box drawn connecting 4 lattice points is mathematically considered to contain **1 Lattice Point**.

---

### Step 3: Analyzing the Left Image (Simple Case)
**Scenario:** A Lattice with a **1-atom Basis** (simple red dots).
*   **Lattice Point = Atom.**
*   The solution shows three different black outlines (parallelograms).
*   **Why are they all correct?**
    *   They all connect 4 neighboring atoms.
    *   They all enclose the exact same area.
    *   If you repeated any *one* of these shapes, you would tile the whole floor perfectly.
*   **Takeaway:** There is no "single" correct way to draw a primitive cell. As long as it is the smallest possible tile, it is correct.

---

### Step 4: Analyzing the Right Image (The "Graphene" Trap)
**Scenario:** The Honeycomb Structure (like Graphene).
**This is tricky!** Many students try to draw a hexagon. **A hexagon is NOT a primitive cell.** Why? Because a hexagon contains 6 corners and a middle... it has too many atoms. It is not the *smallest* possible unit.

Recalling Part (b), we know this structure has a **2-atom Basis** (Green + Red).
*   **The Rule:** The Primitive Cell must contain **1 Lattice Point**.
*   **The Fact:** Since 1 Lattice Point = 1 Green + 1 Red (the pair), our Primitive Cell must physically contain **1 Green and 1 Red atom**.

**Look at the black boxes in the solution:**
1.  **The Box on the atoms:** It connects four Green atoms.
    *   Corners: 4 Green atoms $\times$ $1/4$ = **1 Green Atom**.
    *   Inside: The box encloses exactly **1 Red Atom** completely.
    *   Total: 1 Green + 1 Red. Perfect! This is a primitive cell.
2.  **The Box in the empty space:** It connects the empty centers of the hexagons.
    *   Inside this box, you will find exactly one Green atom and one Red atom floating in the middle.
    *   Total: 1 Green + 1 Red. Also perfect!

### Summary for the Exam
When asked to mark a **Primitive Unit Cell**:

1.  **Connect the Dots:** Draw a parallelogram that connects nearest-neighbor lattice points (dots of the *same* color/type).
2.  **Check the "1 Point" Rule:** Does your shape represent exactly one lattice point? (Usually 4 corners $\times$ $1/4$).
3.  **Check the Basis:** If the crystal has a 2-atom basis (like the right image), ensure your box captures that specific pair (e.g., one green, one red).

You are doing great. You now understand the geometry of crystals better than most chemistry students! Any questions on this part?