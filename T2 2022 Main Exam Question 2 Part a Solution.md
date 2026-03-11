

Welcome to the fascinating world of quantum mechanics! I would be delighted to walk you through this problem. It is a fantastic exercise in understanding the "qualitative" behavior of wavefunctions, which physicists use to understand a system's behavior without having to solve horrible differential equations line by line.

First, let's translate the problem from German so we are entirely clear on the task.

**The Setup:**

We have a Hamiltonian operator $\hat{H} = -\frac{1}{2}\partial_x^2 + V(x)$ and a potential function $V(x)$ defined in three pieces:

- $V(x) = 2$ for $x < -1$ (A flat barrier on the left)
    
- $V(x) = 0$ for $-1 \le x \le 0$ (A flat potential well bottom)
    
- $V(x) = 2x^2$ for $x > 0$ (A parabolic harmonic oscillator shape on the right)
    

**The Questions:**

1. Assume there is a ground state $\Phi_0(x)$ with energy $E_0$.
    

- **(a)** Draw the corresponding eigenfunction in each of the intervals $A = (-\infty, -1]$, $B = [-1, a]$, and $C = [a, \infty)$ in a sketch.
    
- **(b)** Describe your drawing: What is the sign of the 2nd derivative in the intervals A, B, and C?
    

As your professor, I am going to teach you a secret: **always solve part (b) before part (a)**. You cannot accurately draw the wavefunction until you know how it curves, and the 2nd derivative is precisely what tells you about the curvature!

---

### Step 1: The Physics of Curvature (Solving Part b)

To find the second derivative, we look at the Time-Independent Schrödinger Equation:

$$\hat{H}\Phi_0(x) = E_0\Phi_0(x)$$

Substituting our specific Hamiltonian, we get:

$$-\frac{1}{2}\frac{d^2\Phi_0}{dx^2} + V(x)\Phi_0(x) = E_0\Phi_0(x)$$

Let's rearrange this to solve for the second derivative, $\Phi_0''(x)$:

$$\Phi_0''(x) = 2(V(x) - E_0)\Phi_0(x)$$

This equation is your best friend for qualitative plotting. By convention, we assume the ground state wavefunction is positive everywhere ($\Phi_0(x) > 0$), as it has no nodes (it never crosses zero). Because $\Phi_0(x)$ is positive, the sign of the second derivative $\Phi_0''(x)$ is completely determined by the sign of $(V(x) - E_0)$.

Before we evaluate the intervals, we need to know where $E_0$ lives. For a bound ground state to exist, its energy must be greater than the absolute minimum of the potential, but lower than the barrier on the left. So, $0 < E_0 < 2$.

The point $a$ mentioned in the problem is the **classical turning point** on the right side. This is the coordinate where the particle's energy exactly equals the potential energy: $E_0 = V(a) = 2a^2$.

Now, let's look at the three intervals:

- **Interval A: $(-\infty, -1]$**
    
    Here, $V(x) = 2$. Since $E_0 < 2$, we know that $V(x) > E_0$.
    
    Looking at our formula, $2(V(x) - E_0)$ is positive. Therefore, **$\Phi_0''(x) > 0$ (Positive)**.
    
    _Meaning:_ The wavefunction curves _away_ from the x-axis (convex).
    
- **Interval B: $[-1, a]$**
    
    Here, the potential dips down to 0 and then rises to meet $E_0$ at $x = a$. Throughout this entire region (except at the exact point $a$), the energy is greater than the potential: $V(x) < E_0$.
    
    Looking at our formula, $2(V(x) - E_0)$ is negative. Therefore, **$\Phi_0''(x) < 0$ (Negative)**.
    
    _Meaning:_ The wavefunction curves _towards_ the x-axis (concave).
    
- **Interval C: $[a, \infty)$**
    
    Here, the potential continues to rise as a parabola, so $V(x) > E_0$.
    
    Just like in region A, $2(V(x) - E_0)$ is positive. Therefore, **$\Phi_0''(x) > 0$ (Positive)**.
    
    _Meaning:_ The wavefunction curves _away_ from the x-axis (convex).
    

---

### Step 2: Sketching the Wavefunction (Solving Part a)

Now that we know the curvature, drawing the sketch is just a matter of connecting the dots while respecting the rules of quantum mechanics (the function must be smooth, continuous, and approach 0 at infinity).

Here is how you should draw it on your paper:

1. **The Setup:** Draw your x and y axes. Draw the potential $V(x)$ (a horizontal line at $y=2$ on the left, dropping to $y=0$ between -1 and 0, and a parabola rising on the right). Draw a dashed horizontal line for $E_0$ somewhere between $y=0$ and $y=2$. Mark the intersections as $x=-1$ and $x=a$.
    
2. **Interval A (The Left Tail):** Start very close to $y=0$ on the far left. Draw a curve that slowly rises. Because the 2nd derivative is positive, it must look like the left side of a smile (curving upward). It hits $x=-1$.
    
3. **Interval B (The Peak):** At $x=-1$, the curvature instantly flips. The curve smoothly transitions into looking like a frown (concave down). It reaches a single peak maximum somewhere in this interval, and begins to slope back downward until it hits $x=a$.
    
4. **Interval C (The Right Tail):** At $x=a$, the curvature flips back! The "frown" turns back into a "smile" shape, curving smoothly so that it asymptotically approaches the x-axis as $x$ goes to infinity.
    

The points $x=-1$ and $x=a$ are **inflection points**—this is where the classical and quantum worlds shake hands, marking the boundaries where the particle transitions from classically "allowed" regions to classically "forbidden" (tunneling) regions!

---

Would you like me to walk you through how the shape of this ground state wavefunction would change if we were looking at the _first excited state_ instead?