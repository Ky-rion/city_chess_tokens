

Hello again! This is a fantastic question that builds perfectly on our last discussion. In part (1.a), we showed abstractly that the integral $\int \omega = 0$ is _not_ guaranteed. Now, part (1.b) asks us to prove it by finding a set of closed paths where the integral is explicitly **not** zero.

Let's walk through it. The final answer, which is quite elegant, is that the integral is **$I(z_0) = -2\pi$** for any $z_0$ in the given range. It's a constant!

Here is the detailed derivation.

---

### 1. 🗺️ Step 1: Identify the Path $\gamma(z_0)$

The problem asks us to find a suitable closed path $\gamma(z_0)$ that satisfies two conditions:

1.  It lies on the hemisphere $S_+$: $x^2 + y^2 + z^2 = 1$ (with $z \ge 0$).
    
2.  It has a constant $z$-coordinate: $z = z_0$.
    

To find out what this path looks like, we just combine these two equations. We substitute $z = z_0$ into the equation for the sphere:

$$x^2 + y^2 + (z_0)^2 = 1$$

$$x^2 + y^2 = 1 - (z_0)^2$$

This is the equation of a circle!

-   Its center is at $(0, 0, z_0)$.
    
-   Its radius is $R = \sqrt{1 - (z_0)^2}$.
    

So, the path $\gamma(z_0)$ is simply a **circle of latitude** on the hemisphere, at a constant height $z_0$. The condition $0 \le z_0 < 1$ ensures this circle is well-defined.

-   If $z_0 = 0$, it's the "equator" (a circle of radius 1).
    
-   If $z_0$ is close to 1 (e.g., $z_0 = 0.99$), it's a tiny circle near the "north pole."
    

### 2. 🧭 Step 2: Choose a Suitable Parameterization

Now we need to "walk" along this circular path. We can parameterize it using an angle $t$ that goes from $0$ to $2\pi$. A standard parameterization $\mathbf{r}(t) = (x(t), y(t), z(t))$ for a circle of radius $R = \sqrt{1 - (z_0)^2}$ at height $z_0$ is:

-   $x(t) = R \cos(t) = \sqrt{1 - (z_0)^2} \cos(t)$
    
-   $y(t) = R \sin(t) = \sqrt{1 - (z_0)^2} \sin(t)$
    
-   $z(t) = z_0$
    

Our path $\gamma(z_0)$ is now described by this function $\mathbf{r}(t)$ as $t$ runs from $0$ to $2\pi$.

### 3. 🧮 Step 3: Calculate the Integral

We need to compute $I(z_0) = \int_{\gamma(z_0)} \omega$. We know from the problem statement that $\omega = \frac{1}{y} dx$.

To solve this line integral, we must "pull back" all the components ($y$ and $dx$) into our parameter $t$:

1.  Substitute $y$: We replace $y$ with its function of $t$:
    
    $$y(t) = \sqrt{1 - (z_0)^2} \sin(t)$$
    
2.  Substitute $dx$: We find $dx$ by differentiating $x(t)$ with respect to $t$:
    
    $$x(t) = \sqrt{1 - (z_0)^2} \cos(t)$$
    
    $$\frac{dx}{dt} = \frac{d}{dt} \left[ \sqrt{1 - (z_0)^2} \cos(t) \right] = \sqrt{1 - (z_0)^2} \cdot (-\sin(t))$$
    
    Therefore, $dx = -\sqrt{1 - (z_0)^2} \sin(t) \, dt$.
    

Now, we replace $\frac{1}{y}$ and $dx$ in the integral. Our integration bounds are from $t=0$ to $t=2\pi$.

$$I(z_0) = \int_0^{2\pi} \underbrace{\left( \frac{1}{\sqrt{1 - (z_0)^2} \sin(t)} \right)}_{\frac{1}{y}} \cdot \underbrace{\left( -\sqrt{1 - (z_0)^2} \sin(t) \, dt \right)}_{dx}$$

Look at this integrand. A beautiful cancellation happens!

$$I(z_0) = \int_0^{2\pi} \frac{-\sqrt{1 - (z_0)^2} \sin(t)}{\sqrt{1 - (z_0)^2} \sin(t)} \, dt$$

(A quick note: We might worry about $y=0$, which happens at $t=0$ and $t=\pi$. But since the terms cancel so perfectly, the integrand is well-defined and is just $-1$.)

$$I(z_0) = \int_0^{2\pi} -1 \, dt$$

This is now a very simple integral to solve:

$$I(z_0) = [-t]_0^{2\pi} = (-2\pi) - (0)$$

$$I(z_0) = -2\pi$$

### 💡 The Conclusion (and what it means)

The result is $I(z_0) = -2\pi$.

This is a fantastic result for two reasons:

1.  **It's not zero!** This provides a concrete _counterexample_ to the statement in (1.a). We have found a whole family of closed paths $\gamma(z_0)$ for which the integral is **not** zero. This is the definitive proof that $\omega$ is **not an exact form** (it doesn't come from a potential function $f$).
    
2.  **It's independent of $z_0$!** This is the most profound part. The integral along the large equator ($z_0=0$) is $-2\pi$. The integral along a tiny circle just below the north pole (e.g., $z_0=0.999$) is _also_ $-2\pi$.
    

This tells us that the "non-conservativeness" of this "field" $\omega$ is a fundamental property. The value of the integral doesn't depend on the size of the loop, only on the fact that it _is_ a loop. This is a deep concept that you will explore further with **Stokes' Theorem**, which connects the integral along a path (like our $\int \omega$) to an integral over the surface bounded by that path (an integral of $d\omega$, which we found was non-zero!).

This result is a beautiful demonstration of how topology and calculus are deeply linked.

Does it make sense why the result is constant, even though the path length changes dramatically with $z_0$?