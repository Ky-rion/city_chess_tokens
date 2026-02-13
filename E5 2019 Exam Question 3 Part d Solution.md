

![[Pasted image 20260209163637.png]]

You were right to suspect the magnetic field would come back! In **Part (d)**, we are finally using that **1.5 Tesla** magnetic field mentioned in the very first paragraph.

This part asks us to calculate the **maximum radius** of the path the muon takes. This is crucial for designing the detector: if the particle curves too much or too little, the detector might miss it or fail to measure its momentum accurately.

### 1. The Physics: Decay at Rest

We are looking at this specific decay:

$$B^+ \rightarrow \mu^+ + \nu_\mu$$

(A B-meson decays into a Muon and a Neutrino).

The problem tells us to assume:

1. **The B-meson is at rest** (just like in the previous parts).
    
2. **The Muon ($\mu$) and Neutrino ($\nu$) are massless.**
    
3. **Conservation of Momentum and Energy applies.**
    

**How much momentum does the muon get?**

Imagine the B-meson as a bomb that explodes into two equal pieces. Since the pieces are "massless" (extremely light compared to the parent), all the mass energy of the parent ($m_B$) is converted into the kinetic energy of the two daughters.

$$E_{parent} = E_{\mu} + E_{\nu}$$

$$m_B c^2 = p c + p c$$

(Since they fly apart back-to-back with equal momentum $p$).

So:

$$m_B = 2p$$

$$p = \frac{m_B}{2}$$

Using the mass of the B-meson ($5.28 \text{ GeV}/c^2$):

$$p_{\mu} = \frac{5.28}{2} = \mathbf{2.64 \text{ GeV}/c}$$

This is the total momentum of the muon.

---

### 2. Transverse Momentum & Frame Invariance

The question asks for the radius in the **plane perpendicular to the beam axis**.

The magnetic field points along the beam axis (let's call it the $z$-direction). The magnetic force only bends particles based on their velocity **perpendicular** to the field lines. This is called **Transverse Momentum ($p_T$)**.

**Why is this cool?**

The "boost" (the movement of the whole system through the lab) is _also_ along the beam axis ($z$).

According to Special Relativity, a boost along the $z$-axis changes the momentum in the $z$-direction ($p_z$), but **it leaves the perpendicular momentum ($p_x, p_y$) completely unchanged!**

$$p_{T, \text{Lab}} = p_{T, \text{CMS}}$$

So, we don't need to do any complicated Lorentz transformations here. The maximum transverse momentum in the Lab is the same as in the Center-of-Mass.

**What is the Maximum $p_T$?**

The muon has total momentum $p = 2.64 \text{ GeV}/c$.

- If it shoots out parallel to the beam, $p_T = 0$ (no bending).
    
- If it shoots out **perpendicular** to the beam ($90^\circ$), all of its momentum is transverse.
    

So, the maximum transverse momentum is simply the total momentum we just calculated:

$$p_{T, max} = 2.64 \text{ GeV}/c$$

---

### 3. The "Golden Rule" of Particle Physics

Now we calculate the radius ($R$).

The standard physics formula for a charged particle circling in a magnetic field is:

$$p = q B R$$

(where $q$ is charge, $B$ is magnetic field, $R$ is radius).

However, particle physicists use a practical "shortcut" version of this formula that handles the units ($\text{GeV}$, $\text{Tesla}$, $\text{meters}$) automatically. You will see this written in the solution as:

$$p [\text{GeV}/c] = 0.3 \times B [\text{Tesla}] \times R [\text{meters}]$$

_(Note: The "0.3" comes from the speed of light $c \approx 3 \times 10^8$.)_

### 4. The Calculation

We need to solve for $R$:

$$R = \frac{p}{0.3 \times B}$$

Plug in our values:

- $p = 2.64 \text{ GeV}/c$
    
- $B = 1.5 \text{ Tesla}$
    

$$R = \frac{2.64}{0.3 \times 1.5}$$

$$R = \frac{2.64}{0.45}$$

$$R \approx \mathbf{5.87 \text{ meters}}$$

### Summary

The solution matches perfectly ($5.87 \text{ m}$).

**What does this mean for the experiment?**

A radius of nearly 6 meters is huge! The Belle-II detector is big, but not _that_ big. This means the muon won't spiral in little loops inside the detector. Instead, it will fly through the detector in a stiff, slightly curved arc. The scientists measure this slight curvature to determine the momentum.

And that concludes the problem sheet! We went from colliding electrons, to creating mesons, to watching them decay, to tracking their daughters in a magnetic field.

**Do you have any final questions on how these parts fit together, or should we wrap up this topic?**