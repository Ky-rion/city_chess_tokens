

Ah, an excellent question! This gets to the very heart of _why_ we use 4-vectors in the first place.

Let's do this step-by-step. The question asks us to do four things:

1.  Calculate the transformations of the individual components.
    
2.  "Square" the original 4-vector ($x^\mu$).
    
3.  "Square" the transformed 4-vector ($x^{\prime\mu}$).
    
4.  Compare them and state what's interesting.
    

---

### 1. Transformations of Individual Components

We start with the matrix equation given in your first problem:

$x^{\prime\nu} = \Lambda^\nu_\mu x^\mu$

This is just a compact way of writing a matrix multiplication. Let's write it out in full:

$$\begin{pmatrix} x^{\prime 0} \\ x^{\prime 1} \\ x^{\prime 2} \\ x^{\prime 3} \end{pmatrix} = \begin{pmatrix} \gamma & -\gamma\beta & 0 & 0 \\ -\gamma\beta & \gamma & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix} \begin{pmatrix} x^0 \\ x^1 \\ x^2 \\ x^3 \end{pmatrix}$$

Now, let's replace the generic $x^0, x^1...$ with their physical meanings from your text ($x^0 = ct, x^1 = x, x^2 = y, x^3 = z$).

$$\begin{pmatrix} ct' \\ x' \\ y' \\ z' \end{pmatrix} = \begin{pmatrix} \gamma & -\gamma\beta & 0 & 0 \\ -\gamma\beta & \gamma & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix} \begin{pmatrix} ct \\ x \\ y \\ z \end{pmatrix}$$

By performing the matrix multiplication (row by column), we get the transformation equation for each component:

-   For $ct'$ (the 0-component):
    
    $ct' = (\gamma)(ct) + (-\gamma\beta)(x) + (0)(y) + (0)(z)$
    
    $ct' = \gamma(ct - \beta x)$
    
-   For $x'$ (the 1-component):
    
    $x' = (-\gamma\beta)(ct) + (\gamma)(x) + (0)(y) + (0)(z)$
    
    $x' = \gamma(x - \beta ct)$
    
-   For $y'$ (the 2-component):
    
    $y' = (0)(ct) + (0)(x) + (1)(y) + (0)(z)$
    
    $y' = y$
    
-   For $z'$ (the 3-component):
    
    $z' = (0)(ct) + (0)(x) + (0)(y) + (1)(z)$
    
    $z' = z$
    

These are the famous **Lorentz transformation** equations! The key takeaway here is that the new time ($t'$) and new position ($x'$) are a **mixture** of the old time and position. This is wildly different from classical physics, where $t' = t$.

---

### 2. Squaring the Original 4-Vector ($x^\mu$)

The "square" of a 4-vector is its scalar product with itself, which your text defined as $x \cdot x$. Let's call this quantity $s^2$.

$s^2 = x \cdot x = \eta_{\mu\nu} x^\mu x^\nu$

As the text shows, this expands to:

$s^2 = (x^0)^2 - (x^1)^2 - (x^2)^2 - (x^3)^2$

$s^2 = c^2t^2 - x^2 - y^2 - z^2$

This is our starting value.

---

### 3. Squaring the Transformed 4-Vector ($x^{\prime\mu}$)

Now, let's calculate the "square" of the new 4-vector, $x^{\prime\mu}$. We'll call it $s^{\prime 2}$.

$s^{\prime 2} = x' \cdot x' = (x^{\prime 0})^2 - (x^{\prime 1})^2 - (x^{\prime 2})^2 - (x^{\prime 3})^2$

$s^{\prime 2} = (ct')^2 - (x')^2 - (y')^2 - (z')^2$

This is where the detailed work comes in. We must substitute the transformation equations we found in Part 1 into this new equation.

$s^{\prime 2} = [\gamma(ct - \beta x)]^2 - [\gamma(x - \beta ct)]^2 - (y)^2 - (z)^2$

Let's expand the first two terms:

$s^{\prime 2} = [\gamma^2(c^2t^2 - 2\beta ctx + \beta^2x^2)] - [\gamma^2(x^2 - 2\beta ctx + \beta^2c^2t^2)] - y^2 - z^2$

Now, let's factor out the $\gamma^2$ from the square brackets:

$s^{\prime 2} = \gamma^2 [ (c^2t^2 - 2\beta ctx + \beta^2x^2) - (x^2 - 2\beta ctx + \beta^2c^2t^2) ] - y^2 - z^2$

Distribute the negative sign inside the brackets:

$s^{\prime 2} = \gamma^2 [ c^2t^2 - 2\beta ctx + \beta^2x^2 - x^2 + 2\beta ctx - \beta^2c^2t^2 ] - y^2 - z^2$

Look for terms that cancel. The "cross term" $-2\beta ctx$ and $+2\beta ctx$ cancel out!

$s^{\prime 2} = \gamma^2 [ c^2t^2 + \beta^2x^2 - x^2 - \beta^2c^2t^2 ] - y^2 - z^2$

Now, let's group the $c^2t^2$ terms and the $x^2$ terms:

$s^{\prime 2} = \gamma^2 [ (c^2t^2 - \beta^2c^2t^2) + (\beta^2x^2 - x^2) ] - y^2 - z^2$

Factor out $c^2t^2$ from the first parenthesis and $-x^2$ from the second:

$s^{\prime 2} = \gamma^2 [ c^2t^2(1 - \beta^2) - x^2(1 - \beta^2) ] - y^2 - z^2$

We can factor out the $(1 - \beta^2)$ term:

$s^{\prime 2} = \gamma^2 (1 - \beta^2) [ c^2t^2 - x^2 ] - y^2 - z^2$

Now for the final, magic step! Remember the definition of $\gamma$:

$\gamma = \frac{1}{\sqrt{1 - \beta^2}}$

If we square both sides: $\gamma^2 = \frac{1}{1 - \beta^2}$

This means: $\gamma^2 (1 - \beta^2) = 1$

The entire $\gamma^2 (1 - \beta^2)$ part of our equation just becomes 1!

$s^{\prime 2} = (1) [ c^2t^2 - x^2 ] - y^2 - z^2$

$s^{\prime 2} = c^2t^2 - x^2 - y^2 - z^2$

---

### 4. Comparison and What's Interesting

Let's compare our two results:

-   **Original "square":** $s^2 = c^2t^2 - x^2 - y^2 - z^2$
    
-   **New "square":** $s^{\prime 2} = c^2t^2 - x^2 - y^2 - z^2$
    

> **They are exactly the same. $s^2 = s^{\prime 2}$**

This is the punchline, and it is **the single most important concept** in special relativity.

What's interesting?

The individual components of the 4-vector are not the same. As we saw in Part 1, $t' \neq t$ (time dilation) and $x' \neq x$ (length contraction). Different observers moving relative to each other will measure completely different times and distances.

However, the specific combination $s^2 = (ct)^2 - x^2 - y^2 - z^2$ **is the same for all observers**.

This quantity, $s^2$, is called the **spacetime interval** (or "invariant interval"). It is a **Lorentz Invariant**—a number that does not change, no matter which inertial reference frame you use to calculate it.

Think of it this way:

In 3D space, if you rotate a ruler, its projection on the x-axis changes, and its projection on the y-axis changes. But its total length $L^2 = x^2 + y^2 + z^2$ is invariant (it doesn't change).

In 4D spacetime, a Lorentz boost (changing your velocity) is like a "rotation" between the time axis and a space axis. The "time component" ($ct$) changes, and the "space component" ($x$) changes. But the total spacetime "length" $s^2 = (ct)^2 - x^2 - y^2 - z^2$ is invariant.

This invariance is the foundation upon which all of modern particle physics is built.

Does this idea of an "invariant interval" that all observers agree on, even when they disagree on time and distance, make sense? We can dive deeper into what $s^2$ means physically (time-like, space-like, light-like) if you want!