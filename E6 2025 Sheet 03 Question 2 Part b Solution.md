

![[Pasted image 20260125183133.png]]

Excellent work! You are moving through these concepts quickly. Let's tackle **Part b)**, which deals with visualizing the lattice and counting the planes.

This part is crucial because the **(110) plane** is the "superstar" of the **bcc** (body-centered cubic) structure. It is the plane most packed with atoms, which dictates how the material deforms (slips) under stress.

Here is the breakdown of the solution provided by the other professor.

---

### 1. Identifying the Structures

First, the question asks us to look at the graphic (from the previous image) and identify the structures.

-   **Left Image (BCC):** You see atoms at the 8 corners and **one single atom in the very center** of the cube. This is **Body-Centered Cubic (bcc)**.
    
-   **Right Image (FCC):** You see atoms at the corners and atoms in the middle of each face. This is **Face-Centered Cubic (fcc)**.
    

**Task:** We focus on the **left (bcc)** structure.

---

### 2. Drawing the (110) Plane

The question asks you to draw the **(110)** plane into the bcc structure.

**How to find it:**

Recall the rule for Miller Indices $(h k l)$: The plane intersects the axes at $\frac{1}{h}, \frac{1}{k}, \frac{1}{l}$.

-   $h = 1 \rightarrow$ Intercept at $x = 1$
    
-   $k = 1 \rightarrow$ Intercept at $y = 1$
    
-   $l = 0 \rightarrow$ Intercept at $z = \infty$ (Parallel to the z-axis)
    

**Drawing Instructions:**

1.  **Find the floor:** Look at the bottom square of the cube. Draw a line connecting $x=1$ (the front-right corner? Depends on your axis definition, usually the point at $a$ on the x-axis) to $y=1$ (the point at $a$ on the y-axis).
    
2.  **Extrude up:** Since the $z$-index is 0, the plane runs straight up, parallel to the walls.
    
3.  **The Result:** It looks like a diagonal rectangular sheet slicing through the cube.
    

**Professor's Insight:**

Why is this plane special in **bcc**?

The equation for this plane is $x + y = 1$.

The center atom in a bcc crystal is located at coordinate $(0.5, 0.5, 0.5)$.

If you plug that in: $0.5 + 0.5 = 1$.

**The plane slices perfectly through the center atom!**

---

### 3. Counting the Equivalent Planes (Multiplicity)

The solution states: **"There are 12 equivalent planes."**

This can be confusing because usually, we think of a front face and a back face as "parallel," so are they different? In crystallography (specifically for calculating Diffraction Multiplicity), we count the **unique normal vectors**. Basically, how many distinct directions can I look at this crystal and see the same atomic arrangement?

We calculate this by permuting (swapping) the positions of the numbers and changing their signs.

**The Family {110}:**

We have two "1"s and one "0".

-   **Step 1: Swap positions (3 variations)**
    
    The zero can be in the $z$, $y$, or $x$ position.
    
    $\{110\}, \{101\}, \{011\}$
    
-   **Step 2: Swap signs (4 variations per position)**
    
    For the pair $\{1,1\}$, we can have:
    
    $(++), (--), (+-), (-+)$
    
    _(Note: The zero has no sign, so we only flip the ones.)_
    

**Let's list them all (just like the solution text):**

**Group A: The Zero is in Z (vertical planes)**

1.  $(110)$
    
2.  $(\bar{1}\bar{1}0)$ $\rightarrow$ written as $(-1-10)$ in your text
    
3.  $(1\bar{1}0)$ $\rightarrow$ written as $(1-10)$
    
4.  $(\bar{1}10)$ $\rightarrow$ written as $(-110)$
    

**Group B: The Zero is in Y (diagonal slices through the sides)**

5. $(101)$

6. $(\bar{1}0\bar{1})$ $\rightarrow$ written as $(-10-1)$

7. $(10\bar{1})$ $\rightarrow$ written as $(10-1)$

8. $(\bar{1}01)$ $\rightarrow$ written as $(-101)$

**Group C: The Zero is in X (diagonal slices through the front/back)**

9. $(011)$

10. $(0\bar{1}\bar{1})$ $\rightarrow$ written as $(0-1-1)$

11. $(01\bar{1})$ $\rightarrow$ written as $(01-1)$

12. $(0\bar{1}1)$ $\rightarrow$ written as $(0-11)$

**Total:** $3 \text{ groups} \times 4 \text{ planes} = \mathbf{12}$ **equivalent planes.**

**Next Step:**

We have identified the planes and the family count. The next logical step in a solid-state course is usually calculating the **distance** between these planes ($d$-spacing) or determining the **packing density** on this specific plane. Would you like to try calculating the d-spacing for these planes next?