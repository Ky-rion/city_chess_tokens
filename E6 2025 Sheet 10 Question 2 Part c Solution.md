

![[Pasted image 20260126140519.png]]
![[Pasted image 20260126140532.png]]

Welcome to the most exciting part of Solid State Physics!

In parts (a) and (b), we assumed the electrons were "free"—gliding through the crystal like ghosts, completely ignoring the atoms. But in reality, crystals have positively charged atomic nuclei that attract the electrons.

Part (c) asks: **"What happens if we turn on a weak periodic potential?"** (i.e., the electrons now slightly "feel" the lattice).

This is the moment where the "Free Electron Model" evolves into the **"Nearly Free Electron Model,"** and it gives birth to the most important concept in modern electronics: **The Band Gap**.

Let's break down the solution provided in your image.

---

### **1. The "Forbidden Zone" (The Band Gap)**

The most dramatic change happens exactly at the **Brillouin Zone boundaries** (the vertical dashed lines at $k = \pm \pi/a$).

-   **In Part (a) (Free Electrons):** The energy curve was a continuous parabola. At the boundary, you could pass smoothly from the first zone to the second zone. The energy at $k = \pi/a$ was a single, specific value.
    
-   **In Part (c) (Weak Potential):** The text explains that the energy parabola "splits" (_aufspaltet_) at the boundaries.
    
    -   Instead of one energy value at the boundary, you now have **two**.
        
    -   One energy state is pushed down (lower energy).
        
    -   One energy state is pushed up (higher energy).
        
    -   **The Result:** A range of energies between these two points where **no electron states exist**. This is the shaded gap in "Abbildung 3" labeled "forbidden zones" (_verbotene Zonen_).
        

**Why does this happen? (Physics Deep Dive)**

When an electron wave has a wavelength that matches the lattice spacing (which happens at $k = \pi/a$), it undergoes **Bragg Reflection**. The wave bounces back and forth, creating a **standing wave**.

-   One standing wave accumulates electron probability **on top** of the positive ions (Low Energy).
    
-   The other standing wave accumulates probability **in between** the ions (High Energy).
    
-   The energy difference between sitting "on the ions" vs "between the ions" is exactly the energy gap ($E_g$).
    

---

### **2. The "Bending" of the Curve**

The second major change is the shape of the curve itself near the boundaries.

-   **The Rule:** The text states that surfaces of constant energy must "intersect the boundaries of the Brillouin zones at right angles" (_rechtwinklig schneiden_).
    
-   **What this looks like:** Look closely at the black dots in "Abbildung 3".
    
    -   In the free electron case (Part a), the parabola hit the boundary at a slant.
        
    -   In this case (Part c), the curve **flattens out** as it touches the dashed line. It becomes horizontal.
        

**Why does it flatten?**

The slope of the energy curve ($\frac{dE}{dk}$) represents the **Group Velocity** (the speed) of the electron. At the zone boundary, we have a standing wave. Standing waves don't go anywhere! Their velocity is zero. Therefore, the slope of the graph must be zero (flat) at the boundary.

---

### **3. Summary of Changes (The "Takeaway")**

If you are asked to redraw the diagram from Part (a) with a "weak periodic potential," here is your checklist:

1.  **Draw the Gap:** At the vertical lines ($k = \pm \pi/a$), erase the point where the bands meet. Draw one point lower and one point higher. There should be a vertical empty space between them.
    
2.  **Flatten the Tips:** Modify the parabola so it curves to become horizontal just before it hits the gap. It should look like an "S" shape bending into the boundary.
    
3.  **Distort the Fermi Surface:** Because the energy curve is now bent, the Fermi surface (the shape of the "water" filling the bucket) is no longer a perfect sphere. As the text mentions, the "sharp tips" get rounded off.
    

This transition from "free" to "gapped" is what distinguishes metals from semiconductors and insulators. You have just derived the fundamental principle of the transistor!

**Would you like me to summarize the entire problem (a, b, and c) into a single "cheat sheet" for your exam study?**