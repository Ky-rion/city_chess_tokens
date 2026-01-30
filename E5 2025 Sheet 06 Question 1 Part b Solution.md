

![[Pasted image 20260128115416.png]]

Excellent! Let's continue our journey. You are doing great.

Now we are moving on to **part (b)**. This is actually one of the most important results in experimental nuclear physics.

In part (a), we found a general formula for $F(q)$. In part (b), we are asking: **"What happens in the specific case where the electron barely hits the nucleus?"** (i.e., when the momentum transfer $q$ is very small, close to 0).

The result will show us that the **slope** of the form factor at low energy tells us exactly how big the nucleus is (the "mean square radius" $\langle r^2 \rangle$).

Let's break down the solution step-by-step.

---

### Step 1: The Taylor Expansion Strategy

We have the result from part (a):

$$F(q) = \frac{4\pi\hbar}{Zeq} \int_0^\infty \rho(r) r \sin\left(\frac{qr}{\hbar}\right) dr$$

The problem asks us to look at the behavior near $q=0$. Whenever physicists see "near zero," we immediately reach for a **Taylor Series expansion**.

We know the expansion for $\sin(x)$ when $x$ is small:

$$\sin(x) \approx x - \frac{x^3}{3!} + \dots = x - \frac{x^3}{6}$$

In our integral, the "x" is the term $\frac{qr}{\hbar}$. So, we substitute:

$$\sin\left(\frac{qr}{\hbar}\right) \approx \left(\frac{qr}{\hbar}\right) - \frac{1}{6}\left(\frac{qr}{\hbar}\right)^3$$

---

### Step 2: Substituting into the Integral

Now, let's plug this approximation back into our big equation for $F(q)$.

$$F(q) \approx \frac{4\pi\hbar}{Zeq} \int_0^\infty \rho(r) r \left[ \frac{qr}{\hbar} - \frac{q^3r^3}{6\hbar^3} \right] dr$$

We can split this into two separate integrals (let's call them Term 1 and Term 2).

**Term 1 (The Leading Term):**

$$\frac{4\pi\hbar}{Zeq} \int \rho(r) r \left(\frac{qr}{\hbar}\right) dr = \frac{4\pi\hbar}{Zeq} \cdot \frac{q}{\hbar} \int \rho(r) r^2 dr$$

Everything cancels nicely here! The $\hbar$, $q$, and $q$ all cancel out.

$$\text{Term 1} = \frac{4\pi}{Ze} \int \rho(r) r^2 dr$$

_Physics Pause:_ Recall that $dV = 4\pi r^2 dr$ for spherical symmetry. So $\int \rho(r) 4\pi r^2 dr$ is just the total charge of the nucleus, which is $Ze$.

$$\text{Term 1} = \frac{1}{Ze} \cdot (Ze) = 1$$

This makes sense! If $q=0$ (no scattering), the probability $F(0)$ should be 1.

**Term 2 (The Correction Term):**

$$- \frac{4\pi\hbar}{Zeq} \int \rho(r) r \left( \frac{q^3r^3}{6\hbar^3} \right) dr$$

Let's pull out the constants. We have $q^3$ on top and $q$ on bottom, leaving $q^2$.

$$= - \frac{4\pi\hbar}{Ze} \cdot \frac{q^2}{6\hbar^3} \int \rho(r) r^4 dr$$

$$= - q^2 \cdot \frac{1}{6\hbar^2} \cdot \left[ \frac{4\pi}{Ze} \int \rho(r) r^4 dr \right]$$

So, putting it all together, our form factor looks like this:

$$F(q) \approx 1 - q^2 \left( \frac{1}{6\hbar^2} \frac{4\pi}{Ze} \int \rho(r) r^4 dr \right)$$

---

### Step 3: Identifying the "Mean Square Radius"

Now we need to identify the physics hidden in that second integral.

In statistics, the **mean** (average) of a value $x$ is written as $\langle x \rangle$.

For a distribution $f(r)$, the mean of $r^2$ is defined as:

$$\langle r^2 \rangle = \frac{\int r^2 \cdot f(\vec{r}) dV}{\int f(\vec{r}) dV}$$

Since our probability distribution is the normalized charge distribution $f(r) = \rho(r)/Ze$:

$$\langle r^2 \rangle = \int r^2 \frac{\rho(r)}{Ze} dV$$

Switching to spherical coordinates ($dV = 4\pi r^2 dr$):

$$\langle r^2 \rangle = \frac{4\pi}{Ze} \int_0^\infty r^2 \cdot \rho(r) \cdot r^2 dr = \frac{4\pi}{Ze} \int_0^\infty \rho(r) r^4 dr$$

**Look closely!** This is exactly the term inside our brackets in Step 2!

So we can rewrite our form factor equation as:

$$F(q) \approx 1 - q^2 \frac{\langle r^2 \rangle}{6\hbar^2}$$

---

### Step 4: Taking the Derivative

The question asks for the value of $\frac{dF(q)}{dq^2}$ at $q=0$.

**A note on notation:**

You might look at $\frac{dF}{dq^2}$ and think "second derivative". In this specific context, it is shorthand for "derivative with respect to the variable $q^2$". It's asking for the **slope** if you were to plot $F$ on the y-axis and $q^2$ on the x-axis.

If we look at our linear equation:

$$F(q^2) = 1 - \left( \frac{\langle r^2 \rangle}{6\hbar^2} \right) q^2$$

This is just the equation of a line $y = mx + b$, where $y=F$, $x=q^2$, and the slope $m$ is the coefficient of $q^2$.

Therefore:

$$\frac{dF}{d(q^2)} = - \frac{\langle r^2 \rangle}{6\hbar^2}$$

This matches the result in the solution image exactly!

### Why does this matter?

This is one of the coolest tricks in physics.

1.  We shoot electrons at a nucleus with very low energy (low $q$).
    
2.  We measure how many scatter (finding $F(q)$).
    
3.  We plot $F(q)$ versus $q^2$.
    
4.  We measure the slope of that line.
    
5.  Boom! We immediately know the physical size ($\langle r^2 \rangle$) of the nucleus.
    

This is exactly how we know the radius of the proton is about $0.84$ femtometers!