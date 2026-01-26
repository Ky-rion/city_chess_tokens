

![[Pasted image 20260125183305.png]]
![[Pasted image 20260125183324.png]]

Excellent work following along! You are doing great. Now we enter the "Upside Down" of solid-state physics: the **Reciprocal Lattice** (reziprokes Gitter).

In Part b), we need to transform our "real world" vectors ($\vec{a}$) into "reciprocal world" vectors ($\vec{b}$). This is crucial because while atoms live in real space, things like X-ray diffraction patterns and electron waves live in reciprocal space.

---

### Step 1: The Golden Rule of Reciprocal Space

The bridge between these two worlds is defined by a simple dot product rule. Your professor’s solution states this clearly in equation (3):

$$\vec{a}_i \cdot \vec{b}_j = 2\pi \delta_{ij}$$

**What does this mean in plain English?**

-   If the indices match ($i=j$), the product is $2\pi$.
    
-   If the indices are different ($i \neq j$), the product is **zero** (meaning they are perpendicular!).
    

So, to find our unknown vectors $\vec{b}_1$ and $\vec{b}_2$, we just need to solve a few mini-puzzles.

---

### Step 2: Calculating Vector $\vec{b}_1$

We are looking for $\vec{b}_1 = \begin{pmatrix} x \\ y \end{pmatrix}$.

**Condition 1: It must "match" $\vec{a}_1$**

Using the rule $\vec{a}_1 \cdot \vec{b}_1 = 2\pi$:

$$\vec{a}_1 \cdot \vec{b}_1 = a \begin{pmatrix} 1 \\ 0 \end{pmatrix} \cdot \begin{pmatrix} x \\ y \end{pmatrix} = a(1\cdot x + 0\cdot y) = ax$$

$$ax = 2\pi \quad \Rightarrow \quad x = \frac{2\pi}{a}$$

**Condition 2: It must be perpendicular to $\vec{a}_2$**

Using the rule $\vec{a}_2 \cdot \vec{b}_1 = 0$:

$$\vec{a}_2 \cdot \vec{b}_1 = \frac{a}{3} \begin{pmatrix} 1 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} \frac{2\pi}{a} \\ y \end{pmatrix} = 0$$

Let's drop the factor $\frac{a}{3}$ (since it can't be zero) and focus on the dot product inside:

$$1 \cdot \left(\frac{2\pi}{a}\right) + 2 \cdot y = 0$$

$$2y = -\frac{2\pi}{a} \quad \Rightarrow \quad y = -\frac{\pi}{a}$$

**Result for $\vec{b}_1$:**

$$\vec{b}_1 = \begin{pmatrix} \frac{2\pi}{a} \\ -\frac{\pi}{a} \end{pmatrix} = \frac{2\pi}{a} \begin{pmatrix} 1 \\ -1/2 \end{pmatrix}$$

_(Note: The professor writes it as $\frac{2\pi}{a} \begin{pmatrix} 1 \\ -1/2 \end{pmatrix}$ to keep the units clean)_.

---

### Step 3: Calculating Vector $\vec{b}_2$

Now we look for $\vec{b}_2 = \begin{pmatrix} x \\ y \end{pmatrix}$.

**Condition 1: It must be perpendicular to $\vec{a}_1$**

Using $\vec{a}_1 \cdot \vec{b}_2 = 0$:

$$\vec{a}_1 \cdot \vec{b}_2 = a \begin{pmatrix} 1 \\ 0 \end{pmatrix} \cdot \begin{pmatrix} x \\ y \end{pmatrix} = ax = 0 \quad \Rightarrow \quad x = 0$$

_This makes sense! Since $\vec{a}_1$ is horizontal, $\vec{b}_2$ (which must be perpendicular to it) must be purely vertical._

**Condition 2: It must "match" $\vec{a}_2$**

Using $\vec{a}_2 \cdot \vec{b}_2 = 2\pi$:

$$\vec{a}_2 \cdot \vec{b}_2 = \frac{a}{3} \begin{pmatrix} 1 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 0 \\ y \end{pmatrix} = \frac{a}{3}(1\cdot 0 + 2\cdot y) = \frac{2ay}{3}$$

$$\frac{2ay}{3} = 2\pi \quad \Rightarrow \quad y = \frac{3\pi}{a}$$

**Result for $\vec{b}_2$:**

$$\vec{b}_2 = \begin{pmatrix} 0 \\ \frac{3\pi}{a} \end{pmatrix} = \frac{2\pi}{a} \begin{pmatrix} 0 \\ 3/2 \end{pmatrix}$$

---

### Step 4: Drawing the Reciprocal Lattice

Now we visualize this using the professor's drawing in the final image.

1.  **The Axes:** Notice the axes are no longer $x$ and $y$. They are $k_x$ and $k_y$ (or just labeled with units of $1/a$).
    
2.  **The Scale:** The grid in the drawing is scaled so that one large square is roughly $\frac{2\pi}{a}$.
    
3.  **Drawing $\vec{b}_1$:**
    
    -   Go **1 unit** to the right (positive x).
        
    -   Go **0.5 units** down (negative y).
        
    -   See the arrow pointing down-right? That is $\vec{b}_1$.
        
4.  **Drawing $\vec{b}_2$:**
    
    -   Go **0 units** in x.
        
    -   Go **1.5 units** up.
        
    -   See the arrow pointing straight up? That is $\vec{b}_2$.
        
5.  **The New Unit Cell:** Just like before, we complete the parallelogram (the shaded red area with dashed lines).
    

**Professor's Insight:**

Notice the geometric relationship.

-   In real space, $\vec{a}_1$ was horizontal. In reciprocal space, $\vec{b}_2$ is vertical. They are perpendicular!
    
-   Reciprocal vectors are always perpendicular to the "other" real space vector. This is a great way to sanity-check your drawings during an exam.
    

Would you like to move on to calculating the **area** of these unit cells? That's usually the next step in understanding the density of these points!