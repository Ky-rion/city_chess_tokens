

This is the perfect question to end on. It's the one that connects the strange new world of relativity right back to the familiar physics of everyday life.

We're going to show how the classical formula for kinetic energy, $KE = \frac{1}{2}mv^2$, is just an _approximation_ of the more complete relativistic formula.

### 1. The Expression for Energy

In part (c), we were given the expression for total relativistic energy:

$E = \gamma mc^2$

We also know the definitions of $\gamma$ (gamma) and $\beta$ (beta):

$\gamma = \frac{1}{\sqrt{1 - \beta^2}} = (1 - \beta^2)^{-1/2}$

$\beta = v/c$

The "classical limit" $v \ll c$ (velocity is much, much less than the speed of light) is the same as saying **$\beta$ is a very small number** ($\beta \ll 1$). This is the key to our expansion.

### 2. The Taylor Expansion

Let's start by substituting the definition of $\gamma$ into our energy equation:

$E = mc^2(1 - \beta^2)^{-1/2}$

We need to Taylor expand the $(1 - \beta^2)^{-1/2}$ part. For this, we can use the **binomial expansion**, which is a Taylor series for expressions of the form $(1+x)^n$.

The formula for the expansion (for a small $x$) is:

$(1 + x)^n \approx 1 + nx + \frac{n(n-1)}{2!}x^2 + \dots$

For our situation:

-   $x = -\beta^2$
    
-   $n = -1/2$
    

Since the classical limit $\beta$ is very small, $\beta^2$ is tiny, and $\beta^4$ is unimaginably tiny. This means we can get a fantastic approximation by just keeping the first two terms:

$(1 + x)^n \approx 1 + nx$

Let's plug our $x$ and $n$ into this:

$\gamma = (1 - \beta^2)^{-1/2} \approx 1 + (-\frac{1}{2})(-\beta^2)$

$\gamma \approx 1 + \frac{1}{2}\beta^2$

### 3. Finding the Expression for Energy

Now we substitute this simplified $\gamma$ back into our energy equation $E = \gamma mc^2$:

$E \approx (1 + \frac{1}{2}\beta^2) mc^2$

Let's distribute the $mc^2$:

$E \approx mc^2 + \frac{1}{2}\beta^2 mc^2$

Finally, let's replace $\beta$ with its definition, $\beta = v/c$:

$E \approx mc^2 + \frac{1}{2}(\frac{v}{c})^2 mc^2$

Look what happens to the $c^2$ in the second term:

$E \approx mc^2 + \frac{1}{2}(\frac{v^2}{c^2}) mc^2$

$E \approx mc^2 + \frac{1}{2}mv^2$

---

### 4. Interpreting the Result

This is our final result: **$E \approx mc^2 + \frac{1}{2}mv^2$**

Let's look at the two terms on the right side:

1.  **$mc^2$**: This is the particle's **rest energy**. As we found in part (d), this is the energy a particle has _just by existing_, even when it's not moving. This is a purely relativistic idea.
    
2.  **$\frac{1}{2}mv^2$**: This is the **classical kinetic energy**! This is the exact formula you would use in a high-school physics class.
    

This is the interpretation:

The total relativistic energy ($E$) of a particle is the sum of its rest energy (the energy of its mass) and its kinetic energy (the energy of its motion).

At the low speeds of our everyday world ($v \ll c$), the full relativistic formula for energy beautifully simplifies to become the classical formula we always knew, _plus_ a new, constant term, $mc^2$, which classical mechanics never accounted for.

This demonstrates the **correspondence principle**: a new, more general theory (Special Relativity) must successfully reproduce the results of the old, established theory (Classical Mechanics) in the domain where the old theory was known to be valid (low velocities).

You've just proven that Einstein's physics doesn't _replace_ Newton's—it _includes_ it as a special case.

Congratulations on completing this entire problem set! You've derived some of the most fundamental equations in modern physics. How do you feel about these concepts, now that you've seen them all connect?