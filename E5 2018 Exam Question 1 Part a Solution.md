

Welcome back to "class"! This is a classic problem in High Energy Physics. It illustrates the fundamental reason why modern physicists build giant colliders (like the LHC or LEP) rather than just shooting beams at stationary targets.

We are going to compare two methods of making $B$-meson pairs: a **Collider** (crashing two cars head-on) and a **Fixed Target** (crashing a speeding car into a parked one).

Here are the constants we will use from the text:

- Mass of $B$-meson ($m_B$) $= 5.28 \text{ GeV}/c^2$
    
- Lifetime ($\tau_B$) $= 1.64 \text{ ps} = 1.64 \times 10^{-12} \text{ s}$
    
- Mass of Electron/Positron ($m_e$): Not given in the text, but **crucial** for part (d). In physics exams, you are expected to know $m_e \approx 0.511 \text{ MeV}/c^2 = 0.000511 \text{ GeV}/c^2$.
    

---

### (a) The Minimum Center-of-Mass Energy ($E_{cm}$)

**Concept:** To create new particles, we need energy. The most efficient way to create particles is to have just enough energy to make their mass, with nothing left over for movement (kinetic energy). This is called the "Threshold Energy."

At the threshold, the two resulting particles ($B^+$ and $B^-$) are produced at rest **in the center-of-mass frame**.

$$E_{cm} = (\text{Mass of products}) \times c^2$$

$$E_{cm} = m_{B^+} + m_{B^-} = 2 \cdot m_B$$

**Calculation:**

$$E_{cm} = 2 \cdot 5.28 \text{ GeV} = 10.56 \text{ GeV}$$

> **Answer:** The minimum center-of-mass energy required is **10.56 GeV**.

---

### (b) Collider Experiment: Minimum Beam Energy

**Concept:** In a symmetric collider (electron vs. positron with equal energy), the laboratory frame **is** the center-of-mass frame. They hit head-on, so their net momentum is zero.

$$E_{cm} = E_{beam, 1} + E_{beam, 2}$$

Since both beams have equal energy $E_{beam}$:

$$E_{cm} = 2 \cdot E_{beam}$$

**Calculation:**

We know $E_{cm} = 10.56 \text{ GeV}$ from part (a).

$$10.56 \text{ GeV} = 2 \cdot E_{beam}$$

$$E_{beam} = 5.28 \text{ GeV}$$

> **Answer:** Each beam must have an energy of **5.28 GeV**.

---

### (c) Flight Distance in Collider (Case b)

**Concept:** This is a bit of a trick question to test your understanding of "threshold" energy.

In part (b), we calculated the _minimum_ energy. At this exact minimum, all the energy goes into creating the mass of the $B$ mesons ($E=mc^2$). There is **zero energy left over** for kinetic energy (motion).

In the collider frame, at the exact threshold, the particles are created **at rest**. They have velocity $v=0$.

$$Distance = v \cdot \text{lifetime} = 0$$

_(Note: In a real experiment, you would accelerate them slightly above the minimum so they move away from the interaction point, but technically, at the theoretical minimum, they don't move.)_

> **Answer:** At the minimum energy, the $B^+$ is produced at rest, so the flight distance is **0 m**.

---

### (d) Fixed Target Experiment: Minimum Beam Energy

**Concept:** This is where things get wild! Now we are shooting a positron at a stationary electron ($E_{electron} = m_e$).

Much of the beam's energy is "wasted" just to conserve the forward momentum of the collision. It cannot all go into making mass.

We use the **Invariant Mass** formula squared ($s$):

$$s = E_{cm}^2 \approx 2 \cdot E_{beam} \cdot m_{target}$$

_(This is an approximation where we ignore the tiny mass of the beam particle compared to its huge energy, which is standard in high-energy physics)._

We need the available energy ($\sqrt{s}$) to equal the mass of the two B-mesons ($10.56 \text{ GeV}$).

**Calculation:**

1. **Required $s$**: $(10.56 \text{ GeV})^2 = 111.51 \text{ GeV}^2$
    
2. **Target Mass ($m_e$)**: $0.000511 \text{ GeV}$
    
3. **Solve for Beam Energy**:
    
    $$s = 2 \cdot E_{beam} \cdot m_e$$
    
    $$111.51 = 2 \cdot E_{beam} \cdot 0.000511$$
    
    $$E_{beam} = \frac{111.51}{2 \cdot 0.000511}$$
    
    $$E_{beam} \approx 109,110 \text{ GeV}$$
    

**Professor's Insight:** Look at that difference! In the collider, we only needed **5.28 GeV**. In the fixed target, we need over **100,000 GeV** (or roughly 109 TeV) to do the exact same thing. This is because the electron target is so light that it easily recoils, "stealing" almost all the energy as kinetic energy.

> **Answer:** The positron beam requires an energy of approx **109,110 GeV (or 109 TeV)**.

---

### (e) Flight Distance in Fixed Target (Case d)

**Concept:** Because we had to pump in so much energy (109 TeV), the resulting $B$ mesons are moving incredibly fast in the lab frame! We must account for **Time Dilation**.

The $B$ mesons act as a single unit moving with the center of mass. We need to find the **Lorentz Factor ($\gamma$)** of the system.

**Step 1: Calculate $\gamma$**

The total energy in the lab is roughly the beam energy ($109,110 \text{ GeV}$). The mass of the "object" moving (the two B mesons) is $10.56 \text{ GeV}$.

$$\gamma = \frac{E_{total, lab}}{Mass_{total}} = \frac{109,110}{10.56} \approx 10,332$$

**Step 2: Time Dilation**

The particle lives for $\tau = 1.64 \text{ ps}$ in its own frame. In the lab, it lives $\gamma$ times longer.

$$\tau_{lab} = \gamma \cdot \tau$$

$$\tau_{lab} = 10,332 \cdot (1.64 \times 10^{-12} \text{ s}) \approx 1.69 \times 10^{-8} \text{ s}$$

**Step 3: Calculate Distance**

At these energies, the speed is essentially the speed of light ($v \approx c$).

$$Distance = c \cdot \tau_{lab}$$

$$d = (3 \times 10^8 \text{ m/s}) \cdot (1.69 \times 10^{-8} \text{ s})$$

$$d \approx 5.07 \text{ meters}$$

> **Answer:** due to relativistic time dilation, the $B^+$ meson flies approximately **5.07 meters** before decaying.

---

### Summary Table

|**Feature**|**Collider (a, b, c)**|**Fixed Target (d, e)**|
|---|---|---|
|**Energy needed from Machine**|**5.28 GeV** (Efficient)|**~109,110 GeV** (Inefficient)|
|**Product Velocity**|0 (At rest)|$\approx c$ (Speed of light)|
|**Decay Distance**|0 meters|~5 meters|

This shows why we use **Colliders** to discover heavy particles (energy efficiency) but **Fixed Target** experiments if we want the particles to live long enough in the lab to study their tracks (flight distance)!