

![[Pasted image 20260209163533.png]]

Welcome to Particle Physics 101! I am delighted to be your guide. Don't worry if this looks intimidating at first glance; we are going to break it down step-by-step.

This problem is a classic example of "Relativistic Kinematics"—basically, how things move and collide when they are traveling near the speed of light.

Here is the breakdown of part **(a)**, using the solution provided by your other professor.

### The Goal: Finding the "Available" Energy

The question asks for the **Schwerpunktsenergie**, which translates to **Center-of-Mass (CM) Energy**.

In particle physics, we denote the square of this energy with the symbol **$s$**. So, the Center-of-Mass energy itself is written as **$\sqrt{s}$**.

Think of $\sqrt{s}$ as the "useful" energy in a collision. It is the total energy available to create new particles (like the $\Upsilon(4S)$ meson mentioned in the text).

### 1. The Setup

We have two particles colliding head-on (frontal):

1. **Electron ($e^-$):** Energy $E_1 = 7 \text{ GeV}$.
    
2. **Positron ($e^+$):** Energy $E_2 = 4 \text{ GeV}$.
    

Notice that the energies are _asymmetric_ ($7$ vs $4$). In older colliders, beams often had equal energy. In Belle-II (as the text notes), they are asymmetric to give the resulting particles a little "boost" so they move in the lab, making them easier to measure.

### 2. The "Massless" Assumption

In the solution image, you see the phrase: _"Bei masselosen Elektronen/Positronen"_ (For massless electrons/positrons).

**Why do we assume they are massless?**

The mass of an electron is approximately $0.000511 \text{ GeV}$. The collision energy is $7 \text{ GeV}$.

$$7 \text{ GeV} \gg 0.000511 \text{ GeV}$$

Since the kinetic energy is so massive compared to the particle's rest mass, we can safely ignore the rest mass to simplify the math without losing accuracy. This is the **Ultra-relativistic limit**.

In this limit:

$$Energy (E) \approx Momentum (p) \times c$$

(If we work in "natural units" where $c=1$, then simply $E \approx p$).

### 3. Decoding the Solution Formula

The solution uses the concept of **Invariant Mass**. The fundamental rule of relativistic kinematics is that the "length" of the energy-momentum 4-vector is conserved.

The formula for the invariant mass squared ($s$) of a system is:

$$s = (E_{total})^2 - (\vec{p}_{total})^2$$

Let's look at the formula in the image:

$$\sqrt{s} = \sqrt{(7+4)^2 - (7-4)^2}$$

Here is why the numbers are arranged that way:

**A. The Total Energy term $(7+4)^2$:**

Energy is a **scalar** (it has no direction). To get the total energy of the system, you simply add the energy of the two particles together.

$$E_{total} = 7 \text{ GeV} + 4 \text{ GeV} = 11 \text{ GeV}$$

**B. The Total Momentum term $(7-4)^2$:**

Momentum is a **vector** (it has direction).

- The electron is flying to the right (let's say positive direction): $+7 \text{ GeV}/c$.
    
- The positron is flying head-on to the left (negative direction): $-4 \text{ GeV}/c$.
    

When you add these vectors, they partially cancel each other out:

$$p_{total} = |7 - 4| = 3 \text{ GeV}/c$$

**C. Putting it together:**

Now we plug these into the master formula ($E^2 - p^2$):

$$\sqrt{s} = \sqrt{(11)^2 - (3)^2}$$

$$\sqrt{s} = \sqrt{121 - 9}$$

$$\sqrt{s} = \sqrt{112}$$

### 4. The Result

When you calculate $\sqrt{112}$, you get approximately:

$$\mathbf{10.583 \text{ GeV}}$$

This matches the solution provided!

**Why is this specific number important?**

The text mentions that $\Upsilon(4S)$ mesons are created. The mass of an $\Upsilon(4S)$ meson is almost exactly **$10.58 \text{ GeV}/c^2$**. The scientists at Belle-II specifically tuned the energies of the electron ($7$) and positron ($4$) beams so that the total available energy ($\sqrt{s}$) would perfectly match the mass of the particle they wanted to create. This is called running on **resonance**.

**Would you like to move on to part (b) or do you have questions about 4-vectors and momentum first?**