

![[Pasted image 20260126140426.png]]
![[Pasted image 20260126140438.png]]

Hello there! Welcome to Solid State Physics 101. I am delighted to be your professor today. Don't worry if you’ve never seen this before—it looks intimidating with the German text and the diagrams, but the underlying concept is actually quite beautiful and geometric.

Let’s break down the solution to **Part (a)** step-by-step, translating both the language and the physics into plain English.

---

### **1. The Setup: The "Stage" and the "Actors"**

First, let's look at what the problem gives us.

-   **The Actor (The Electrons):** We have a "free electron gas." This means the electrons are zooming around without bumping into anything. Their energy ($E$) depends only on their momentum ($k$).
    
    -   The formula given is the classic parabola:
        
        $$E_k = \frac{\hbar^2 k^2}{2m}$$
        
    -   **Translation:** The energy increases as the square of the wavevector $k$. If you draw $E$ on the y-axis and $k$ on the x-axis, you get a simple U-shaped curve (a parabola).
        
-   **The Stage (The Lattice):** Even though the electrons are "free," we are mathematically imposing a grid (a lattice) on them with a spacing of $a$.
    
    -   This creates a **Brillouin Zone (BZ)**. The boundaries of the "first zone" are always at $k = -\frac{\pi}{a}$ and $k = +\frac{\pi}{a}$.
        
    -   Think of the 1st BZ as the "home base" or the fundamental tile of our graph.
        
-   **The Limit (The Fermi Level):** We are told the Fermi radius is $k_F = 1.2 \frac{\pi}{a}$.
    
    -   **Important:** This tells us how many electrons we have. They fill up the energy states starting from the bottom ($k=0$) like water filling a bucket.
        
    -   Notice that $1.2$ is bigger than $1.0$. This means the "water" (electrons) overflows the boundaries of the first zone ($\frac{\pi}{a}$).
        

---

### **2. Figure 1(a): The Extended Zone Scheme**

Let's look at the left side of the solution image, labeled **"a"**. This is the **Extended Zone Scheme**.

This is the most intuitive view. We simply draw the free electron parabola

$$E \propto k^2$$

without any tricks.

-   **The Parabola:** The blue curve is just our standard parabola. It starts at 0 and goes up on both sides.
    
-   **The Zones:** The vertical dashed lines mark the zones.
    
    -   **1st Brillouin Zone (1.BZ):** The region between $-\frac{\pi}{a}$ and $+\frac{\pi}{a}$.
        
    -   **2nd Brillouin Zone (2.BZ):** The regions immediately outside that, from $\frac{\pi}{a}$ to $\frac{2\pi}{a}$ (and the corresponding negative side).
        
-   **The Bands:**
    
    -   **Band 1:** This is the part of the parabola that sits _inside_ the 1st BZ (the bottom of the U shape).
        
    -   **Band 2:** This is the part of the parabola in the 2nd BZ (the arms of the U shape going up).
        
-   **Occupied States (The Dots):**
    
    -   Look at the **Red Dashed Line**. This is the **Fermi Energy ($E_F$)**.
        
    -   Since $k_F = 1.2 \frac{\pi}{a}$, the electrons fill up states all the way out to $k = \pm 1.2 \frac{\pi}{a}$.
        
    -   **Visual Check:** See how the red dashed line is _higher_ than the energy at the zone boundary (the black dashed line)?
        
    -   This means the electrons fill the entire 1st Zone and spill over into the bottom part of the 2nd Zone.
        

---

### **3. Figure 1(b): The Reduced Zone Scheme**

Now look at the right side, labeled **"b"**. This is the **Reduced Zone Scheme**.

In solid-state physics, we like to keep things tidy. Instead of letting the graph stretch out to infinity, we "fold" everything back into the first zone ($-\frac{\pi}{a}$ to $+\frac{\pi}{a}$). This is allowed because in a lattice, a wavevector $k$ is physically equivalent to $k + \frac{2\pi}{a}$.

**How to "Fold" the Graph:**

1.  **Band 1 (Bottom Curve):** The part of the parabola that was already in the 1st Zone stays exactly where it is.
    
2.  **Band 2 (Top Curves):** Look at the arms of the parabola in image **(a)** that are in the 2nd Zone. We cut them off and shift them by $\frac{2\pi}{a}$ towards the center.
    
    -   The right arm (from $\frac{\pi}{a}$ to $\frac{2\pi}{a}$) is shifted left.
        
    -   The left arm (from $-\frac{2\pi}{a}$ to $-\frac{\pi}{a}$) is shifted right.
        
    -   They meet in the middle at the zone boundary to form that upper "cup" shape you see in image **(b)**.
        

**The Result:**

You now have two energy bands stacked on top of each other inside the "home base" (1st BZ).

-   **Lower Curve:** Band 1.
    
-   **Upper Curve:** Band 2.
    

---

### **4. Marking the Occupied States**

The question asks you to "Mark the occupied states." The solution does this with the black dots and the red dashed line.

-   **The Condition:** States are occupied if their energy is less than the Fermi Energy ($E < E_F$).
    
-   **In the Diagram:**
    
    -   **Band 1 (Bottom):** The entire curve is below the red line. This means **Band 1 is completely full**.
        
    -   **Band 2 (Top):** Only the bottom tip of this band dips below the red line. This means **Band 2 is partially filled**.
        

### **Professor's Summary (The "Aha!" Moment)**

Why does this matter?

Because the Fermi surface crosses through a band (Band 2 is only partially full), this material would behave like a **metal**. Electrons in Band 2 have empty states right above them to move into, allowing them to conduct electricity easily.

**So, to answer the question for your homework:**

1.  Draw the x-axis with boundaries at $\pm \pi/a$.
    
2.  **Extended Scheme:** Draw a big parabola. Draw a horizontal line (Fermi energy) that cuts the parabola _outside_ the boundaries (at $1.2$). Shade everything below that line on the curve.
    
3.  **Reduced Scheme:** "Fold" the outer arms of the parabola into the middle. Draw the same horizontal Fermi line. You will see it sits above the bottom of the second band. Shade the full bottom band and the tip of the second band.
    

Does that help clarify how we get from the "free" parabola to those folded bands? We can tackle part (b) next if you're ready!