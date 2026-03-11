

Welcome back! You are on the final stretch of this problem, and you have built up some incredible momentum to get here.

Let's translate this short and sweet final question:

> **5. Determine $\langle\hat{P}_x^2\rangle$. [1 Pkt.]**

As your AI physics professor, I want to point out a crucial exam meta-strategy here. Notice that this question is only worth **1 point**. When a theoretical physics question is worth just one point, it is practically screaming at you: _"Do not do a massive calculation! Use what you already know!"_

You actually already have all the tools to solve this instantly based on our work in Parts 3 and 4. Here is the breakdown.

---

### Step 1: Breaking Down Momentum

Just like position ($r$) exists in three dimensions ($x, y, z$), the momentum vector ($\vec{P}$) also has three components corresponding to those directions: $\hat{P}_x$, $\hat{P}_y$, and $\hat{P}_z$.

Using the exact same 3D geometry rules we used for distance in Part 3, the total squared momentum is the sum of its squared components:

$$\vec{P}^2 = \hat{P}_x^2 + \hat{P}_y^2 + \hat{P}_z^2$$

If we take the quantum average (expectation value) of this entire equation, we get:

$$\langle\vec{P}^2\rangle = \langle\hat{P}_x^2\rangle + \langle\hat{P}_y^2\rangle + \langle\hat{P}_z^2\rangle$$

### Step 2: The Return of Symmetry

Does this logic feel familiar? It should! We are in the exact same physical situation as we were in Part 3.

The electron is still in the ground state (the 1s orbital). Because this state is perfectly spherically symmetric, the electron's motion is completely isotropic. That means the electron has absolutely no preference for moving along the x-axis, the y-axis, or the z-axis. The physics must be perfectly identical in all three directions.

Therefore, the average squared momentum in each direction must be exactly equal:

$$\langle\hat{P}_x^2\rangle = \langle\hat{P}_y^2\rangle = \langle\hat{P}_z^2\rangle$$

### Step 3: The Instant Calculation

Now we just put the pieces together. Since all three directional components are equal, our total momentum equation simplifies beautifully:

$$\langle\vec{P}^2\rangle = 3\langle\hat{P}_x^2\rangle$$

We just need to isolate the piece we are looking for:

$$\langle\hat{P}_x^2\rangle = \frac{\langle\vec{P}^2\rangle}{3}$$

Finally, we look back at our magnificent work from Part 4, where we calculated that the total squared momentum $\langle\vec{P}^2\rangle$ is equal to 1. Plugging that in gives us our answer:

The expectation value $\langle\hat{P}_x^2\rangle$ is **1/3**.

---

**Summary for your exam paper:**

You can answer this in just one concise sentence to get that final point:

> _Because the ground state is spherically symmetric, the expectation values of the squared momentum components are equal ($\langle\hat{P}_x^2\rangle = \langle\hat{P}_y^2\rangle = \langle\hat{P}_z^2\rangle$), meaning $\langle\hat{P}_x^2\rangle = \langle\vec{P}^2\rangle / 3$. Using our result from part 4 ($\langle\vec{P}^2\rangle = 1$), we find $\langle\hat{P}_x^2\rangle = 1/3$._

Congratulations! You just completely conquered a 17-point university-level quantum mechanics problem on the hydrogen atom.

Since we just calculated the average position spread ($\langle x^2 \rangle$) and the average momentum spread ($\langle\hat{P}_x^2\rangle$), would you like to see how we can multiply those two answers together to prove Heisenberg's famous Uncertainty Principle for this atom?