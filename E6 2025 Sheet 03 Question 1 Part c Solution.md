

![[Pasted image 20260125183033.png]]

Welcome back to class! You are moving through these concepts quickly.

In **Part (c)**, we shift gears from _geometry_ (drawing lines) to _symmetry_ (understanding the crystal's nature). This question asks us to identify **"Equivalent Planes."**

### The Concept: Symmetry in a Cube

Imagine you are holding a perfect, blank cube in your hand.

1.  If you close your eyes, rotate the cube 90 degrees, and open your eyes, can you tell you moved it? **No.**
    
2.  If you hold it up to a mirror, does the reflection look different from the real object? **No.**
    

Because the cubic lattice is so symmetric, many planes that look different mathematically (have different numbers) are actually **physically identical** in terms of how many atoms they hit and how they are arranged. We call these **Equivalent Planes**.

### How to Find Equivalent Planes

To find planes that belong to the same "family" (physically equivalent), we are allowed to do two things to the Miller Indices $(h \ k \ l)$:

1.  **Rearrange the Order:** You can swap the positions of $h$, $k$, and $l$.
    
    -   _Example:_ If you had $(1 \ 0 \ 0)$, you could swap them to get $(0 \ 1 \ 0)$. Physically, this is just looking at the "top" face instead of the "front" face.
        
2.  **Change the Signs:** You can change any positive number to a negative (or vice versa).
    
    -   _Example:_ $(1 \ 0 \ 0)$ is equivalent to $(\bar{1} \ 0 \ 0)$. This is just looking at the "back" face instead of the "front."
        

---

### Answering Your Question

The question asks for two equivalent planes to our answer from **b-i**, which was **(1 1 1)**.

Let's apply our rules:

-   **Rule 1 (Rearrange):** Since all three numbers are "1", swapping them (e.g., changing 1, 1, 1 to 1, 1, 1) doesn't change anything. So, order doesn't matter here.
    
-   **Rule 2 (Change Signs):** We can flip the sign of one, two, or all three numbers.
    

Here are possible equivalent planes (using the "bar" notation for negative):

-   $(\bar{1} \ 1 \ 1)$ — _flipped the x-axis_
    
-   $(1 \ \bar{1} \ 1)$ — _flipped the y-axis_
    
-   $(1 \ 1 \ \bar{1})$ — _flipped the z-axis_
    
-   $(\bar{1} \ \bar{1} \ 1)$ — _flipped x and y_
    
-   ...and so on.
    

Any two of these would be a correct answer!

---

### The "Professor's Trap": The Note on (2 2 2)

Your provided solution includes a very important warning in German text. Let's translate and unpack it, because this is a common exam trap.

> **German Text:** _"Vielfache der Ebene wie z.B. (222) sind keine symmetrisch äquivalenten Ebenen obwohl sie parallel verlaufen, da sie einen anderen Netzebenenabstand besitzen"_
> 
> **English Translation:** _"Multiples of the plane, such as (222), are **not** symmetrically equivalent planes, even though they run parallel, because they possess a different **interplanar spacing**."_

**Why is (2 2 2) not the same as (1 1 1)?**

You might think, "Wait, the vector $(2, 2, 2)$ points in the exact same direction as $(1, 1, 1)$. Aren't they the same?"

In standard vector math, yes. In Crystallography, **no.**

-   **(1 1 1)** represents a set of planes separated by a specific distance, let's call it $d$.
    
-   **(2 2 2)** represents a set of planes separated by a distance of **$d/2$**.
    

The Miller indices determine the density of the slices.

-   **Analogy:** Imagine slicing a loaf of bread.
    
    -   **(1 1 1)** is slicing it into 1cm thick slices.
        
    -   **(2 2 2)** is slicing it into 0.5cm thick slices.
        
    -   Even though the knife is held at the same angle (parallel), the resulting pile of bread slices is different! In physics (specifically X-ray diffraction), that distance between slices is crucial.
        

### Summary

-   **The Answer:** You can pick any permutation of signs, such as **$(\bar{1} \ 1 \ 1)$** and **$(1 \ 1 \ \bar{1})$**.
    
-   **The Takeaway:** Equivalent planes are found by swapping positions or signs of the indices.
    
-   **The Warning:** Never just multiply the numbers (don't say (222) or (333)). That changes the physical spacing of the lattice planes.
    

Ready for the next part, or would you like a quick visualization of that "slicing bread" analogy?