

Welcome to our solid-state physics session! I am delighted to be your professor today. Since you are new to this, we are going to break this down step-by-step. Physics is often about storytelling with math, so let's uncover the story behind this problem.

This problem is about **Phonons** (quantized sound waves or vibrations in a crystal) colliding and combining. Specifically, it deals with a strange phenomenon called **Umklapp scattering**, which is the primary reason why crystals resist heat flow at higher temperatures.

Here is the plan for our solution:

1.  **The Setup:** Define our coordinate system and constants.
    
2.  **The Vectors:** Mathematically describe the two incoming phonons.
    
3.  **The Collision:** Add them together.
    
4.  **The Check:** See if the new phonon fits in the "allowed box" (The Brillouin Zone).
    
5.  **The Umklapp:** If it doesn't fit, we map it back to its equivalent physical state.
    

---

### Step 1: The Setup & Constants

First, we need to convert everything into consistent units. The problem gives the lattice constant $a$ in nanometers (nm) but the wave vector $k$ in inverse centimeters ($cm^{-1}$). Let's stick to **cm** to match the wave vector.

-   Lattice constant ($a$):
    
    $a = 0.25 \text{ nm} = 0.25 \times 10^{-9} \text{ m} = 0.25 \times 10^{-7} \text{ cm}$
    
-   Magnitude of Phonon 1 ($|\vec{k}_1|$):
    
    $|\vec{k}_1| = 1.15 \times 10^8 \text{ cm}^{-1}$
    

The Rules of the Game (The Brillouin Zone):

In a crystal, momentum is cyclic. It's like a clock face: if you go past 12, you start over at 1. The "12 o'clock" limit in a crystal is the edge of the First Brillouin Zone (1BZ).

For a simple cubic lattice, the 1BZ is a cube. The boundaries of this cube are at $k = \pm \frac{\pi}{a}$ in the $x, y,$ and $z$ directions.

Let's calculate this boundary limit ($k_{max}$):

$$k_{max} = \frac{\pi}{a} = \frac{3.14159}{0.25 \times 10^{-7} \text{ cm}} \approx 1.257 \times 10^8 \text{ cm}^{-1}$$

> **Professor's Note:** Keep this number in mind! **$1.257 \times 10^8$**. Any component of our final vector larger than this means we have left the First Brillouin Zone.

---

### Step 2: Constructing the Vectors

Now, let's write down the vectors for the two phonons.

**Phonon 1 ($\vec{k}_1$):**

-   Direction: $[001]$ (This is the z-direction).
    
-   Magnitude: $1.15 \times 10^8$.
    
-   Vector:
    
    $$\vec{k}_1 = (0, 0, 1.15) \times 10^8 \text{ cm}^{-1}$$
    

**Phonon 2 ($\vec{k}_2$):**

-   Direction: $[011]$. This points diagonally in the y-z plane.
    
-   **Crucial Step:** We must use a **unit vector** for direction. The length of the vector $[0, 1, 1]$ is $\sqrt{0^2 + 1^2 + 1^2} = \sqrt{2}$. So the direction unit vector is $(0, \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}})$.
    
-   Magnitude: The problem states it is "half the length" of the first one.
    
    $|\vec{k}_2| = \frac{1.15}{2} \times 10^8 = 0.575 \times 10^8 \text{ cm}^{-1}$.
    
-   Vector calculation:
    
    $$\vec{k}_2 = 0.575 \times \left( 0, \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}} \right) \times 10^8$$
    
    Since $1/\sqrt{2} \approx 0.707$:
    
    $$\vec{k}_2 \approx (0, 0.4065, 0.4065) \times 10^8 \text{ cm}^{-1}$$
    

---

### Step 3: The Summation (Interaction)

The problem states a new phonon is created by summation. We simply add the vectors component by component.

$$\vec{k}_{sum} = \vec{k}_1 + \vec{k}_2$$

$$\vec{k}_{sum} = (0, 0, 1.15) + (0, 0.4065, 0.4065)$$

(ignoring the $10^8$ factor for a moment)

-   $x$-component: $0 + 0 = 0$
    
-   $y$-component: $0 + 0.4065 = 0.4065$
    
-   $z$-component: $1.15 + 0.4065 = 1.5565$
    

So, the resulting raw vector is:

$$\vec{k}_{sum} = (0, 0.4065, 1.5565) \times 10^8 \text{ cm}^{-1}$$

---

### Step 4: The "Is it Allowed?" Check

Now we look at part (a) of your question: _"Show that it does not belong to the first Brillouin zone."_

Recall our boundary limit from Step 1: **$k_{max} = 1.257 \times 10^8$**.

Let's look at our components:

-   $k_x = 0$ (Safe)
    
-   $k_y = 0.4065$ (Safe, this is less than 1.257)
    
-   $k_z = 1.5565$ (**Violation!** This is greater than 1.257)
    

Because the z-component $1.5565$ is larger than the boundary $\frac{\pi}{a} \approx 1.257$, **the vector extends outside the First Brillouin Zone.**

---

### Step 5: The Umklapp Process (Folding Back)

When a phonon goes outside the zone, the crystal lattice "diffracts" it back in. This is called an **Umklapp** process (German for "flip over"). We must subtract a Reciprocal Lattice Vector $\vec{G}$ to bring it back to the "equivalent" point inside the first zone.

The reciprocal lattice vector $\vec{G}$ has a length of $\frac{2\pi}{a}$.

$$G = \frac{2\pi}{a} = 2 \times k_{max} = 2 \times 1.257 \times 10^8 \approx 2.514 \times 10^8 \text{ cm}^{-1}$$

To fix our overflowing $z$-component, we subtract $G$ from the z-direction:

$$k'_{z} = k_{sum, z} - G$$

$$k'_{z} = (1.5565 - 2.514) \times 10^8$$

$$k'_{z} = -0.9575 \times 10^8 \text{ cm}^{-1}$$

The Final Equivalent Phonon $\vec{k}'$:

We keep the x and y components (they were fine) and use the new folded z component.

$$\vec{k}' \approx (0, \; 0.41, \; -0.96) \times 10^8 \text{ cm}^{-1}$$

### Summary of the Physics

1.  **Result:** Two phonons moving roughly in the "forward" direction collided.
    
2.  **Surprise:** The resulting momentum was so high it "broke the speed limit" of the crystal grid (exceeded the Brillouin Zone).
    
3.  **Umklapp:** The lattice pushed back hard, subtracting momentum ($\vec{G}$).
    
4.  **Outcome:** The resulting phonon has a negative z-component ($-0.96$). Even though the parents were moving "forward" (positive z), the child moves "backward". **This is why Umklapp scattering causes resistance—it turns forward-moving energy around!**
    

Would you like me to explain more about why the lattice subtracts exactly $\frac{2\pi}{a}$?