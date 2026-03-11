

This is a perfect continuation from your previous question! We just proved that the Hamiltonian doesn't care if we swap identical particles. Now, we are going to build the mathematical tools that actually _do_ the swapping and sorting.

First, let's translate the text:

> **3. Give the projectors $\hat{\Pi}_{\pm}$ onto the exchange-symmetric and anti-symmetric functions. [2 Pts.]**

To answer this, we need to understand two things: what "symmetric" and "anti-symmetric" mean in this context, and what a "projector" is. Let's break it down!

---

### Part 1: Symmetries of the Wavefunction

In quantum mechanics, if we have two identical particles, the overall probability of finding them in a specific arrangement cannot change if we simply swap their labels. Mathematically, the probability is the _square_ of the wavefunction, $|\Psi|^2$.

If $|\Psi(x_1, x_2)|^2 = |\Psi(x_2, x_1)|^2$, there are only two possibilities for the wavefunction itself when we swap the particles:

1. **Symmetric (+):** The wavefunction stays exactly the same.
    
    $$\Psi(x_1, x_2) = \Psi(x_2, x_1)$$
    
    Particles that do this are called **Bosons** (like photons).
    
2. **Anti-symmetric (-):** The wavefunction spits out a minus sign.
    
    $$\Psi(x_1, x_2) = -\Psi(x_2, x_1)$$
    
    Particles that do this are called **Fermions** (like electrons, which is what we have in our Helium atom!).
    

### Part 2: What is a Projector?

Imagine you have a messy box containing a mix of red and blue marbles. A "projector" is like a magical sieve. A "red projector" would filter out everything that isn't red, leaving you with a box of purely red marbles.

In math, a projector ($\hat{\Pi}$) takes an arbitrary, messy mathematical function that has no specific symmetry, and forcefully "filters" it so that it becomes purely symmetric or purely anti-symmetric.

### Part 3: The Answer - Building the Projectors

We use the exchange operator $\hat{S}_{12}$ from your previous problem to build these filters. Remember, $\hat{S}_{12}$ swaps particle 1 and particle 2.

Here are the formulas for the projectors:

- **The Symmetric Projector ($\hat{\Pi}_+$):**
    
    $$\hat{\Pi}_+ = \frac{1}{2} (1 + \hat{S}_{12})$$
    
    _(Note: The '1' here represents the identity operator, meaning "do nothing to the function".)_
    
- **The Anti-symmetric Projector ($\hat{\Pi}_-$):**
    
    $$\hat{\Pi}_- = \frac{1}{2} (1 - \hat{S}_{12})$$
    

### Part 4: But _Why_ Does This Work? (The Professor's Proof)

Let's see the magic in action. Let's take a completely random, arbitrary wavefunction $f(x_1, x_2)$ and hit it with the symmetric projector $\hat{\Pi}_+$:

$$\hat{\Pi}_+ f(x_1, x_2) = \frac{1}{2} [f(x_1, x_2) + \hat{S}_{12}f(x_1, x_2)]$$

$$\hat{\Pi}_+ f(x_1, x_2) = \frac{1}{2} [f(x_1, x_2) + f(x_2, x_1)]$$

Let's call this new function $\Psi_{sym}$. Did our filter work? Let's test it by swapping $x_1$ and $x_2$ in our new function:

$$\Psi_{sym}(x_2, x_1) = \frac{1}{2} [f(x_2, x_1) + f(x_1, x_2)]$$

Because addition is commutative ($A+B = B+A$), this is exactly the same as $\Psi_{sym}(x_1, x_2)$! We took a random function and successfully forced it to be symmetric.

If you do the exact same thing with the anti-symmetric projector $\hat{\Pi}_-$, you get:

$$\Psi_{anti} = \frac{1}{2} [f(x_1, x_2) - f(x_2, x_1)]$$

If you swap $x_1$ and $x_2$ here, you get $\frac{1}{2} [f(x_2, x_1) - f(x_1, x_2)]$, which is exactly $-\Psi_{anti}$. The minus sign naturally pops out! The $\frac{1}{2}$ is there just to keep the probabilities normalized.

---

Since our problem is about a Helium atom, our particles are electrons. Electrons are Fermions, which means we will exclusively be relying on that anti-symmetric projector ($\hat{\Pi}_-$) to build valid physical states.

Are you ready to see the next part of the problem where we likely apply these tools to construct the actual ground state of the Helium atom?