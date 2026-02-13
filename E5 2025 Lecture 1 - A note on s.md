

[Hello, let's do some particle physics! I'm new to the subject so please explain things in lots of detail. I've seen many collider questions ask about the energy in the center of mass frame. From my understanding, the quantity s is just the squared length of the momentum four-vector. But many of the answers to the questions use strange approximations for s. Could you please explain what these approximations are and where they come from, as well as how to use them? Thank you!]

Hello! Welcome to the fascinating world of particle physics. It is wonderful that you are diving into the kinematics of colliders—this is the foundation for understanding how we discover new particles.

You are absolutely right: the Mandelstam variable $s$ is indeed the squared length of the total four-momentum vector of the colliding particles. However, in high-energy physics (like at the LHC at CERN), we deal with particles moving so fast that their mass becomes negligible compared to their kinetic energy. This leads to the "strange approximations" you've noticed.

Here is a detailed breakdown of where these approximations come from and how to use them.

---

### 1. The Exact Definition of $s$

First, let's look at the rigorous definition without any approximations. In a collision between two particles (Particle 1 and Particle 2), we define the four-momenta as:

- $p_1 = (E_1, \vec{p}_1)$
    
- $p_2 = (E_2, \vec{p}_2)$
    

The variable $s$ is the square of the sum of these vectors:

$$s = (p_1 + p_2)^2$$

If we expand this dot product using the metric signature $(+, -, -, -)$, we get:

$$s = p_1^2 + p_2^2 + 2p_1 \cdot p_2$$

Since the square of a four-momentum is the particle's mass squared ($p^2 = m^2$), this becomes:

$$s = m_1^2 + m_2^2 + 2(E_1 E_2 - \vec{p}_1 \cdot \vec{p}_2 \cos\theta)$$

Where $\theta$ is the angle between the two particle beams. This is the **exact** formula.

---

### 2. The "High Energy" Approximation

In modern particle physics, we usually accelerate particles to speeds extremely close to the speed of light ($c=1$).

When a particle is **ultra-relativistic** (moving very fast), its energy $E$ is much larger than its rest mass $m$ ($E \gg m$). Because of the relationship $E^2 = m^2 + |\vec{p}|^2$, if $m$ is tiny compared to $E$, we can approximate:

$$|\vec{p}| \approx E$$

This implies the particle is essentially behaving like a photon (massless). We use this logic to simplify the formula for $s$ in two main scenarios.

### 3. Scenario A: The Fixed Target Approximation

Imagine you shoot a beam of high-energy particles at a stationary target (like shooting protons into a block of lead).

- **Particle 1 (Beam):** High energy ($E_1 \gg m_1$), so $|\vec{p}_1| \approx E_1$.
    
- **Particle 2 (Target):** At rest, so $\vec{p}_2 = 0$ and $E_2 = m_2$.
    

**The Derivation:**

Using the exact formula:

$$s = m_1^2 + m_2^2 + 2(E_1 m_2 - \vec{p}_1 \cdot 0)$$

$$s = m_1^2 + m_2^2 + 2 E_1 m_2$$

**The Approximation:**

Since the beam energy $E_1$ is massive compared to the particle masses, the terms $m_1^2$ and $m_2^2$ are negligible. We drop them, leaving:

$$s \approx 2 E_{beam} m_{target}$$

> **Key Takeaway:** In a fixed target experiment, the available energy for creating new particles ($\sqrt{s}$) grows only with the **square root** of the beam energy. This is inefficient!

---

### 4. Scenario B: The Collider Approximation (The "Strange" One)

This is what you likely see in collider questions. Here, two beams are fired **head-on** at each other.

- **Particle 1:** Moving right. $E_1 \gg m_1$.
    
- **Particle 2:** Moving left. $E_2 \gg m_2$.
    
- **Angle:** Since they are head-on, the angle is $180^\circ$, so $\cos\theta = -1$.
    

**The Derivation:**

The dot product term $- \vec{p}_1 \cdot \vec{p}_2$ becomes $+ |\vec{p}_1| |\vec{p}_2|$ because of the opposite directions.

$$s = m_1^2 + m_2^2 + 2(E_1 E_2 + |\vec{p}_1| |\vec{p}_2|)$$

**The Approximation:**

1. **Drop the masses:** $m_1$ and $m_2$ are tiny, so ignore $m^2$ terms.
    
2. **Assume $p \approx E$:** Replace momentum with energy.
    

The equation becomes:

$$s \approx 0 + 0 + 2(E_1 E_2 + E_1 E_2)$$

$$s \approx 4 E_1 E_2$$

If the two beams have equal energy ($E_1 = E_2 = E$), which is common in symmetric colliders like the LHC:

$$s \approx 4 E^2$$

$$\sqrt{s} \approx 2E$$

> **Key Takeaway:** In a collider, the available energy $\sqrt{s}$ is simply the sum of the two beam energies ($2E$). You get out exactly what you put in!

---

### Summary of Formulas

|**Scenario**|**Exact Formula**|**Approximation (High Energy)**|
|---|---|---|
|**Fixed Target**|$s = m_1^2 + m_2^2 + 2 E_{beam} m_{target}$|$$s \approx 2 E_{beam} m_{target}$$|
|**Collider (Head-on)**|$s = m_1^2 + m_2^2 + 2(E_1 E_2 +|\vec{p}_1|

### How to use these in questions

When you see a problem, check these three conditions to see if you can use the approximation:

1. **High Energy:** Is the energy given in GeV or TeV while the mass is in MeV? (e.g., a 7 TeV proton which has a mass of only 0.938 GeV). If yes, assume $m \approx 0$.
    
2. **Configuration:** Is it a stationary target or a head-on collision?
    
3. **Result Required:** If you need a rough estimate or scaling behavior, use the approximation. If you need a precision calculation near a threshold (where energy is _barely_ enough to make a particle), use the exact formula.
    

Would you like to try calculating the difference in available energy ($\sqrt{s}$) between a fixed-target setup and a collider setup using a real example, like the protons at the LHC?


[Nice! That clears things up. You said that the square of four-momentum is also the square of the mass. How do we know this? What other useful identities can we extract?]


It is great to hear that the previous explanation helped! The relationship $p^2 = m^2$ is indeed the cornerstone of relativistic kinematics.

Here is the derivation of why that is true, along with the other essential identities ("invariants") that you will constantly use in particle physics problems.

### 1. Why $p^2 = m^2$?

This identity comes directly from the definition of the four-momentum vector and the geometry of spacetime (Special Relativity).

**The Definition**

A four-momentum vector $p^\mu$ describes a particle's motion in spacetime:

$$p^\mu = (E, p_x, p_y, p_z) = (E, \vec{p})$$

_(Note: We are using "natural units" where $c=1$. If we weren't, it would be $(E/c, \vec{p})$)._

**The Dot Product (Lorentz Invariant)**

In standard Euclidean geometry (3D space), the length squared of a vector is $x^2 + y^2 + z^2$. However, in Special Relativity, we use the **Minkowski metric**. The time component contributes positively, and the space components contribute negatively (signature $+---$):

$$p^2 = p^\mu p_\mu = E^2 - (p_x^2 + p_y^2 + p_z^2)$$

$$p^2 = E^2 - |\vec{p}|^2$$

**The Energy-Momentum Relation**

Einstein's full equation for energy is:

$$E^2 = m^2 + |\vec{p}|^2$$

If we rearrange this equation to solve for mass:

$$m^2 = E^2 - |\vec{p}|^2$$

**The Conclusion**

Comparing the dot product and Einstein's equation, we see they are identical:

$$p^2 = m^2$$

> **Why this matters:** This quantity is a **Lorentz Invariant**. No matter how fast you are moving or which reference frame you are in, the "length" of a particle's momentum vector is _always_ its mass. This allows you to evaluate $p^2$ in the frame where the math is easiest (usually the Center of Mass frame or the Rest frame) and know the answer holds true everywhere.

---

### 2. Other Essential Identities

In particle physics questions, you rarely solve for $E$ and $\vec{p}$ individually. Instead, you manipulate these "invariant scalars." Here are the tools you need in your toolkit.

#### A. The Conservation of Four-Momentum

Just like classical energy and momentum, four-momentum is conserved.

$$p_{initial}^\mu = p_{final}^\mu$$

Squaring both sides of this equation is the most common trick in the book:

$$(p_1 + p_2)^2 = (p_3 + p_4)^2$$

#### B. The Mandelstam Variables ($s, t, u$)

You already know $s$. There are two others, $t$ and $u$, which describe momentum transfer. For a scattering process $1 + 2 \rightarrow 3 + 4$:

- **$s$ (Center of Mass Energy squared):**
    
    $$s = (p_1 + p_2)^2 = (p_3 + p_4)^2$$
    
- **$t$ (Four-momentum transfer squared):**
    
    $$t = (p_1 - p_3)^2 = (p_2 - p_4)^2$$
    
    _Useful for understanding how much "kick" particle 1 gave to particle 3._
    
- **$u$ (Cross-momentum transfer squared):**
    
    $$u = (p_1 - p_4)^2 = (p_2 - p_3)^2$$
    

#### C. The Sum Rule (The "Magic" Identity)

This is an incredibly useful identity to check your work. The sum of the Mandelstam variables equals the sum of the masses squared:

$$s + t + u = m_1^2 + m_2^2 + m_3^2 + m_4^2$$

**Proof Sketch:**

Expand the definitions:

$$s = p_1^2 + p_2^2 + 2p_1 p_2$$

$$t = p_1^2 + p_3^2 - 2p_1 p_3$$

$$u = p_1^2 + p_4^2 - 2p_1 p_4$$

Add them up ($s+t+u$) and use conservation of momentum ($p_1 + p_2 = p_3 + p_4$) to show that the cross-terms cancel out, leaving only the $p^2$ terms (which are $m^2$).

#### D. Massless Limits

If you are dealing with photons or ultra-relativistic particles ($m \approx 0$), the identities simplify beautifully:

- $p^2 = 0$ (for photons)
    
- $p_i \cdot p_j \approx \frac{s_{ij}}{2}$ (where $s_{ij}$ is the invariant mass of the pair $i, j$)
    

---

### Summary Table

|**Identity**|**Formula**|**When to use**|
|---|---|---|
|**Invariant Mass**|$p^2 = m^2$|Always true. Converts vectors to scalars.|
|**Conservation**|$p_{in} = p_{out}$|Step 1 of almost every problem.|
|**Sum Rule**|$s+t+u = \sum m_i^2$|To find one variable (e.g., $u$) if you know $s$ and $t$.|
|**Photon**|$p^2 = 0$|When light is involved.|

Would you like to try applying the **Sum Rule** or the **Conservation** square trick to a simple process, like Electron-Positron annihilation ($e^+ e^- \rightarrow \gamma \gamma$)?


[I saw a question once that collided a 7GeV beam of electrons with a 4 GeV beam of positrons. When calculating s, this is the formula that the person used. How does this path fit with the logic you explained earlier?]


This is an excellent find! The formula in your image fits **perfectly** with the logic we discussed, but it is taking a slightly different path to get to the same answer.

The person who wrote that solution is going back to the most fundamental definition of the invariant mass squared:

$$s = (\text{Total Energy})^2 - (\text{Total Momentum Vector})^2$$

Here is the step-by-step breakdown of why their "difference of squares" method ($11^2 - 3^2$) gives the exact same result as the "product" method ($4 E_1 E_2$) I showed you.

### 1. The Logic in the Image

The image text says _"Bei masselosen Elektronen/Positronen"_ (For massless electrons/positrons). This means they are using the approximation where mass is zero, so Momentum ($p$) = Energy ($E$).

They are looking at the **Total System** (the sum of the two particles):

- **Total Energy ($E_{tot}$):** Energy is a scalar, so you always just add them up.
    
    $$E_{tot} = E_1 + E_2 = 7 + 4 = 11 \text{ GeV}$$
    
- **Total Momentum ($\vec{p}_{tot}$):** Momentum is a vector with direction. In a collider, the particles move in **opposite** directions. If the 7 GeV electron is moving right ($+7$), the 4 GeV positron is moving left ($-4$).
    
    $$|\vec{p}_{tot}| = |p_1 - p_2| = |7 - 4| = 3 \text{ GeV}$$
    
    _(Note: The system is not stationary! It has a net drift of 3 GeV to the right)._
    

Now, they apply the fundamental definition of Lorentz invariant mass squared ($s = E^2 - p^2$) to the _whole system_:

$$s = (E_{tot})^2 - (p_{tot})^2$$

$$s = (11)^2 - (3)^2$$

$$s = 121 - 9 = 112 \text{ GeV}^2$$

Finally, they take the square root to get the energy in the center of mass:

$$\sqrt{s} = \sqrt{112} \approx 10.583 \text{ GeV}$$

### 2. Connecting it to my formula ($4E_1 E_2$)

Let's see if this matches the collider approximation I gave you earlier: $s \approx 4 E_1 E_2$.

$$s \approx 4 \cdot (7 \text{ GeV}) \cdot (4 \text{ GeV})$$

$$s \approx 112 \text{ GeV}^2$$

It matches exactly!

**The Mathematical Proof**

You can actually prove these two methods are identical using simple algebra.

$$s = (E_1 + E_2)^2 - (E_1 - E_2)^2$$

Expand the squares:

$$s = (E_1^2 + 2E_1E_2 + E_2^2) - (E_1^2 - 2E_1E_2 + E_2^2)$$

The $E_1^2$ and $E_2^2$ terms cancel out, leaving:

$$s = 2E_1E_2 - (-2E_1E_2) = 4E_1E_2$$

### Which one should you use?

Both are correct, but they are useful in different situations:

- **Use the Image's Method ($E_{tot}^2 - p_{tot}^2$)** when you want to stick to the fundamental definition. It helps remind you that the center-of-mass frame is just the frame where the total momentum is zero.
    
- **Use the Approximation ($4E_1 E_2$)** when you want to be fast. It is the standard "quick check" formula in collider physics.
    

**Key Takeaway:** The "strange approximation" in the image is actually just a very literal application of $p^2 = m^2$ applied to the total system vector! They calculated the "mass" of the collision itself.