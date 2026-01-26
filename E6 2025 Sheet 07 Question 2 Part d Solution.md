

![[Pasted image 20260125185546.png]]

We have arrived at one of the most important concepts in all of Solid State Physics: The **Brillouin Zone**.

If the Wigner-Seitz cell is "Personal Space" in the real world (where atoms live), the Brillouin Zone is "Personal Space" in the **Reciprocal World** (where waves and electron momentums live).

This part of the question asks us to construct the **1st** and **2nd** Brillouin Zones.

---

### Step 1: Switch Universes (Real Space $\rightarrow$ Reciprocal Space)

Before we can draw anything, we have to translate our map. We currently have "Real Lattice VECTORS" ($\vec{a}$), but Brillouin Zones live on a map made of "Reciprocal Lattice VECTORS" ($\vec{b}$).

Your professor's solution gives the formula to translate between them:

$$\vec{a_i} \cdot \vec{b_j} = 2\pi \delta_{ij}$$

**In plain English:**

1.  **Direction:** For a simple square grid, the reciprocal vectors point in the same direction as the real ones ($x \rightarrow k_x$, $y \rightarrow k_y$).
    
2.  **Length:** The length is inverted. If the real atoms are far apart ($a$ is big), the reciprocal points are close together ($2\pi/a$ is small), and vice-versa.
    

**Calculation:**

-   Real vector $\vec{a_1} = (a, 0)$ $\rightarrow$ Reciprocal vector $\vec{b_1} = (\frac{2\pi}{a}, 0)$
    
-   Real vector $\vec{a_2} = (0, a)$ $\rightarrow$ Reciprocal vector $\vec{b_2} = (0, \frac{2\pi}{a})$
    

**The New Map:**

Instead of a grid of dots separated by distance **$a$**, we now have a grid of dots separated by distance **$2\pi/a$**.

---

### Step 2: Construct the 1st Brillouin Zone (The Blue Square)

The rule for the **1st Brillouin Zone** is simple: **It is just the Wigner-Seitz cell of the Reciprocal Lattice.**

We do exactly what we did in part (c), but on our new map:

1.  **Center:** Start at the origin $(0,0)$ in k-space (called the $\Gamma$ point).
    
2.  **Neighbors:** Identify the 4 nearest neighbors (Up, Down, Left, Right).
    
3.  **Bisect:** Draw walls halfway between the center and these neighbors.
    
    -   The distance to a neighbor is $2\pi/a$.
        
    -   The wall is at half that distance: $\pi/a$.
        

**Result:** You get a square centered at the origin with boundaries at $k_x = \pm \pi/a$ and $k_y = \pm \pi/a$.

-   This is the **Blue Square** in the solution image.
    

---

### Step 3: Construct the 2nd Brillouin Zone (The Orange Diamonds)

Now things get interesting. The 2nd Brillouin Zone is the "next layer" of territory.

**The Recipe:**

1.  **Next-Nearest Neighbors:** Look at the lattice points that are next-closest. In a square grid, these are the **diagonal** dots (at the 4 corners).
    
2.  **Bisect:** Draw perpendicular walls halfway to these diagonal neighbors.
    
3.  **The Shape:** These new diagonal walls cut off the corners of the space, forming a larger diamond shape.
    

**Defining the Zone:**

The "2nd Brillouin Zone" is NOT the whole diamond. It is **only the new area** we just added.

-   **1st Zone:** The area closest to the origin (0 Bragg reflections).
    
-   **2nd Zone:** The area that is 2nd closest to the origin.
    

**Visualizing the Solution Image:**

-   The **Orange Lines** in the solution represent the walls drawn for the diagonal neighbors.
    
-   The **2nd Brillouin Zone** consists of the 4 triangles that stick out from the blue square to form the larger diamond.
    
-   Mathematically, it is the area of the Diamond **minus** the area of the Blue Square.
    

---

### Summary Checklist

![[Pasted image 20260126212231.png]]

> **Professor's Tip:** Why do we number them? If an electron increases its momentum (moves out from the center), it starts in the 1st zone. When it crosses the boundary (the blue line), it gets diffracted by the crystal lattice. Crossing that line puts it into the 2nd zone. These boundaries are where band gaps open up in semiconductors!

---

**Next Step for you:**

We have covered Miller Indices, Wigner-Seitz cells, and Brillouin Zones. These are the three pillars of crystal geometry.

Would you like to try a quick "final exam" question? I can give you a different lattice shape (like a rectangle where $a$ is twice as big as $b$) and ask you how the 1st Brillouin Zone would change shape compared to the square one we just did. (Hint: Remember the inverse relationship!)