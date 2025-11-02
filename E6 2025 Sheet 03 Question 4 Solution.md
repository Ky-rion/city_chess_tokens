

Here is a step-by-step description of how you would graphically demonstrate the invariance of Miller indices.

The core idea is to:

1.  Determine the Miller indices for the plane using the **original origin (O)**.
    
2.  Graphically **shift the origin** to a new, equivalent lattice point **(O')**.
    
3.  Determine the Miller indices for the **exact same plane** relative to this **new origin (O')**.
    
4.  Compare the results.
    

---

### 1. Determine Indices with the Original Origin (O)

First, we find the Miller indices for the blue plane shown in your image, using the origin $O = (0, 0, 0)$.

1.  **Find Intercepts:** We find where the plane crosses the $x$, $y$, and $z$ axes.
    
    -   **x-axis:** The plane is parallel to the x-axis, so it never crosses it. The intercept is at **$\infty$**.
        
    -   **y-axis:** The plane is also parallel to the y-axis. The intercept is at **$\infty$**.
        
    -   **z-axis:** The image shows the plane crosses the z-axis at **$\frac{2c}{3}$**.
        
2.  **Write Intercepts as Fractions:** We write these intercepts as fractions of the lattice parameters ($a, b, c$).
    
    -   $( \infty \cdot a, \infty \cdot b, \frac{2}{3} \cdot c )$
        
    -   The fractional intercepts are: $(\infty, \infty, \frac{2}{3})$
        
3.  **Take Reciprocals:** We take the reciprocal of each fractional intercept.
    
    -   $( \frac{1}{\infty}, \frac{1}{\infty}, \frac{1}{2/3} )$
        
    -   This gives: $(0, 0, \frac{3}{2})$
        
4.  **Clear Fractions:** We multiply by the smallest common denominator (in this case, 2) to get the smallest set of integers $(hkl)$.
    
    -   $2 \cdot (0, 0, \frac{3}{2}) = (0, 0, 3)$
        

So, relative to the original origin $O$, the plane belongs to the **$(003)$** family.

---

### 2. Shift the Origin (O')

Now, we graphically shift the origin to a new, equivalent lattice point. A simple choice is the corner at the top of the unit cell.

-   **New Origin O' = $(0, 0, c)$**
    

This means our new coordinate system ($x'$, $y'$, $z'$) is related to the old one ($x, y, z$) as follows:

-   $x' = x$
    
-   $y' = y$
    
-   $z' = z - c$
    

---

### 3. Determine Intercepts with the New Origin (O')

Next, we find the intercepts of the **exact same blue plane** on the **new axes** ($x'$, $y'$, $z'$).

1.  **Find Intercepts (New System):**
    
    -   **x'-axis:** The plane is still parallel to the $x'$-axis (since $x' = x$). The intercept is at **$\infty$**.
        
    -   **y'-axis:** The plane is still parallel to the $y'$-axis (since $y' = y$). The intercept is at **$\infty$**.
        
    -   z'-axis: The plane is at the old coordinate $z = \frac{2c}{3}$. To find the new $z'$ intercept, we convert:
        
        $z' = z - c = \frac{2c}{3} - c = -\frac{c}{3}$
        
        So, the new z-intercept is $-\frac{c}{3}$.
        
2.  **Write Intercepts as Fractions:**
    
    -   $(\infty \cdot a, \infty \cdot b, -\frac{1}{3} \cdot c)$
        
    -   The fractional intercepts are: $(\infty, \infty, -\frac{1}{3})$
        
3.  **Take Reciprocals:**
    
    -   $(\frac{1}{\infty}, \frac{1}{\infty}, \frac{1}{-1/3})$
        
    -   This gives: $(0, 0, -3)$
        
4.  **Clear Fractions:** The indices are already integers. We write a negative index with a bar over the number.
    
    -   $(0, 0, \bar{3})$
        

---

### 4. Conclusion

-   **Original Indices:** $(003)$
    
-   **New Indices (after shift):** $(00\bar{3})$
    

In crystallography, the **$(003)$** family and the **$(00\bar{3})$** family describe the **exact same set of planes**. They are perfectly parallel and have the same spacing ($d = c/3$), they just differ in the "direction" of the normal vector (one points up, one points down), which is an arbitrary choice.

By showing that a shift in the origin from one lattice point to another results in crystallographically equivalent indices, you have graphically demonstrated that the **Miller indices are independent of the choice of origin**.