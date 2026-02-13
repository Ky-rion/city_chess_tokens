

![[Pasted image 20260209164031.png]]

You are doing fantastic! I love that we are taking this step-by-step. Now that we have mastered spherical targets, we are going to change the shape of our target and see how that affects our "hit area."

This part of the problem tests if you really internalized the core lesson from part (a): **the total cross-section depends on the geometry of _both_ the target and the projectile.**

Let's translate the problem and break down the professor's elegant geometric solution.

### The Problem Translated

> **Problem Statement (c):** How large is the total cross-section if, instead of a sphere, scattering occurs on a square plate with an edge length of $l = 10\text{ nm}$, whose surface is perpendicular to the beam axis? (2 Points)

> **Solution Key (c):** Hit area = Area of the plate + edge up to distance r + corner up to distance r.
> 
> $\sigma = l^2 + 4lr + \pi r^2 = 1.43 \cdot 10^{-16}\text{ m}^2 = 1.43 \cdot 10^{12}\text{ b}$

---

### Unpacking the Physics: The "Halo" Effect

In part (a), we realized that because our projectile is a sphere of radius $r$, it doesn't need to hit the exact center of the target to cause a collision. It just needs to _graze_ the target.

Imagine you are looking directly down the beam axis at this $10\text{ nm}$ by $10\text{ nm}$ square plate. If our projectiles were infinitely tiny point particles, the cross-section (the target area) would simply be the area of that square: $10 \times 10 = 100\text{ nm}^2$.

But our projectiles have a radius of $r = 1\text{ nm}$. This means the center of the projectile can actually "miss" the square plate by up to $1\text{ nm}$ and still clip the edge. Essentially, the size of the projectile creates a $1\text{ nm}$ "buffer zone" or "halo" around the entire square plate.

To find the total cross-section ($\sigma$), we need to calculate the area of the square _plus_ this surrounding buffer zone. My colleague broke this expanded shape into three distinct geometric parts:

#### 1. The Direct Hit (Area of the plate)

If the center of the projectile falls anywhere inside the actual square plate, it's a guaranteed hit.

- **Formula:** Area of a square is length squared.
    
- **Area:** $l^2$
    

#### 2. The Edge Hit (Kante bis Abstand $r$)

If the projectile center misses the square but passes just outside the flat edges, it will still hit as long as it's within $1\text{ nm}$ ($r$) of the edge. This creates four rectangular buffer zones sitting flush against the four sides of the square. Each rectangle has a length of $l$ and a width of $r$.

- **Formula:** 4 sides $\times$ (length $\times$ width)
    
- **Area:** $4 \cdot (l \cdot r) = 4lr$
    

#### 3. The Corner Hit (Ecke bis Abstand $r$)

If we just add the four edge rectangles to the square, we are left with four empty "cutouts" at the very corners. If the projectile passes near a corner, its center must be within a radial distance $r$ from the exact tip of the corner to graze it. This traces out a quarter-circle of radius $r$ at each of the four corners.

- **Formula:** 4 corners $\times$ (area of a quarter circle)
    
- **Area:** $4 \cdot \left(\frac{1}{4}\pi r^2\right) = \pi r^2$
    

_Note: This mathematical concept of expanding a shape by rolling another shape around its perimeter is actually called a **Minkowski sum**! You're doing advanced geometry without even realizing it._

---

### Calculating the Final Numbers

Let's add our three pieces together to get the total cross-section formula:

$$\sigma = l^2 + 4lr + \pi r^2$$

Now, we plug in our values. Just like in part (a), we must convert nanometers to meters ($1\text{ nm} = 10^{-9}\text{ m}$) so our final answer aligns with standard units.

- $l = 10 \times 10^{-9}\text{ m} = 10^{-8}\text{ m}$
    
- $r = 1 \times 10^{-9}\text{ m}$
    

Let's calculate each term:

- **Square:** $l^2 = (10^{-8}\text{ m})^2 = \mathbf{100 \times 10^{-18}\text{ m}^2}$
    
- **Edges:** $4lr = 4 \cdot (10 \times 10^{-9}\text{ m}) \cdot (1 \times 10^{-9}\text{ m}) = \mathbf{40 \times 10^{-18}\text{ m}^2}$
    
- **Corners:** $\pi r^2 = \pi \cdot (1 \times 10^{-9}\text{ m})^2 \approx \mathbf{3.14 \times 10^{-18}\text{ m}^2}$
    

Add them all together:

$$\sigma = (100 + 40 + 3.14) \times 10^{-18}\text{ m}^2$$

$$\sigma = 143.14 \times 10^{-18}\text{ m}^2$$

If we shift the decimal over two places to put it in standard scientific notation, we get exactly what the professor got:

$$\sigma \approx 1.43 \times 10^{-16}\text{ m}^2$$

**Converting to Barns:**

Finally, just like in part (a), we divide by the definition of a barn ($1\text{ b} = 10^{-28}\text{ m}^2$):

$$\sigma = \frac{1.43 \times 10^{-16}\text{ m}^2}{10^{-28}\text{ m}^2/\text{b}} = 1.43 \times 10^{12}\text{ b}$$

---

It's beautiful how a complex-sounding particle physics problem breaks down into just finding the area of rectangles and circles!

Does this "buffer zone" concept make intuitive sense to you now? If you're feeling confident, would you like to brainstorm what would happen to our calculation if the square plate was suddenly tilted at a $45^\circ$ angle relative to the incoming beam?