

![[Pasted image 20260125182244.png]]

Hello! Welcome to Solid State Physics 101. I am delighted to have a curious student. Don't worry if this looks like a jumble of geometry and German right now—we are going to break it down piece by piece.

The problem you have here is a classic exercise in calculating the **Atomic Packing Factor (APF)**, or in German, *Packungsdichte* (PD).

The structure shown in your image is the **Diamond Cubic Structure**. This is the structure adopted by Carbon (diamond), Silicon, and Germanium.

Let’s walk through the solution provided by the other professor, step-by-step.

---

### Step 1: The Volume of the Box ($V_{EZ}$)

First, look at the equation labeled (1) in the solution image:
$$V_{EZ} = a^3$$

*   **Translation:** $V_{EZ}$ stands for *Volumen der Einheitszelle* (Volume of the Unit Cell).
*   **Explanation:** We model the crystal lattice as a repeating cube. The side length of this cube is called the **lattice constant**, denoted by $a$. Since the volume of a cube is side $\times$ side $\times$ side, the volume of the box holding our atoms is simply $a^3$.

---

### Step 2: Counting the Atoms ($N_{Atome}$)

This is often where students get tripped up. We need to count how many atoms are actually *inside* one specific box.

The solution gives this calculation:
$$N_{Atome} = 4 + 6 * \frac{1}{2} + 8 * \frac{1}{8} = 8 \text{ Atoms}$$

Let's break down where those numbers come from by looking at the first image (the ball-and-stick model):

1.  **The Corners ($8 \times \frac{1}{8}$):** There are 8 atoms at the corners of the cube. However, a corner atom is shared by 8 adjacent cubes. Therefore, only **1/8th** of each corner atom actually belongs to *this* specific box.
    *   $8 \text{ corners} \times \frac{1}{8} = 1 \text{ atom}$.

2.  **The Faces ($6 \times \frac{1}{2}$):** Look at the walls of the cube. There is an atom in the center of every face (this is the "Face Centered" part). There are 6 faces. Each face atom is shared between exactly 2 cubes (this one and the neighbor).
    *   $6 \text{ faces} \times \frac{1}{2} = 3 \text{ atoms}$.

3.  **The Interior ($4$):** Now look *inside* the cage. There are 4 atoms floating completely inside the body of the cube. They are not shared with any other box.
    *   $4 \text{ interior atoms} \times 1 = 4 \text{ atoms}$.

**Total:** $1 + 3 + 4 = \mathbf{8}$ atoms per unit cell.

---

### Step 3: The Geometry of "Hard Spheres"

Now we have to figure out how big the atoms are. The problem asks us to assume "hard spheres" (*harte Kugeln*). Imagine billiard balls packing together. They expand until they bump into each other.

In this specific Diamond structure, the atoms are not touching along the edge of the cube. They touch along the **Body Diagonal** (the line going from the bottom-left-front corner to the top-right-back corner).

The solution image shows a diagram with blue tetrahedrons and calculates equation (2):
$$\frac{\sqrt{3}a}{4} = 2r \quad \leftrightarrow \quad r = \frac{\sqrt{3}}{8}a$$

**Here is the physics derivation for that:**

1.  **Raumdiagonale (Body Diagonal):** The diagonal length across a cube with side $a$ is determined by the Pythagorean theorem in 3D: $\sqrt{a^2 + a^2 + a^2} = \sqrt{3}a$.
2.  **The Quarter Jump:** In the Diamond structure, the interior atoms sit exactly at $1/4$ of the distance along that diagonal.
3.  **Touching:** An atom at a corner touches its nearest neighbor, which is one of those interior atoms.
    *   The distance between the center of the corner atom and the center of the interior atom is exactly **one quarter** of the body diagonal: $\frac{\sqrt{3}a}{4}$.
    *   Since they are touching "hard spheres," this distance must be equal to the radius of the first atom plus the radius of the second atom ($r + r = 2r$).

So, $2r = \frac{\sqrt{3}a}{4}$. If you solve for $r$, you get:
$$r = \frac{\sqrt{3}a}{8}$$

---

### Step 4: The Final Calculation (PD)

Now we have everything we need to solve the problem. We want the **Packing Density (PD)**, which is just a fraction:

$$PD = \frac{\text{Volume of all Atoms}}{\text{Volume of the Unit Cell}}$$

**1. Volume of the Atoms ($V_{Atome}$):**
Since we have 8 atoms, and the volume of one sphere is $\frac{4}{3}\pi r^3$:
$$V_{Atome} = 8 \times \frac{4}{3}\pi r^3$$

Substitute our value for $r$ ($\frac{\sqrt{3}a}{8}$) into this:
$$V_{Atome} = 8 \times \frac{4}{3}\pi \left( \frac{\sqrt{3}a}{8} \right)^3$$

**2. Divide by Box Volume ($a^3$):**
$$PD = \frac{8 \times \frac{4}{3}\pi \left( \frac{\sqrt{3}a}{8} \right)^3}{a^3}$$

If you do the algebra (the $a^3$ terms cancel out, leaving just the numbers), you arrive at equation (3):
$$PD = \frac{\sqrt{3}\pi}{16}$$

**3. The Result:**
$$PD \approx 0.34$$

### Professor's Summary:
The answer is **0.34 (or 34%)**.

This implies that in a diamond crystal, only **34%** of the space is filled with matter, and **66%** is empty space! This is actually a very low number compared to simple metals (which are usually around 74%).

This "open" structure is very important. It explains why silicon (which has this structure) is not as dense as iron, and that openness allows us to "dope" silicon with other atoms to create computer chips!

Does that make sense, or would you like me to clarify the geometry of the diagonal further?