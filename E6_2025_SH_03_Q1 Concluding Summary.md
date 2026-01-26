

Here is a condensed "Solid State Cheat Sheet" based on the problems we just solved. This is perfect for a quick review before an exam.

### 📄 Solid State Physics Cheat Sheet: Crystal Planes

#### 1. The Golden Rule of Miller Indices

Indices $(h \ k \ l)$ are the **reciprocals** of the axis intercepts.

-   **Indices $\to$ Drawing:**
    
    1.  Invert the numbers: $x = 1/h$, $y = 1/k$, $z = 1/l$.
        
    2.  Mark these points on the axes (in terms of lattice constant $a$).
        
    3.  Connect the dots.
        
-   **Drawing $\to$ Indices:**
    
    1.  Find where the plane cuts the axes (the intercepts).
        
    2.  Invert the intercepts ($1 / \text{intercept}$).
        
    3.  Clear fractions (multiply by a common factor to get integers).
        

> **Key Trick:** If a plane is parallel to an axis (never touches it), the intercept is $\infty$. The index is $\frac{1}{\infty} = \mathbf{0}$.

---

#### 2. Equivalent Planes (Symmetry)

In a cubic system, planes are physically "equivalent" if they look the same after rotating the cube.

-   **Notation:** Curly brackets $\{h k l\}$ represent the whole family of equivalent planes.
    
-   **How to generate them:**
    
    1.  **Permute:** Swap the order of numbers (e.g., $(100) \to (010)$).
        
    2.  **Change Signs:** Make positive numbers negative or vice versa (e.g., $(111) \to (\bar{1}11)$).
        
    
    -   _Note:_ A bar over a number ($\bar{1}$) means $-1$.
        

> **Exam Trap:** $(111)$ and $(222)$ are **NOT** equivalent. They are parallel, but $(222)$ has half the interplanar spacing. Never reduce Miller indices like fractions unless specifically asked for direction vectors.

---

#### 3. Interplanar Spacing Formula ($d_{hkl}$)

Calculates the perpendicular distance between parallel planes in a **cubic** lattice.

**The Formula:**

$$d_{hkl} = \frac{a}{\sqrt{h^2 + k^2 + l^2}}$$

**Alternative Form (Squared):**

$$\frac{1}{d^2_{hkl}} = \frac{h^2 + k^2 + l^2}{a^2}$$

_(Use this if it makes the algebra easier, as seen in your professor's solution)._

-   $a$ = Lattice constant (edge length of the cube).
    
-   $h, k, l$ = Miller indices.
    

---

#### 4. Units & Constants

-   **Å (Angstrom):** $1 \text{ \AA} = 10^{-10} \text{ m}$.
    
-   Commonly used for lattice constants (e.g., $a = 6 \text{ \AA}$).
    

---

#### Quick visual check (The "Triangle" Types)

-   **(1 0 0):** A flat wall (face of the cube).
    
-   **(1 1 0):** A rectangular sheet cutting diagonally through the cube (like a wall divider).
    
-   **(1 1 1):** A triangle connecting three corners.
    

Good luck with your studies! You now have a solid foundation for Chapter 1. Would you like me to quiz you on any of these to make sure it sticks?