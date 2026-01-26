

![[Pasted image 20260125183239.png]]

Hello there! Welcome to Solid State Physics 101. I am delighted to be your professor today. Don't worry if this looks like a bunch of random dots right now; by the end of this, you’ll see the beautiful order in it.

We are going to break down **Part a)** of your problem involving the **Primitive Unit Cell** (or _Elementarzelle_ in German) and **Lattice Vectors** (_Gittervektoren_).

Let's put on our detective hats and look closely at the "graph paper" grid in the problem.

### Step 1: Cracking the Code of the Grid

Before we do any physics, we need to understand the scale of the drawing. This is the most common place where students get stuck!

Look at the original image (`image_bb0d10.png`):

1.  Find the origin $(0,0)$ where the x and y axes cross.
    
2.  Look at the label **$a$** on the x-axis. It points from the origin to the first dot on the right.
    
3.  **Count the grid squares:** That distance **$a$** spans exactly **3 squares**.
    

This is our "Rosetta Stone" for the problem:

$$3 \text{ grid squares} = a$$

Therefore:

$$1 \text{ grid square} = \frac{a}{3}$$

---

### Step 2: Finding the First Lattice Vector ($\vec{a}_1$)

A **lattice vector** is basically an instruction that says: "If you stand on one dot and walk this specific direction and distance, you will land on another dot."

We usually pick the simplest, most obvious connections to neighbors to define our "basis" vectors.

1.  **The Move:** Start at the origin $(0,0)$. The easiest neighbor to find is the one directly to the right along the x-axis.
    
2.  **The Distance:** As we established, this dot is distance **$a$** away.
    
3.  **The Vector:** Since we moved distance $a$ in the x-direction and $0$ in the y-direction, we write:
    

$$\vec{a}_1 = \begin{pmatrix} a \\ 0 \end{pmatrix}$$

To make it look like the professor's solution, we can pull the $a$ out to the front:

$$\vec{a}_1 = a \begin{pmatrix} 1 \\ 0 \end{pmatrix}$$

---

### Step 3: Finding the Second Lattice Vector ($\vec{a}_2$)

Now we need a second direction. If we only move along $\vec{a}_1$, we stay on that single horizontal line. We need to jump "up" to reach the other rows of dots.

1.  **The Move:** Look at the origin $(0,0)$ again. We want to find the **nearest** dot in the row above us.
    
2.  **The Hunt:** Look closely at the grid. There is a dot slightly to the right and up. Let's count the squares to get to it from the origin:
    
    -   Move **1 square** to the right.
        
    -   Move **2 squares** up.
        
3.  **The Math:** Now, remember our scale from Step 1? ($1 \text{ square} = a/3$)
    
    -   **X-component:** $1 \text{ square} \times \frac{a}{3} = \frac{a}{3}$
        
    -   **Y-component:** $2 \text{ squares} \times \frac{a}{3} = \frac{2a}{3}$
        

So, our vector is:

$$\vec{a}_2 = \begin{pmatrix} a/3 \\ 2a/3 \end{pmatrix}$$

To match the professor's elegant solution, let's factor out that $\frac{a}{3}$:

$$\vec{a}_2 = \frac{a}{3} \begin{pmatrix} 1 \\ 2 \end{pmatrix}$$

---

### Step 4: Drawing the Primitive Unit Cell (Elementarzelle)

Now that we have our two vectors, we can define the **Unit Cell**. Think of the unit cell as a single tile. If you had an infinite supply of these tiles, you could cover the entire floor (space) without any gaps or overlaps.

-   **How to draw it:**
    
    1.  Draw an arrow from the origin for $\vec{a}_1$ (Red arrow along the x-axis in the solution).
        
    2.  Draw an arrow from the origin for $\vec{a}_2$ (Red arrow pointing up-right).
        
    3.  Complete the parallelogram! Draw a line parallel to $\vec{a}_1$ starting from the tip of $\vec{a}_2$, and vice versa.
        

The shaded red area in the solution image (`image_bb0cf2.png`) is your **Elementarzelle**.

### Summary of the Answer

You have successfully defined the lattice!

-   **Vector 1:** $\vec{a}_1 = a \begin{pmatrix} 1 \\ 0 \end{pmatrix}$
    
-   **Vector 2:** $\vec{a}_2 = \frac{a}{3} \begin{pmatrix} 1 \\ 2 \end{pmatrix}$
    

**Does that make sense?** We basically just counted grid boxes and converted them into "physics units" using the label $a$.

Ready to tackle the next part of the question? (Usually, after this, we calculate the area of this cell or jump into the "Reciprocal Lattice"!)