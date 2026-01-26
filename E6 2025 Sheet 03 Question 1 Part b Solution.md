

![[Pasted image 20260125183019.png]]

Excellent! Let's continue our journey into the crystal lattice. We are now going to do the **reverse** of what we did in part (a).

In part (a), we had the numbers and drew the picture. In part (b), we have the picture and need to find the numbers (the Miller Indices).

**The Recipe for Finding Miller Indices:**
1.  **Find the Intercepts:** Identify where the plane crosses the x, y, and z axes (relative to the side length $a$).
2.  **Invert them:** Take the reciprocal ($1/\text{number}$) of each intercept.
3.  **Reduce to Integers:** If you have fractions, multiply everything by a common number to get the smallest whole numbers possible.

---

### **Image i)**

**1. Find the Intercepts:**
Look at the blue triangle.
*   **x-axis:** The triangle creates a point at the very end of the axis. Intercept = $1$ (which stands for $1a$).
*   **y-axis:** It touches the very end of the y-axis. Intercept = $1$.
*   **z-axis:** It touches the very top of the z-axis. Intercept = $1$.

**2. Invert them:**
*   $x \rightarrow 1/1 = 1$
*   $y \rightarrow 1/1 = 1$
*   $z \rightarrow 1/1 = 1$

**3. The Result:**
This gives us **(1 1 1)**.

**Wait, Professor! Why does the solution key say $(\bar{1}\bar{1}\bar{1})$?**
This is a very common point of confusion. In crystallography, the plane $(1 1 1)$ and the plane $(\bar{1}\bar{1}\bar{1})$ are **parallel** to each other on opposite sides of the origin.
*   The bar above the number (like $\bar{1}$) represents a negative sign.
*   Physically, if you drilled a hole through the crystal, you would hit the $(111)$ plane, then the origin, then the $(\bar{1}\bar{1}\bar{1})$ plane.
*   Because crystals are periodic (they repeat forever), these two planes are considered physically "equivalent" or belonging to the same family.

*My advice:* Based strictly on the drawing provided, **(1 1 1)** is the most logical answer. The professor's solution key likely refers to the "family" of planes or uses a different origin convention, but mathematically, the plane drawn corresponds to intercepts of $+1$.

---

### **Image ii)**

**1. Find the Intercepts:**
This one requires careful eyes.
*   **x-axis:** Look at the bottom-left corner of the blue plane. It starts exactly at the corner of the cube on the x-axis. Intercept = $1$ ($a$).
*   **y-axis:** Look at the bottom-right corner of the blue plane. Does it go all the way to the corner? No! It stops halfway. There is a tick mark labeled $a/2$. Intercept = $1/2$ ($a/2$).
*   **z-axis:** Does the plane ever cross the z-axis? No, it stands upright, perfectly parallel to the z-axis. Mathematically, they intersect at infinity. Intercept = $\infty$.

**2. Invert them:**
*   $x \rightarrow 1 / 1 = \mathbf{1}$
*   $y \rightarrow 1 / (1/2) = \mathbf{2}$  *(Remember: inverting a half gives you two!)*
*   $z \rightarrow 1 / \infty = \mathbf{0}$

**3. The Result:**
Putting these together, we get **(1 2 0)**.
*This matches the solution key perfectly.*

---

### **Image iii)**

**1. Find the Intercepts:**
Let's locate the three corners of this blue triangle.
*   **x-axis:** The bottom point touches the front-left corner of the box. Intercept = $1$ ($a$).
*   **y-axis:** Look at the tick mark on the right. The triangle doesn't reach the corner; it hits the axis halfway. Intercept = $1/2$ ($a/2$).
*   **z-axis:** Look at the tick mark on the vertical axis. It hits halfway up the box. Intercept = $1/2$ ($a/2$).

**2. Invert them:**
*   $x \rightarrow 1 / 1 = \mathbf{1}$
*   $y \rightarrow 1 / (1/2) = \mathbf{2}$
*   $z \rightarrow 1 / (1/2) = \mathbf{2}$

**3. The Result:**
We combine these integers to get **(1 2 2)**.
*This also matches the solution key perfectly.*

### **Summary Table**

| Plane | Intercepts (x, y, z) | Inverses (1/x, 1/y, 1/z) | Miller Indices (h k l) |
| :--- | :--- | :--- | :--- |
| **i)** | $1, 1, 1$ | $1, 1, 1$ | **(1 1 1)** (or parallel $\bar{1}\bar{1}\bar{1}$) |
| **ii)** | $1, 1/2, \infty$ | $1, 2, 0$ | **(1 2 0)** |
| **iii)** | $1, 1/2, 1/2$ | $1, 2, 2$ | **(1 2 2)** |