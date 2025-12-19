

Hello again! I am glad you asked about the second part. This is where we test your intuition about crystal geometry.

In part (a), we saw a collision that broke the "speed limit" of the crystal (Umklapp). Now, we are going to change the direction of the second phonon and see if the outcome changes. We also have a very interesting conceptual question to answer at the end.

Let's dive in!

---

### Part 1: Changing the Direction to [010]

**The New Setup:**

-   Phonon 1 ($\vec{k}_1$): Still unchanged.
    
    $$\vec{k}_1 = (0, 0, 1.15) \times 10^8 \text{ cm}^{-1}$$
    
-   **Phonon 2 ($\vec{k}_2$):**
    
    -   Magnitude: Still $0.575 \times 10^8 \text{ cm}^{-1}$.
        
    -   New Direction: $[010]$ (The positive y-direction).
        
    -   New Vector:
        
        $$\vec{k}_2 = (0, 0.575, 0) \times 10^8 \text{ cm}^{-1}$$
        

The Summation:

We add them together component by component:

$$\vec{k}_{sum} = \vec{k}_1 + \vec{k}_2$$

$$\vec{k}_{sum} = (0, 0, 1.15) + (0, 0.575, 0)$$

$$\vec{k}_{sum} = (0, \; 0.575, \; 1.15) \times 10^8 \text{ cm}^{-1}$$

The Check (Is it Umklapp?):

Recall the "speed limit" (the boundary of the First Brillouin Zone) we calculated earlier:

$$k_{max} = \frac{\pi}{a} \approx 1.257 \times 10^8 \text{ cm}^{-1}$$

For a Simple Cubic lattice, a vector is inside the first zone if **every single component** ($k_x, k_y, k_z$) is smaller than $k_{max}$.

Let's check our new vector components:

1.  **x-component:** $0$ (Safe)
    
2.  **y-component:** $0.575 < 1.257$ (Safe)
    
3.  **z-component:** $1.15 < 1.257$ (Safe!)
    

Conclusion for Part 1:

Because all components are within the boundary limits, the resulting phonon stays inside the First Brillouin Zone.

Answer: No, this would not be Umklapp scattering. This is a Normal process (N-process).

---

### Part 2: The General Concept

The Question:

"Is the combination of two orthogonal phonons in every lattice always in the first Brillouin zone? Justify!"

The Short Answer:

No. It is not always in the first Brillouin zone.

The Explanation (The Counter-Example):

Physics questions that ask if something is "always" true are usually inviting you to find a specific case where it breaks. We can break this rule using the same Simple Cubic lattice we are already using.

Imagine the First Brillouin Zone as a **cube** (box).

-   The distance from the center to the **face** (the wall) is $k_{face} = \frac{\pi}{a}$.
    
-   The distance from the center to a **corner** is much longer: $k_{corner} = \sqrt{3} \frac{\pi}{a}$.
    

This means you can have valid vectors that reach deep into the corners, which are actually _longer_ than the distance to the wall.

**Let's construct a scenario where "Orthogonal Addition" causes an Umklapp:**

1.  Imagine we rotate our coordinate system by $45^\circ$ in the x-y plane.
    
2.  Let's define two vectors, $\vec{A}$ and $\vec{B}$, that point diagonally into the corners of the box.
    

-   **Vector A:** $\vec{A} = (0.9 \frac{\pi}{a}, \; 0.9 \frac{\pi}{a}, \; 0)$
    
    -   Is it inside the zone? Yes! Because $0.9 < 1$, both components are allowed.
        
-   **Vector B:** $\vec{B} = (0.9 \frac{\pi}{a}, \; -0.9 \frac{\pi}{a}, \; 0)$
    
    -   Is it inside the zone? Yes!
        
    -   Are they orthogonal? Let's check the dot product:
        
        $\vec{A} \cdot \vec{B} = (0.9)(0.9) + (0.9)(-0.9) = 0.81 - 0.81 = 0$.
        
        Yes, they are perfectly perpendicular (orthogonal).
        

3.  Now, add them together:
    
    $$\vec{Sum} = \vec{A} + \vec{B} = (1.8 \frac{\pi}{a}, \; 0, \; 0)$$
    
4.  The Result:
    
    The resulting vector points strictly along the x-axis with a length of 1.8 $\frac{\pi}{a}$.
    
    However, the boundary in the x-direction is 1.0 $\frac{\pi}{a}$.
    

Justification:

Even though vectors $\vec{A}$ and $\vec{B}$ were both safe inside the zone (hiding in the corners), and even though they were orthogonal, their sum combined to form a vector that shoots straight out of the box face.

Therefore, the combination of orthogonal phonons is **not** guaranteed to stay in the First Brillouin Zone. Umklapp scattering can still happen!

Professor's Next Step:

Since we've covered the math of scattering, would you like to see a quick calculation of how much energy is lost or conserved in this process compared to the momentum? (This highlights the difference between N-processes and U-processes in thermal conductivity).