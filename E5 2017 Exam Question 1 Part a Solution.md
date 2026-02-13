

Welcome to Particle Physics 101! I am delighted to be your guide. This problem sheet is a fantastic introduction because it touches on the fundamental pillars of our field: relativity, collision kinematics, accelerator design, and quantum interactions.

You have a problem about a **Muon Collider**. This is very cutting-edge! Scientists are currently debating building one of these because muons (heavy cousins of electrons) have some distinct advantages over protons or electrons, which we will discover as we solve this.

Here is the translation of the problem setup so we are on the same page:

> **Scenario:** A theoretical collider smashes **Muons** ($\mu^-$) with energy $300\text{ GeV}$ into **Anti-Muons** ($\mu^+$) with energy $100\text{ GeV}$.
> 
> **Result:** A Top/Anti-Top quark pair ($t\bar{t}$) is created.
> 
> **Constants:**
> 
> - Mass of Muon ($m_\mu$) = $105\text{ MeV}/c^2$
>     
> - Mass of Electron ($m_e$) = $0.511\text{ MeV}/c^2$
>     
> - Mass of Top Quark ($m_t$) = $173.1\text{ GeV}/c^2$
>     

Let's solve this step-by-step.

---

### (a) How high is the Center-of-Mass Energy?

**The Professor's Insight:**

In particle physics, the "useful" energy for creating new particles isn't just the sum of the beam energies ($300 + 100 = 400$). Because the beams have different momenta, the collision center is moving. We need the "Center-of-Mass" energy ($\sqrt{s}$), which represents the energy available _if you were standing at the point where they collide head-on_.

**The Calculation:**

For highly relativistic particles (where Energy $\gg$ Mass), we can approximate their momentum $p \approx E$. The formula for the center-of-mass energy squared ($s$) in a collider with opposite beams is:

$$s \approx 4 E_1 E_2$$

Where:

- $E_1 = 300\text{ GeV}$
    
- $E_2 = 100\text{ GeV}$
    

$$s = 4 \cdot (300\text{ GeV}) \cdot (100\text{ GeV}) = 120,000\text{ GeV}^2$$

To get the energy ($\sqrt{s}$):

$$\sqrt{s} = \sqrt{120,000} \approx \mathbf{346.41\text{ GeV}}$$

> **Physics Note:** Notice that the simple sum is $400\text{ GeV}$, but the useful collision energy is only $\approx 346\text{ GeV}$. The "missing" energy is actually kinetic energy of the whole system moving through the lab!

---

### (b) What is the momentum magnitude of the Top-Quark in the Center-of-Mass system?

**The Professor's Insight:**

We just calculated that we have $346.41\text{ GeV}$ of available energy in the collision center. We are creating a pair of Top quarks ($t$ and $\bar{t}$).

In the Center-of-Mass (CoM) frame, these two quarks fly apart back-to-back with equal energy.

**The Calculation:**

First, how much energy does _each_ Top quark get? Since they share the total energy equally:

$$E_{top} = \frac{\sqrt{s}}{2} = \frac{346.41}{2} = 173.205\text{ GeV}$$

Now, we use the most famous equation in particle physics (the full version of $E=mc^2$):

$$E^2 = (pc)^2 + (mc^2)^2$$

Rearranging for momentum ($p$):

$$p = \sqrt{E_{top}^2 - m_t^2}$$

We know the Top quark mass $m_t = 173.1\text{ GeV}/c^2$.

$$p = \sqrt{(173.205)^2 - (173.1)^2}$$

$$p = \sqrt{29999.97 - 29963.61}$$

$$p = \sqrt{36.36} \approx \mathbf{6.03\text{ GeV}/c}$$

> **Observation:** Look closely at $E_{top}$ ($173.2\text{ GeV}$) vs the mass ($173.1\text{ GeV}$). We are _barely_ above the threshold to create these particles! They will be moving very slowly (non-relativistically) compared to the muons.

---

### (c) With what velocity $\beta = v/c$ does the $t\bar{t}$-system move relative to the Lab system?

**The Professor's Insight:**

Because one beam is pushing harder ($300\text{ GeV}$) than the other ($100\text{ GeV}$), the resulting debris (the $t\bar{t}$ system) will slide through the laboratory in the direction of the stronger beam. We measure speed in physics as $\beta$ (fraction of light speed).

**The Calculation:**

The velocity of the center of mass is the total momentum divided by the total energy.

$$\beta = \frac{cp_{total}}{E_{total}}$$

Since the beams are head-on (opposite directions), we subtract their momenta:

$$cp_{total} \approx E_1 - E_2 = 300 - 100 = 200\text{ GeV}$$

$$E_{total} = E_1 + E_2 = 300 + 100 = 400\text{ GeV}$$

$$\beta = \frac{200}{400} = \mathbf{0.5}$$

**Answer:** The system moves at **0.5c** (half the speed of light) relative to the lab.

---

### (d) Minimum radius of the accelerator (Max B-field = 10 T)?

**The Professor's Insight:**

To keep particles moving in a circle, we use powerful magnets. The higher the momentum, the stronger the magnets (or larger the ring) needed. We must design the ring for the "stiffest" beam, which is the $300\text{ GeV}$ muon beam.

**The Calculation:**

The formula balancing magnetic force and centripetal force is:

$$p = q \cdot B \cdot R$$

There is a very handy "Rule of Thumb" version of this formula for particle physicists using standard units (GeV, Tesla, meters):

$$p [\text{GeV}/c] = 0.3 \cdot B [\text{T}] \cdot R [\text{m}]$$

Rearranging for Radius ($R$):

$$R = \frac{p}{0.3 \cdot B}$$

Using $p = 300\text{ GeV}/c$ and $B = 10\text{ T}$:

$$R = \frac{300}{0.3 \cdot 10} = \frac{300}{3} = \mathbf{100\text{ meters}}$$

---

### (e) Energy loss via Synchrotron Radiation (Muons vs Electrons)?

**The Professor's Insight:**

This is the **crucial** reason why we want a Muon collider!

When charged particles run in circles, they "scream" out energy in the form of light (X-rays). This is called Synchrotron Radiation.

The amount of energy they lose per lap ($\Delta E$) depends heavily on their mass. Lighter particles (like electrons) lose a massive amount of energy; heavier particles (like muons) lose very little.

**The Calculation:**

The formula for energy loss scales as the inverse of mass to the fourth power:

$$\Delta E \propto \frac{1}{m^4}$$

To find the ratio of Muon loss to Electron loss (assuming same energy and radius):

$$\text{Ratio} = \frac{\Delta E_\mu}{\Delta E_e} = \left( \frac{m_e}{m_\mu} \right)^4$$

- $m_e = 0.511\text{ MeV}$
    
- $m_\mu = 105\text{ MeV}$
    

$$\text{Ratio} = \left( \frac{0.511}{105} \right)^4 \approx (0.004866)^4$$

$$\text{Ratio} \approx \mathbf{5.6 \times 10^{-10}}$$

**Interpretation:** Muons lose almost **zero** energy compared to electrons. This allows us to accelerate them to incredibly high energies in circular rings without wasting all our power battling radiation loss!

---

### (f) Through which interactions can the reaction $\mu^- \mu^+ \rightarrow t \bar{t}$ take place? (Name at least two)

**The Professor's Insight:**

We need to look at the forces of nature. We are annihilating leptons ($\mu$) to create quarks ($t$).

1. **Strong Force:** No. Leptons (muons) do not feel the strong force.
    
2. **Electromagnetic Force:** Yes! The muon and antimuon can annihilate into a **Photon ($\gamma$)**, which then turns into the quark pair.
    
3. **Weak Force:** Yes! They can annihilate into a **Z Boson ($Z^0$)**, which then decays into the quark pair.
    

**Answer:**

The reaction can proceed via:

1. **Electromagnetic Interaction** (exchange of a photon, $\gamma$)
    
2. **Weak Interaction** (exchange of a Z boson, $Z^0$)
    
    _(Bonus: It is theoretically possible via the Higgs Boson ($H$), though the coupling to muons is very small)._
    

---

### Professor's Summary for the Student

You've just analyzed a machine that could be the future of physics!

1. You calculated that a "lopsided" collision ($300$ vs $100$) still gives you enough energy ($\approx 346\text{ GeV}$) to create the heaviest known particle, the Top quark.
    
2. You proved that Muons are superior to electrons for circular rings because they are heavier and don't radiate away their energy ($m^{-4}$ scaling).
    

**Would you like me to explain more about why the Top quark is so special, or how we actually detect these particles once they are created?**