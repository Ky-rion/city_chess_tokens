

![[Pasted image 20260125183804.png]]
![[Pasted image 20260125183826.png]]
![[Pasted image 20260125183847.png]]

Welcome back to class! I am so glad you asked for the continuation. This part is where the "detective work" really gets interesting.

In Part (a), we identified the "fingerprints" (the Miller indices: 110, 200, 211, etc.).

In Part (b), we are going to use a powerful tool called the **Structure Factor** to determine _why_ we see those specific fingerprints and not others. This will tell us if our crystal cube is **Simple Cubic (sc)**, **Face-Centered Cubic (fcc)**, or **Body-Centered Cubic (bcc)**.

The other professor's notes (images 2 and 3) walk through this process of elimination. Let's break down exactly what he did.

---

### The Concept: What is the Structure Factor ($S_G$)?

Think of the "Structure Factor" as a volume knob for diffraction peaks.

-   When X-rays hit atoms in a unit cell, the waves scatter.
    
-   Sometimes these waves arrive in sync and add up (Loud volume = **Peak visible**).
    
-   Sometimes they arrive out of sync and cancel each other out (Zero volume = **Extinction** / Peak missing).
    

The formula for the Structure Factor depends on the position of every atom $(x, y, z)$ in the unit cell:

$$S_{hkl} = \sum_{j} f \cdot e^{2\pi i (h x_j + k y_j + l z_j)}$$

-   $f$: Atomic scattering factor (how strongly one atom scatters).
    
-   $h, k, l$: The Miller indices we are testing.
    
-   $x_j, y_j, z_j$: The coordinates of the atoms in the cell.
    

Let's test our three suspects.

---

### Suspect 1: Simple Cubic (sc)

**The Setup:**

In a simple cubic lattice, there is effectively only **1 atom** per unit cell, located at the origin $(0,0,0)$.

**The Math (from Image 2):**

We plug the position $(0,0,0)$ into our formula:

$$S_{sc} = f \cdot e^{2\pi i (h\cdot 0 + k\cdot 0 + l\cdot 0)} = f \cdot e^0$$

Since $e^0 = 1$, we get:

$$S_{sc} = f$$

**The Rule:**

The result is just $f$. It is _never_ zero.

This means **ALL reflections are allowed.** Every possible integer combination of $(hkl)$ should produce a peak: (100), (110), (111), (200), etc.

**The Verdict:**

Look at our list from Part (a): We found (110), (200), (211)...

But where is **(100)**?

If this were Simple Cubic, the (100) peak would be the very first huge spike. It is missing from our graph.

-   **Conclusion:** It is **NOT** Simple Cubic because we are missing expected peaks.
    

---

### Suspect 2: Face-Centered Cubic (fcc)

**The Setup:**

The FCC lattice is crowded. It has **4 atoms** in the unit cell at these coordinates:

1.  $(0, 0, 0)$
    
2.  $(\frac{1}{2}, \frac{1}{2}, 0)$
    
3.  $(\frac{1}{2}, 0, \frac{1}{2})$
    
4.  $(0, \frac{1}{2}, \frac{1}{2})$
    

**The Math (from Image 3):**

The professor sums up the waves from all 4 atoms. It looks messy, but using Euler's identity ($e^{i\pi} = -1$), it simplifies to a beautiful condition (Equation 11 in the image):

$$S_{fcc} = f \left( 1 + (-1)^{k+l} + (-1)^{h+l} + (-1)^{h+k} \right)$$

**The Rule:**

For $S$ to be non-zero (visible), the terms inside the parentheses must not cancel out. This only happens if $h, k, l$ are **all even** OR **all odd**.

-   If you mix even and odd numbers (e.g., 1, 0, 0), the math results in $1 - 1 + 1 - 1 = 0$. Silence.
    

**The Verdict:**

Let's look at our very first peak from Part (a): **(110)**.

-   $h=1$ (Odd)
    
-   $k=1$ (Odd)
    
-   $l=0$ (Even)
    
    This is a "mixed" triplet. For an FCC crystal, the (110) reflection is forbidden (extinction).
    
-   **Conclusion:** It is **NOT** Face-Centered Cubic because our graph clearly shows a (110) peak.
    

---

### Suspect 3: Body-Centered Cubic (bcc)

**The Setup:**

The BCC lattice has **2 atoms** in the unit cell:

1.  $(0, 0, 0)$ (Corner)
    
2.  $(\frac{1}{2}, \frac{1}{2}, \frac{1}{2})$ (Body Center)
    

**The Math (from Image 3):**

We sum the waves from these two atoms:

$$S_{bcc} = f \left( e^{2\pi i(0)} + e^{2\pi i (\frac{h}{2} + \frac{k}{2} + \frac{l}{2})} \right)$$

$$S_{bcc} = f \left( 1 + e^{i\pi(h+k+l)} \right)$$

Since $e^{i\pi} = -1$, this becomes:

$$S_{bcc} = f (1 + (-1)^{h+k+l})$$

**The Rule:**

Look at the term $(-1)^{h+k+l}$.

-   If the sum $(h+k+l)$ is **ODD**, then $(-1)^{\text{odd}} = -1$. The formula becomes $f(1 - 1) = 0$. (Peak Missing).
    
-   If the sum $(h+k+l)$ is **EVEN**, then $(-1)^{\text{even}} = +1$. The formula becomes $f(1 + 1) = 2f$. (Peak Visible!).
    

So, the rule for BCC is: **The sum $h+k+l$ must be an even number.**

**The Verdict:**

Let's check the peaks we found in Part (a):

1.  **(110)**: $1 + 1 + 0 = 2$ (**Even** $\rightarrow$ Allowed)
    
2.  **(200)**: $2 + 0 + 0 = 2$ (**Even** $\rightarrow$ Allowed)
    
3.  **(211)**: $2 + 1 + 1 = 4$ (**Even** $\rightarrow$ Allowed)
    
4.  **(220)**: $2 + 2 + 0 = 4$ (**Even** $\rightarrow$ Allowed)
    
5.  **(310)**: $3 + 1 + 0 = 4$ (**Even** $\rightarrow$ Allowed)
    

**Final Conclusion:**

Every single peak in our diffractogram follows the BCC rule ($h+k+l = \text{even}$).

Therefore, the crystal structure is **Body-Centered Cubic (bcc)**.

That wraps up Part (b)! You have successfully used quantum interference math to look inside a crystal. Is there a Part (c) to this problem, or perhaps you'd like to calculate the atomic radius of this BCC crystal?