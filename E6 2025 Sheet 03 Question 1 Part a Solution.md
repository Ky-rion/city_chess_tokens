

![[Pasted image 20260125183004.png]]

Hello! Welcome to the world of Solid State Physics. I am delighted to have you in my class. Don't worry if this looks like abstract geometry at first glance; Crystallography is actually very logical once you know the "secret code."

We are looking at **Miller Indices**, which are a notation system used to describe planes of atoms within a crystal lattice.

Let's break down the solution for **Part a): Drawing the (221) plane.**

### The "Secret Code" of Miller Indices

The notation given in the problem is **(2 2 1)**.
In generic terms, we call these numbers **(h k l)**.

*   $h = 2$ corresponds to the **x-axis**.
*   $k = 2$ corresponds to the **y-axis**.
*   $l = 1$ corresponds to the **z-axis**.

The most common mistake beginners make is thinking that a "2" means the plane crosses the axis at 2 units. **It is actually the opposite!**

Miller indices are defined by the **reciprocal** (the inverse) of the intercepts.

### The Algorithm: How to find the Intecepts

To draw the plane, we need to find where it cuts through the $x$, $y$, and $z$ axes of our cube. Let's assume the side length of our cubic unit cell is called **$a$**.

Here is the 3-step recipe:

1.  **Take the Miller Indices:** $(2, 2, 1)$
2.  **Take the Reciprocal (flip them):**
    *   $x \rightarrow 1/2$
    *   $y \rightarrow 1/2$
    *   $z \rightarrow 1/1$
3.  **Multiply by the lattice constant ($a$):**
    *   **x-intercept** $= \frac{1}{2} \cdot a = \mathbf{a/2}$
    *   **y-intercept** $= \frac{1}{2} \cdot a = \mathbf{a/2}$
    *   **z-intercept** $= 1 \cdot a = \mathbf{a}$

### Analyzing the Professor's Solution Image

Now, let's look at the diagram provided by your other professor. It perfectly visualizes the math we just did.

1.  **The Coordinate System:** Look at the origin (where $x, y, z$ meet in the bottom back corner).
2.  **The X-Axis (Bottom Left):**
    *   The plane needs to cut the x-axis at $a/2$.
    *   Look at the image: You can see a tick mark labeled **$a/2$**. The blue triangle's corner sits exactly halfway along the bottom-left edge of the cube.
3.  **The Y-Axis (Bottom Right):**
    *   The plane needs to cut the y-axis at $a/2$.
    *   Look at the image: There is a tick mark labeled **$a/2$**. The second corner of the blue triangle sits exactly halfway along the bottom-right edge.
4.  **The Z-Axis (Top Vertical):**
    *   The plane needs to cut the z-axis at $1a$ (or just $a$).
    *   Since the cube itself has a height of $a$, an intercept of $a$ means the plane must touch the very top corner of the box.
    *   Look at the image: The top point of the blue triangle goes all the way to the top corner of the unit cell on the z-axis.

### Summary
To draw the **(221)** plane:
1.  Make a dot halfway along the x-axis ($a/2$).
2.  Make a dot halfway along the y-axis ($a/2$).
3.  Make a dot at the full length of the z-axis ($a$).
4.  Connect these three dots to form a triangle.

And there you have it! That blue triangle represents a slice of the (221) plane cutting through the unit cell.

Ready for the next part?