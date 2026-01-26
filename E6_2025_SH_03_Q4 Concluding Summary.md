

Here is a concise "Cheat Sheet" summary tailored for your exam preparation. This covers the specific mechanics and concepts we used to solve the problem, plus the standard conventions you need to memorize.

### 📝 Solid State Physics Cheat Sheet: Miller Indices

#### **1. The 3-Step Algorithm (How to find $hkl$)**

To determine the Miller Indices for any plane:

1.  **Find Intercepts:** Identify where the plane cuts the axes ($x, y, z$) in terms of unit vectors ($a, b, c$).
    
2.  **Take Reciprocals:** Divide 1 by each intercept value.
    
    $$h' = \frac{1}{x}, \quad k' = \frac{1}{y}, \quad l' = \frac{1}{z}$$
    
3.  **Reduce to Integers:** Multiply all three numbers by the smallest common number (LCM) to clear fractions.
    
    $$(hkl) = \text{Smallest whole numbers}$$
    

---

#### **2. Important Rules & Shortcuts**

-   **The "Parallel" Rule (Infinity):**
    
    If a plane is **parallel** to an axis, it never intersects it.
    
    -   Intercept = $\infty$
        
    -   Index = $\frac{1}{\infty} = 0$
        
    -   _Example:_ A plane parallel to the x-axis will always have $h=0$ (e.g., $(0kl)$).
        
-   **The "Origin Shift" Concept (from your exercise):**
    
    Miller indices represent a **family of infinite parallel planes**.
    
    -   Shifting the coordinate system origin to a new lattice point does **not** change the indices.
        
    -   Indices calculated from a plane cutting 1 unit cell are identical to indices calculated from a parallel plane cutting 3 unit cells.
        
-   **Negative Intercepts:**
    
    If a plane cuts an axis at a negative coordinate (e.g., $-1$), the index gets a bar over the number.
    
    -   Intercept: $-1 \rightarrow$ Index: $\bar{1}$ (Pronounced "bar one").
        

---

#### **3. Mathematical Relationships**

If you know the Miller Indices $(hkl)$, the plane intersects the axes at:

$$x_{intercept} \propto \frac{1}{h}, \quad y_{intercept} \propto \frac{1}{k}, \quad z_{intercept} \propto \frac{1}{l}$$

_From your specific problem:_

$$ \frac{h}{k} = \frac{y_{intercept}}{x_{intercept}} \quad \text{(Inverse relationship)}$$

_(Note: Since $h \propto 1/x$ and $k \propto 1/y$)_

---

#### **4. Notation Watch (Don't mix these up!)**

-   **( h k l )** : Parentheses = A specific **Plane**.
    
-   **[ u v w ]** : Square Brackets = A specific **Direction** (Vector).
    
-   **{ h k l }** : Curly Braces = A **Family** of planes (equivalent by symmetry, e.g., the faces of a cube).
    
-   **< u v w >** : Angle Brackets = A **Family** of directions.
    

---

### **How to verify your answer in an exam:**

If you aren't sure if your indices $(hkl)$ are correct, check the **ratio**.

-   In your exercise, the $y$-intercept was **3** times larger than the $z$-intercept ($3$ vs $1$).
    
-   Therefore, the $z$-index must be **3** times larger than the $y$-index ($3$ vs $1$).
    
-   _Inverse logic:_ **Big intercept = Small index. Small intercept = Big index.**
    

**Next Step:**

Would you like to try a quick "quiz" question? I can give you a set of intercepts, and you can try to calculate the Miller Indices using this cheat sheet to see if it sticks!