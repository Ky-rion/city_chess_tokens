

[It's been wonderful for me too! I've got a little clarifying question about the centrifugal barrier with you. The solution said that around r = 0 the wavefunction was proportional to r^l. Where does this proportionality come from, how do we know this?]


That's a fantastic question! It's one of those "magic" results that often gets stated without proof. It comes directly from solving the Schrödinger equation in 3D.

Here's the mathematical trail.

### 1. The 3D Schrödinger Equation

When we solve the Schrödinger equation in 3D for a central potential $V(r)$ (a potential that only depends on distance $r$), we split the wave function $\psi$ into a radial part $R(r)$ and an angular part $Y_{lm}(\theta, \phi)$.

The equation for the radial part $R(r)$ turns out to be:

$$-\frac{\hbar^2}{2m} \frac{1}{r^2} \frac{d}{dr} \left( r^2 \frac{d R}{dr} \right) + \left[ V(r) + \frac{\hbar^2 l(l+1)}{2mr^2} \right] R(r) = E R(r)$$

That second term in the brackets, $\frac{\hbar^2 l(l+1)}{2mr^2}$, is exactly the **centrifugal barrier** we've been discussing!

### 2. Looking at $r \to 0$

We want to know what this equation forces $R(r)$ to do _very close to the origin_ (as $r \to 0$).

As $r$ gets tiny:

-   The $E$ term is just a constant.
    
-   Most "normal" potentials, like the Coulomb $V(r) \propto 1/r$, are _less_ powerful than...
    
-   ...the centrifugal barrier, which explodes like $\mathbf{1/r^2}$.
    

So, for $r \to 0$, the centrifugal barrier term and the derivative term are the only ones that matter. The equation simplifies to:

$$-\frac{\hbar^2}{2m} \frac{1}{r^2} \frac{d}{dr} \left( r^2 \frac{d R}{dr} \right) + \frac{\hbar^2 l(l+1)}{2mr^2} R(r) \approx 0$$

Let's clean this up by multiplying the whole equation by $-\frac{2mr^2}{\hbar^2}$:

$$\frac{d}{dr} \left( r^2 \frac{d R}{dr} \right) - l(l+1) R(r) \approx 0$$

### 3. Solving the Simplified Equation

This is a standard differential equation. The standard way to solve it is to try a "power-law" solution, exactly what we're looking for:

Let's guess: $R(r) \approx A r^s$ (where $A$ is a constant and $s$ is the exponent we need to find).

Let's plug this guess into our simplified equation:

-   $\frac{d R}{dr} = A s r^{s-1}$
    
-   $r^2 \frac{d R}{dr} = A s r^{s+1}$
    
-   $\frac{d}{dr} (r^2 \frac{d R}{dr}) = \frac{d}{dr} (A s r^{s+1}) = A s (s+1) r^s$
    

Now substitute this back into the equation from Step 2:

$$[A s (s+1) r^s] - l(l+1) [A r^s] = 0$$

We can divide by $A r^s$ (since it's not zero):

$$s(s+1) - l(l+1) = 0$$

$$s^2 + s - l(l+1) = 0$$

This is a simple quadratic equation for $s$. We can solve it by factoring. We need two numbers that add to $+1$ and multiply to $-l(l+1)$. The numbers are $(l+1)$ and $-l$:

$$(s + (l+1))(s - l) = 0$$

This gives two possible solutions for the exponent $s$:

1.  **$s = l$**
    
2.  **$s = -(l+1)$**
    

### 4. The Physical Solution

So, the full "mathematical" solution for $R(r)$ near the origin is a combination of both:

$$R(r) \approx A r^l + B r^{-(l+1)}$$

Now we must apply **physical reality**.

-   The wave function must be "well-behaved." The probability of finding the particle has to be finite.
    
-   The second term, $B r^{-(l+1)}$, is $\frac{B}{r^{l+1}}$.
    
-   As $r \to 0$, this second term **blows up to infinity** (for any $l \ge 0$).
    
-   An infinitely large wave function at the origin is physically impossible. It's "non-normalizable."
    

To prevent this physical impossibility, we are forced to set its coefficient to zero: **$B = 0$**.

This leaves us with only one physically acceptable solution:

$$R(r) \approx A r^l$$

And that's where it comes from! The behavior $\psi \propto r^l$ near the origin is the _only_ solution to the Schrödinger equation that doesn't blow up to infinity at the center.