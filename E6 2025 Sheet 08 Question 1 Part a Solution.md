

![[Pasted image 20260125185821.png]]

Hello! Welcome to "Solid State Physics 101." I am delighted to be your guide. Don't worry if this looks intimidating at first—it is actually a beautiful piece of counting logic once you see past the Greek letters!

We are going to break down **Question 1(a)** and the solution provided in the second image.

The core goal of this problem is to figure out how electrons fit inside a piece of metal. It turns out they don't just pile up randomly; they follow very strict traffic rules known as **Quantum Mechanics**.

---

### 1. The Setup: The Metal Box

Imagine you are holding a small cube of metal.

-   **Size:** The edge length is $L = 1 \text{ cm} = 0.01 \text{ m}$.
    
-   **Electron Density:** The problem gives us $n = 5 \cdot 10^{28} \text{ m}^{-3}$. This tells us how crowded the electrons are.
    

Our job is to count two things:

1.  **"Orbital" States:** How many distinct _parking spots_ exist for electrons up to a certain energy level.
    
2.  **Total Electrons:** How many actual _cars_ (electrons) are parked there.
    

### 2. Welcome to "k-Space"

This is the most important concept in the entire course. In classical mechanics, we describe particles by where they are ($x, y, z$). In Quantum Mechanics for solids, it is often much more useful to describe them by their **momentum** (or wave vector), which we call $\vec{k}$.

Imagine a 3D coordinate system. Instead of $x, y, z$, the axes are $k_x, k_y, k_z$.

In this "k-space," allowed electron states look like a grid of dots. The solution you provided uses **Periodic Boundary Conditions** (a standard mathematical trick), which tells us the spacing between these dots is $2\pi/L$.

-   **The Fermi Sphere:** At absolute zero temperature ($T \to 0$), electrons fill up the lowest energy states first. In k-space, this forms a perfect sphere. The surface of this sphere is the **Fermi Surface**, and its radius is the **Fermi Wave Vector**, $k_F$.
    

---

### 3. Step-by-Step through the Solution

Let's walk through the red text in your second image.

#### Step A: Calculating the Fermi Radius ($k_F$)

The solution starts with:

$$k_F = (3\pi^2 n_e)^{1/3}$$

-   **What this means:** This is the radius of the sphere in k-space that encloses all the electrons. It depends only on the density $n_e$. Higher density $\rightarrow$ larger sphere.
    

#### Step B: Calculating the Volume of the Fermi Sphere ($V_F$)

Next, the professor calculates the volume of that sphere using standard geometry ($Volume = \frac{4}{3}\pi r^3$):

$$V_F = \frac{4}{3} \pi k_F^3$$

By substituting the formula for $k_F$ from Step A into this, they simplify it to:

$$V_F = 4\pi^3 n_e$$

-   **Why do this?** We are trying to find the total "volume" of filled states in this abstract momentum space so we can divide it by the size of a single state later.
    

#### Step C: The Volume of a Single State ($V_k$)

The solution states:

> _"jeder Zustand nimmt ein Volumen von $V = \frac{(2\pi)^3}{L^3}$ im k-Raum ein"_
> 
> _(Every state occupies a volume of ... in k-space)_

Remember the grid of dots? This is the size of the little box surrounding one single dot in our grid.

$$V_k = \frac{(2\pi)^3}{L^3} = \frac{8\pi^3}{L^3}$$

#### Step D: Counting the "States" ($N$)

Now, we simply divide the Total Volume of the sphere by the Volume of one single state. This tells us how many parking spots (dots) are inside the sphere.

$$N = \frac{V_F}{V_k} = \frac{4\pi^3 n_e}{8\pi^3 / L^3}$$

If you cancel out the $\pi^3$ and move the $L^3$ to the top, you get:

$$N = \frac{1}{2} n_e L^3$$

Plugging in the numbers ($n_e = 5 \cdot 10^{28}$ and $L^3 = (10^{-2})^3 = 10^{-6}$):

$$N = 0.5 \cdot (5 \cdot 10^{28}) \cdot 10^{-6} = 2.5 \cdot 10^{22}$$

**Result:** There are **$2.5 \cdot 10^{22}$ spatial states** inside the sphere.

---

### 4. The Second Calculation: Total Electrons ($N_e$)

The problem asks us to calculate the number of conduction electrons in the cube directly.

This is much simpler. We just multiply the density by the real-world volume of the cube ($V_{cube} = L^3$).

$$N_e = V_{cube} \cdot n_e = L^3 \cdot n_e$$

$$N_e = 10^{-6} \text{ m}^3 \cdot 5 \cdot 10^{28} \text{ m}^{-3} = 5 \cdot 10^{22}$$

---

### 5. The "Why?" - The Factor of 2

We have arrived at the punchline of the question.

-   **Number of Spatial States ($N$):** $2.5 \cdot 10^{22}$
    
-   **Number of Electrons ($N_e$):** $5.0 \cdot 10^{22}$
    

**Why do we have exactly twice as many electrons as we have states in the sphere?**

The solution says:

> _"Da jeweils zwei Elektronen einen Zustand besetzen $(\uparrow \downarrow)$ ist $N_e = 2N$."_
> 
> _(Since two electrons occupy one state $(\uparrow \downarrow)$, $N_e = 2N$.)_

**The Explanation:**

This is the **Pauli Exclusion Principle** combined with **Spin**.

In Quantum Mechanics, an electron is defined by where it is moving (its k-state, which we counted in Step D) **AND** its intrinsic spin.

-   Spin can be "Up" ($\uparrow$)
    
-   Spin can be "Down" ($\downarrow$)
    

Every single "dot" in our k-space sphere is actually a bench that fits exactly two people. So, even though we counted $2.5 \cdot 10^{22}$ "parking spots" (k-vectors), we can fit $5.0 \cdot 10^{22}$ electrons into those spots because they pair up.

### Summary

1.  We calculated the volume of the "ball" of electrons in momentum space.
    
2.  We divided that by the size of one momentum "pixel" to find there are $2.5 \cdot 10^{22}$ pixels.
    
3.  We realized that because every pixel holds 2 electrons (Spin Up/Down), the total number of electrons is $5.0 \cdot 10^{22}$.
    

Would you like me to clarify how we derived the formula for $k_F$ or move on to the next part of the question?