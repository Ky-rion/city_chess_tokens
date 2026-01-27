

![[Pasted image 20260126140454.png]]
![[Pasted image 20260126140502.png]]

Welcome back to class! You mastered the 1D wire; now we are going to graduate to a **3D Crystal**.

This might sound harder, but physically, it's just like standing in a square room. If you look straight at a wall, the distance is short. If you look into the corner of the room, the distance is longer. That simple geometric fact changes the physics completely!

Let's break down **Part (b)**.

---

### **1. The New Challenge: Anisotropy**

In 1D, there is only one direction (left/right). In 3D, the properties of the crystal depend on _which direction_ you travel. This is called **anisotropy**.

We are looking at a **Simple Cubic Lattice**.

-   **[100] Direction:** This is looking straight along one of the cube's edges (like looking directly at a wall).
    
-   **[111] Direction:** This is looking along the body diagonal (from one bottom corner to the opposite top corner).
    

The question asks us to compare the **Brillouin Zone boundaries** and **occupied states** for these two distinct directions.

---

### **2. The [100] Direction (Left Diagram)**

This direction is essentially the same as our 1D case.

-   **The Boundary:** The distance to the edge of the Brillouin Zone along the x-axis is exactly $k_{boundary} = \frac{\pi}{a}$.
    
-   **The Electrons:** Remember, our Fermi radius (the "water level" of electrons) is $k_F = 1.2 \frac{\pi}{a}$.
    
-   **The Comparison:**
    
    $$1.2 \frac{\pi}{a} > 1.0 \frac{\pi}{a}$$
    
    The electrons **overflow** the first zone boundary.
    

**Looking at the [100] Plot:**

-   It looks almost identical to the 1D plot you saw in Part (a).
    
-   **Band 1:** Completely full (black dots cover the whole curve).
    
-   **Band 2:** Partially full (the dots spill into the bottom of the second band).
    
-   **Physics:** In this direction, the electron gas behaves like a multivalent metal—it occupies multiple bands.
    

---

### **3. The [111] Direction (Right Diagram)**

This is where the 3D geometry kicks in. We are now looking along the diagonal.

-   **The Boundary:** The Brillouin Zone boundary is defined by the plane that bisects the reciprocal lattice vector.
    
    -   The vector to the nearest neighbor in reciprocal space along the diagonal is $\vec{G}_{111} = \frac{2\pi}{a}(1,1,1)$.
        
    -   The length of this vector is $\frac{2\pi}{a} \times \sqrt{1^2+1^2+1^2} = \frac{2\pi\sqrt{3}}{a}$.
        
    -   The zone boundary is halfway there:
        
        $$k_{boundary} = \frac{\pi\sqrt{3}}{a} \approx 1.73 \frac{\pi}{a}$$
        
    -   _Note:_ The boundary is much farther away because the diagonal of a cube is longer than its edge!
        
-   **The Comparison:**
    
    Now compare this new boundary to our Fermi radius:
    
    $$k_F = 1.2 \frac{\pi}{a}$$
    
    $$k_{boundary} \approx 1.73 \frac{\pi}{a}$$
    
    $$1.2 < 1.73$$
    
    **The "Aha!" Moment:** along this direction, the electron "water level" ($1.2$) does **not** reach the boundary ($1.73$).
    

**Looking at the [111] Plot:**

-   **Wider Zone:** Notice the x-axis goes much further out (to $\frac{\sqrt{3}\pi}{a}$) before the band folds back.
    
-   **Band 1:** The red dashed line ($E_F$) hits the curve _before_ it reaches the zone edge. The electrons are comfortably contained entirely within the first band.
    
-   **Band 2 & 3:** These are completely empty.
    

---

### **4. Summary of the Difference**

The solution diagram beautifully illustrates this contrast:

![[Pasted image 20260127180017.png]]

**What does this mean for the student?**

When you sketch this:

1.  **For [100]:** Draw the narrow zone boundaries. Make sure your Fermi energy line is high enough to cross into the second band.
    
2.  **For [111]:** Draw wide zone boundaries. Keep the **same** energy height for your Fermi line (energy is a scalar, it doesn't care about direction), but because the parabola is stretched out, the line will hit the curve _before_ the boundary.
    

You are doing great! This concept—that a Fermi surface might cross a zone boundary in one direction but not another—is exactly how we get complex Fermi surfaces (like "monster" shapes or "necks") in real metals like Copper.

Ready for the next part?