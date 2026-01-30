

![[Pasted image 20260128115109.png]]

Hello there! Welcome to class. It is wonderful to have such a curious student. Since you are new to this material, we are going to take this step-by-step, building up your intuition before we even touch the calculus.

We are looking at **Question 4(a)**, which asks us how to determine the "size" of an atomic nucleus.

In classical physics, a ball has a hard edge—it has a definite radius $R$. But in quantum mechanics and particle physics, nuclei are "fuzzy." They are clouds of charge. So, instead of a hard edge, we talk about the **mean squared radius** ($\langle r^2 \rangle$). This is essentially a statistical average of how spread out the charge is.

Let's break down the solution provided by the other professor.

---

### 1. The Setup: The "Probability" Cloud

The problem statement gives us a charge distribution:

$$\rho(r) = Z \cdot e \cdot f(r)$$

-   **$Z$**: The number of protons (atomic number).
    
-   **$e$**: The elementary charge.
    
-   **$f(r)$**: This is the most important part for us. It is the **shape function** or density profile. It tells us how the protons are distributed from the center of the nucleus outwards.
    

The problem states that the integral of $f(r)$ over all space is equal to **1**:

$$\iiint f(r) \, dx \, dy \, dz = 1$$

This is just a fancy way of saying $f(r)$ is normalized. If you sum up the "shape" over the entire universe, you get 100% of the nucleus's shape. Think of $f(r)$ as a **probability density**: if you poke a random point in space, $f(r)$ tells you the probability of finding a piece of the nucleus there.

---

### 2. The Goal: The Expectation Value

We want to find $\langle r^2 \rangle$. In statistics and quantum mechanics, when you want to find the average (expectation) value of a variable (in this case, $r^2$), you integrate that variable multiplied by the probability density over all possible space.

So, in Cartesian coordinates ($x, y, z$), the formula is:

$$\langle r^2 \rangle = \iiint r^2 \cdot f(r) \, dx \, dy \, dz$$

This is the first line of the professor's solution.

---

### 3. The Transformation: Switching to Spherical Coordinates

Now, solving this integral in Cartesian coordinates ($dx \, dy \, dz$) would be a nightmare because nuclei are spheres, not cubes! We need to switch to **Spherical Coordinates**.

In spherical coordinates, we trade $x, y, z$ for:

1.  **$r$**: Distance from the center.
    
2.  **$\theta$ (theta)**: The angle down from the vertical axis (North pole).
    
3.  **$\phi$ (phi)**: The angle around the equator.
    

**The Volume Element Trap**

This is the part that trips up almost every physics student the first time. You cannot just swap $dx \, dy \, dz$ for $dr \, d\theta \, d\phi$.

When you integrate in 3D spherical coordinates, the tiny "block" of volume you are summing up gets bigger as you get further away from the center (think of the skin of an onion—there is more onion in the outer layers than the inner layers).

To account for this, we must include the **Jacobian factor** (the volume element):

$$dV = r^2 \sin(\theta) \, dr \, d\theta \, d\phi$$

This leads us to the second line of the professor's solution:

$$= \int_0^\infty \int_0^\pi \int_0^{2\pi} r^2 f(r) \cdot \underbrace{r^2 \sin(\theta) \, dr \, d\theta \, d\phi}_{\text{The Volume Element}}$$

Notice there are **two** $r^2$ terms here now:

1.  The first $r^2$ comes from the quantity we are measuring (mean squared radius).
    
2.  The second $r^2$ comes from the geometry of the volume element.
    

---

### 4. Solving the Integral

Because the nucleus is **spherically symmetric** (the problem states this), $f(r)$ does not depend on the angles $\theta$ or $\phi$. This allows us to separate the integrals.

We can pull the radial parts ($r$) to one side, and the angular parts ($\theta, \phi$) to the other.

**Step A: The Angular Part**

Let's integrate the angles first. This represents summing up the surface area of a unit sphere.

$$\int_0^{2\pi} d\phi \int_0^\pi \sin(\theta) \, d\theta$$

-   The integral of $d\phi$ from $0$ to $2\pi$ is simply **$2\pi$**.
    
-   The integral of $\sin(\theta) d\theta$ from $0$ to $\pi$ is $[-\cos(\theta)]_0^\pi = -(-1) - (-1) = \textbf{2}$.
    

Multiply them together:

$$2\pi \times 2 = 4\pi$$

This is where the **$4\pi$** in the final answer comes from! It physically represents the full solid angle of a sphere.

**Step B: The Radial Part**

Now we are left with the radius. We combine the two $r^2$ terms:

$$r^2 \cdot r^2 = r^4$$

So the radial integral is:

$$\int_0^\infty r^4 f(r) \, dr$$

---

### 5. The Final Result

When we combine the angular result ($4\pi$) with the radial integral, we get the professor's final equation (1):

$$\langle r^2 \rangle = 4\pi \int_0^\infty r^4 f(r) \, dr$$

**What does this tell us?**

It tells us that to find the mean squared radius of a nucleus, you don't need to worry about 3D space. You just need to take the radial profile $f(r)$, multiply it by $r^4$, and integrate from the center to infinity. The $4\pi$ accounts for the fact that we are dealing with spheres.

Does that help clarify how we got from the basic definition to that final integral? We can move on to the next part whenever you are ready!