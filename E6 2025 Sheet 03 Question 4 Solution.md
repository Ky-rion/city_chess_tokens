

![[Pasted image 20260125183521.png]]
![[Pasted image 20260125183532.png]]

Hello! It is a pleasure to meet you. I would be delighted to step in as your solid-state physics professor today. Don't worry if this looks like a jumble of geometry at first glance—visualizing crystal planes is a skill that takes a little practice, but once you "see" it, it becomes very intuitive.

We are going to walk through the solution provided by the other professor (Image 2) to answer the problem posed in Image 1.

### **The Core Concept: Miller Indices**

First, a quick definition. **Miller Indices** (denoted as $h, k, l$) are three numbers used to describe the orientation of a flat plane slicing through a crystal lattice.

The "Golden Rule" of Miller Indices is that they describe a **family of parallel planes**, not just one single plane. Whether a plane passes through the first unit cell or the hundredth unit cell, if they are parallel, they have the exact same Miller Indices.

This problem asks us to prove exactly that: **Shifting the origin (or moving to a parallel plane) does not change the indices.**

---

### **Step 1: Visualizing the "Blue Plane" (The Extended View)**

Let's look at the second image you uploaded. The professor has drawn **three** unit cells side-by-side along the y-axis.

**Why did he do that?**

In the original problem (Image 1), the blue plane has a very shallow slope. It doesn't cut the axes at "nice" integer numbers inside the first box. To make the math easy, the professor extended the plane until it hit a clear corner.

Look at the **Blue Plane** in Image 2:

1.  **Z-axis intercept:** It starts at the very top of the Z-axis (height = 1).
    
2.  **Y-axis intercept:** It slopes down and to the right, crossing through three whole boxes before hitting the ground (height = 0) at the end of the third box.
    
3.  **X-axis intercept:** The plane runs parallel to the X-axis (it never cuts it), so the intercept is at infinity ($\infty$).
    

#### **Calculation A: The Blue Plane**

Let's calculate the indices based on this large, extended plane.

1.  **Identify Intercepts:**
    
    -   $x = \infty$ (Parallel to x)
        
    -   $y = 3$ (It crosses 3 unit lengths along y)
        
    -   $z = 1$ (It crosses 1 unit length along z)
        
2.  **Take Reciprocals (1 divided by the number):**
    
    -   $h = 1 / \infty = 0$
        
    -   $k = 1 / 3$
        
    -   $l = 1 / 1 = 1$
        
3.  **Reduce to Integers (Clear fractions):**
    
    We have $(0, 1/3, 1)$. To get whole numbers (Miller indices must be integers), we multiply everything by the lowest common denominator, which is **3**.
    
    -   $0 \times 3 = 0$
        
    -   $(1/3) \times 3 = 1$
        
    -   $1 \times 3 = 3$
        

**Result:** The Miller Indices are **(013)**.

---

### **Step 2: Visualizing the "Green Plane" (The Shifted View)**

Now, let's look at the small **Green Plane** in the first unit cell of Image 2.

This green plane is parallel to the blue one. Think of it as the "little sister" of the blue plane that lives entirely inside the first unit cell. This represents what happens if we shift our perspective (or the origin) to look at the plane nearest to us.

Where does this green plane cut the axes?

1.  **Y-axis intercept:** It cuts the y-axis at the edge of the first box ($y = 1$).
    
2.  **Z-axis intercept:** Look closely at the slope. If the big blue plane drops 1 unit of height over 3 units of length, then over **1** unit of length, it only drops **1/3** of height. So, the green plane cuts the z-axis at $1/3$.
    
    _(Note: This is mathematically consistent with the label "2c/3" in your first image. The blue plane at $y=1$ has dropped 1/3, leaving 2/3 remaining height)._
    

#### **Calculation B: The Green Plane**

Let's calculate the indices for this smaller plane.

1.  **Identify Intercepts:**
    
    -   $x = \infty$
        
    -   $y = 1$
        
    -   $z = 1/3$
        
2.  **Take Reciprocals:**
    
    -   $h = 1 / \infty = 0$
        
    -   $k = 1 / 1 = 1$
        
    -   $l = 1 / (1/3) = 3$
        
3.  **Reduce to Integers:**
    
    We have $(0, 1, 3)$. These are already integers! We don't need to multiply by anything.
    

**Result:** The Miller Indices are **(013)**.

---

### **The Conclusion (The "Proof")**

This is the "Aha!" moment the professor wants you to see.

-   When we calculated the indices for the giant **Blue Plane** (Intercepts: $3, 1$), we got **(013)**.
    
-   When we calculated the indices for the shifted **Green Plane** (Intercepts: $1, 1/3$), we also got **(013)**.
    

**Professor's Explanation Translation:**

> "Since the green plane can be shifted... and is congruent to the blue plane, we have shown that the displacement of the origin has no influence on the Miller Indices in a fixed crystal system."

In plain English: Because the lattice repeats periodically, measuring the slope of the plane over 1 unit cell gives you the exact same result as measuring it over 3 unit cells. The Miller Indices describe the **orientation** (the slope), which is constant for both.

### **Summary Checklist for your understanding:**

-   **Reciprocals are key:** We always take $1/intercept$. This is why a large intercept (like 3) becomes a small index, and a fractional intercept (like 1/3) becomes a large index.
    
-   **Infinity becomes Zero:** Any plane parallel to an axis has an index of 0 for that axis.
    
-   **Origin Shifts don't matter:** You can pick any parallel plane in the stack; the math will always simplify to the same $(hkl)$ integers.
    

Would you like me to give you a practice problem with a different plane (e.g., one that cuts x and y but is parallel to z) to test this out?