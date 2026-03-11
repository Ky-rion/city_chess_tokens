

Welcome back! You are making excellent progress. We are shifting gears now from atomic transitions to the dynamics of a free particle. This problem is a classic exercise in understanding how we mathematically describe moving particles in quantum mechanics using "wave packets."

Let's break this down together. As always, we will start by translating the question so we know exactly what we are looking at.

### The Translation

**1.3 Free Motion**

_Let $\phi(p)$ be a wave packet in the interval $[p_0 - \epsilon, p_0 + \epsilon]$ and the Hamiltonian operator in momentum space [3 Pts.]_

$$\hat{H} = A + (\hat{P} - p_0)B + \frac{1}{2}(\hat{P} - p_0)^2C,$$

_Which of the 3 terms A, B, or C determines the mean velocity of the packet? Justify your answer._

---

### The Physics: Understanding Wave Packets and the Hamiltonian

In classical mechanics, a particle has a definite position and a definite momentum. But in quantum mechanics, thanks to the Heisenberg Uncertainty Principle, a localized particle isn't just a single point; it is represented by a **wave packet**.

You can think of a wave packet as a localized "burst" or "envelope" of waves. To build this localized burst, we have to add together (superpose) many individual plane waves, each with a slightly different momentum $p$. The problem states that our wave packet is built from momenta clustered tightly around a central value, $p_0$, within a small window $\pm \epsilon$.

Now, let's look at the operator $\hat{H}$. This is the **Hamiltonian**, which represents the total energy of the system. In this problem, the Hamiltonian has been written out as a Taylor series expansion centered around our wave packet's average momentum, $p_0$.

To find the velocity of the particle, we need to find the velocity of this entire "envelope" of waves as it moves through space. In physics, we call this the **group velocity** ($v_g$).

---

### Solving the Exam Question

To solve this, we need the mathematical bridge between energy (the Hamiltonian) and velocity.

**Step 1: The Relationship Between Energy and Velocity**

From classical mechanics (specifically Hamiltonian mechanics), which carries over elegantly into quantum mechanics via the Heisenberg picture, the velocity $v$ of a particle is given by the derivative of its energy (Hamiltonian) with respect to its momentum $p$:

$$v = \frac{\partial H}{\partial p}$$

_(In strictly quantum mechanical terms, the velocity operator $\hat{v}$ is $\frac{\partial \hat{H}}{\partial \hat{P}}$)_.

**Step 2: Take the Derivative**

Let's apply this derivative to the Hamiltonian given in your exam:

$$\hat{H} = A + (\hat{P} - p_0)B + \frac{1}{2}(\hat{P} - p_0)^2C$$

Taking the derivative with respect to $\hat{P}$:

- The derivative of the constant $A$ is $0$.
    
- The derivative of $(\hat{P} - p_0)B$ is $B$.
    
- The derivative of $\frac{1}{2}(\hat{P} - p_0)^2C$ requires the power rule, giving us $2 \cdot \frac{1}{2}(\hat{P} - p_0)C$, which simplifies to $(\hat{P} - p_0)C$.
    

So, our expression for the velocity operator is:

$$\hat{v} = B + (\hat{P} - p_0)C$$

**Step 3: Evaluate for the Mean Velocity**

The question asks for the _mean_ velocity of the packet. Our wave packet is sharply peaked around the central momentum $p_0$. Therefore, to find the average behavior, we evaluate our velocity expression at the expected momentum value, which is $\langle \hat{P} \rangle \approx p_0$.

If we substitute $p_0$ for $\hat{P}$ in our velocity equation:

$$v_{mean} = B + (p_0 - p_0)C$$

$$v_{mean} = B + 0$$

$$v_{mean} = B$$

### Your Final Answer and Justification

- **The Answer:** The term that determines the mean velocity of the packet is **B**.
    
- **The Justification:** The mean velocity of a wave packet (its group velocity) is given by the first derivative of the Hamiltonian with respect to momentum, evaluated at the central momentum $p_0$. Taking the derivative $\frac{\partial \hat{H}}{\partial \hat{P}}$ yields $B + (\hat{P} - p_0)C$. Evaluating this at $\hat{P} = p_0$ leaves only the constant $B$.
    

---

### A Little Extra Intuition (For your physicist brain)

Just so you completely master this equation, here is what all three terms represent in reality:

- **Term A ($A$):** This is just a constant energy offset. It affects how fast the underlying quantum phase oscillates, but doesn't move the physical envelope itself.
    
- **Term B ($B$):** As we proved, this is the **group velocity**—how fast the particle actually travels through space.
    
- **Term C ($C$):** This term is related to the second derivative of the energy. It represents **dispersion**. Because different momentum waves travel at slightly different speeds, this term dictates how quickly the wave packet will spread out and get wider as time goes on!
    

You are doing a fantastic job working through these fundamentals. Would you like me to walk you through a quick mathematical proof showing exactly how Term C causes that wave packet to spread out over time?