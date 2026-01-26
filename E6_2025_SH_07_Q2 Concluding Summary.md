

Here is a condensed **Crystallography Cheat Sheet** based on the exercises we just covered. This is designed to be quick to read and easy to copy onto your formula sheet.

### **1. Miller Indices (Notation & Calculation)**

**The Notation "Code"**

-   **( h k l )** $\rightarrow$ **Specific Plane** (Round = Smooth surface).
    
-   **{ h k l }** $\rightarrow$ **Family of Planes** (Curly = Bag of all symmetric equivalents).
    
-   **[ h k l ]** $\rightarrow$ **Specific Direction** (Square = Sharp arrow/vector).
    

**Calculating Indices (h k l)**

1.  **Identify Intercepts:** Where does the plane cut axes $x, y, z$? (in units of lattice vectors $a, b, c$).
    
2.  **Invert:** Take the reciprocal ($1 / \text{intercept}$).
    
3.  **Reduce:** Multiply to get smallest whole numbers.
    

> **Key Rule:** If plane is **parallel** to an axis $\rightarrow$ Intercept = $\infty$ $\rightarrow$ Index = **0**.

---

### **2. Wigner-Seitz Cell (Real Space)**

-   **Definition:** The volume of space closest to _one_ specific atom.
    
-   **Construction Recipe:**
    
    1.  Draw lines to **nearest neighbors**.
        
    2.  Draw **perpendicular bisectors** (walls) at the midpoint of those lines.
        
    3.  The enclosed area is the cell.
        

---

### **3. Reciprocal Lattice (k-Space)**

-   **Conversion Formula:** How to turn real vectors ($\vec{a}$) into reciprocal vectors ($\vec{b}$):
    
    $$\vec{a_i} \cdot \vec{b_j} = 2\pi \delta_{ij}$$
    
    _(This means the dot product is $2\pi$ if directions match, and $0$ if they are perpendicular.)_
    
-   **For a Simple Square/Cubic Lattice:**
    
    If real spacing is $a$, reciprocal spacing is:
    
    $$b = \frac{2\pi}{a}$$
    
    _(Inverse relationship: Large real lattice = Tiny reciprocal lattice)._
    

---

### **4. Brillouin Zones (The Map of k-Space)**

-   **1st Brillouin Zone:**
    
    -   It is simply the **Wigner-Seitz Cell** of the **Reciprocal Lattice**.
        
    -   Constructed using **Nearest** neighbors in k-space.
        
-   **2nd Brillouin Zone:**
    
    -   Constructed using **Next-Nearest** neighbors (diagonals).
        
    -   It surrounds the 1st zone.
        
-   **Conservation of Area (The "Secret Rule"):**
    
    All Brillouin zones have the **same area/volume**.
    
    $$\text{Area}_{1} = \text{Area}_{2} = \text{Area}_{5} = \dots = \text{Area}_{N}$$
    
-   **Calculating Area (for Square Lattice):**
    
    $$A = |\vec{b_1}| \cdot |\vec{b_2}| = \left(\frac{2\pi}{a}\right)^2 = \frac{4\pi^2}{a^2}$$
    

---

**Next Step for you:**

You are now armed with a solid cheat sheet! Would you like me to generate a **practice quiz** with 3 short questions (one for each section above) to test if these formulas stick in your memory?