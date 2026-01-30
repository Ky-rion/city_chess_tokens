

![[Pasted image 20260128115353.png]]

Hello there! Welcome to class. I am delighted to be your guide into the fascinating world of particle physics. It is perfectly normal to feel a bit intimidated by integrals like these at first, but I promise you, once we break it down, it is just a beautiful piece of geometry and calculus working together.

Today we are looking at **nuclear form factors**. In simple terms, a "form factor" is a mathematical way of describing the "shape" or internal structure of a particle (like a nucleus) when we scatter other particles (like electrons) off of it.

If a nucleus were just a point with no size, this math would be trivial. But nuclei are fuzzy balls of charge! This derivation connects that "fuzzy ball" shape (the charge distribution $\rho(r)$) to the scattering behavior we measure in the lab ($F(q)$).

Let's walk through the solution provided by your other professor step-by-step.

---

### Step 1: The Definition

We start with the general definition of the form factor provided in the problem statement. This is our "recipe":

$$F(\vec{q}) = \int f(\vec{r}) e^{i\vec{q}\cdot\vec{r}/\hbar} dV$$

**What does this mean?**

-   $f(\vec{r})$ is the shape of the charge. The problem tells us $f(\vec{r}) = \frac{1}{Ze} \rho(r)$.
    
    -   $\rho(r)$ is the charge density at radius $r$.
        
    -   $Ze$ is the total charge of the nucleus ($Z$ protons $\times$ charge $e$). Dividing by $Ze$ just normalizes it so the total probability is 1.
        
-   $e^{i\vec{q}\cdot\vec{r}/\hbar}$ is a "phase factor" from quantum mechanics describing the wave nature of the scattering. $\vec{q}$ is the momentum transfer (how hard the electron hit the nucleus).
    
-   $dV$ means we have to integrate (sum up) this over the entire volume of the nucleus.
    

So, substituting the definition of $f(\vec{r})$, our starting point is:

$$F(\vec{q}) = \frac{1}{Ze} \int \rho(r) e^{i\vec{q}\cdot\vec{r}/\hbar} dV$$

---

### Step 2: Choosing the Coordinate System

This is where physics intuition saves us hours of math. The nucleus is **spherical**. Therefore, we should use **Spherical Coordinates** $(r, \theta, \phi)$.

In spherical coordinates, the volume element $dV$ is:

$$dV = r^2 \sin\theta \, dr \, d\theta \, d\phi$$

**The "Z-axis Trick"**:

We need to calculate the dot product $\vec{q} \cdot \vec{r}$. The vector $\vec{r}$ points all over the place as we integrate. But $\vec{q}$ is a fixed vector (the momentum transfer).

To make life easy, we align our coordinate system so that the $z$-axis points exactly along $\vec{q}$.

If $\vec{q}$ is along the $z$-axis, the angle between $\vec{q}$ and $\vec{r}$ is simply the polar angle $\theta$.

$$\vec{q} \cdot \vec{r} = |\vec{q}| |\vec{r}| \cos\theta = qr \cos\theta$$

Now we can rewrite the integral:

$$F(q) = \frac{1}{Ze} \int_0^\infty \int_0^\pi \int_0^{2\pi} \rho(r) e^{i(qr/\hbar)\cos\theta} \underbrace{r^2 \sin\theta \, d\phi \, d\theta \, dr}_{dV}$$

---

### Step 3: The $\phi$ Integral (The Easy Part)

Let's look at the terms inside the integral. Do you see any $\phi$ anywhere in the function?

No! $\rho(r)$ depends only on $r$, and the exponential depends on $r$ and $\theta$.

Since nothing depends on the azimuthal angle $\phi$, we can just integrate it out immediately:

$$\int_0^{2\pi} d\phi = 2\pi$$

Now our expression looks like the third line in your solution image:

$$F(q) = \frac{2\pi}{Ze} \int_0^\infty \int_0^\pi \rho(r) e^{i(qr/\hbar)\cos\theta} r^2 \sin\theta \, d\theta \, dr$$

---

### Step 4: The $\theta$ Integral (The Tricky Part)

This is the part that often trips students up. We need to solve the integral over $\theta$:

$$\int_0^\pi e^{i(qr/\hbar)\cos\theta} \sin\theta \, d\theta$$

Your solution uses a classic calculus substitution trick.

Let $u = \cos\theta$.

Then, the derivative is $du = -\sin\theta \, d\theta$.

(Or as your solution writes it: $d\theta = \frac{d(\cos\theta)}{-\sin\theta}$).

-   When $\theta = 0$, $u = \cos(0) = 1$.
    
-   When $\theta = \pi$, $u = \cos(\pi) = -1$.
    

This allows us to cancel out the $\sin\theta$ term! The integral becomes:

$$\int_{1}^{-1} e^{i(qr/\hbar)u} (-du) = \int_{-1}^{1} e^{i(qr/\hbar)u} du$$

Now we just integrate the exponential function $\int e^{ax} dx = \frac{1}{a} e^{ax}$. Here, our constant $a = iqr/\hbar$.

$$\left[ \frac{1}{i qr / \hbar} e^{i(qr/\hbar)u} \right]_{-1}^{1} = \frac{\hbar}{iqr} \left( e^{iqr/\hbar} - e^{-iqr/\hbar} \right)$$

**Wait, look at that last term.** Does it look familiar?

Recall **Euler's formula** for sine:

$$\sin(x) = \frac{e^{ix} - e^{-ix}}{2i}$$

If we multiply our result by $\frac{2}{2}$, we can force a sine function to appear:

$$\frac{\hbar}{qr} \cdot 2 \cdot \frac{e^{iqr/\hbar} - e^{-iqr/\hbar}}{2i} = \frac{2\hbar}{qr} \sin\left(\frac{qr}{\hbar}\right)$$

---

### Step 5: Putting it all together

Now we substitute that result back into our main expression. We still have the $\frac{2\pi}{Ze}$ out front, and we still have the integration over $r$ (radius).

$$F(q) = \frac{2\pi}{Ze} \int_0^\infty \rho(r) r^2 \cdot \left[ \frac{2\hbar}{qr} \sin\left(\frac{qr}{\hbar}\right) \right] dr$$

Let's clean up the constants and the $r$ terms.

1.  Combine constants: $\frac{2\pi}{Ze} \times 2\hbar = \frac{4\pi\hbar}{Ze}$.
    
2.  Combine $r$ terms: We have an $r^2$ from the volume element and an $\frac{1}{r}$ from the $\theta$ integration result.
    
    $$r^2 \cdot \frac{1}{r} = r$$
    
3.  The $q$ in the denominator stays there.
    

**Final Result:**

$$F(q) = \frac{4\pi\hbar}{Zeq} \int_0^\infty \rho(r) r \sin\left(\frac{qr}{\hbar}\right) dr$$

### Summary

And there you have it! We successfully showed part (a).

**Why is this cool?**

We started with a complicated 3D volume integral. By exploiting the spherical symmetry of the nucleus, we turned it into a much simpler **1D integral** over just the radius $r$.

This tells us that if we know the charge density $\rho(r)$ (how the protons are distributed from the center of the nucleus out to the edge), we can calculate exactly what the scattering experiment $F(q)$ will look like. Conversely, if we measure $F(q)$ in the lab, we can work backward to figure out the shape of the nucleus!

How does that feel? Ready to tackle part (b) when you are?