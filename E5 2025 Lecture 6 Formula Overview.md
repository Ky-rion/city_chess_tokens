

Class is back in session! We have moved from identifying particles to the machines that make them go fast: **Accelerators**. Specifically, we are looking at the **Synchrotron**, which is the gold standard for high-energy physics.

In an exam, your professor will likely ask you how to design these machines or why we choose circular paths over linear ones. Here is the breakdown.

---

## 1. Resolution and De Broglie Wavelength

$$\Delta x \approx \frac{\lambda}{2} \quad \text{where} \quad \lambda = \frac{h}{p} = \frac{hc}{\beta E}$$

Before we accelerate anything, we need to know why. In particle physics, "higher energy" means "smaller ruler."

- **$\Delta x$:** The resolution (the smallest structure you can see).
    
- **$\lambda$:** The de Broglie wavelength. To "see" inside a proton, your wavelength must be smaller than the proton itself.
    
- **$p$ and $E$:** Momentum and Energy.
    

**Exam Question:** "Why do we need TeV-scale energies to study the Higgs boson?"

**How to answer:** Because according to $\Delta x \approx \lambda/2$, as energy ($E$) increases, the wavelength ($\lambda$) decreases. This allows us to probe incredibly small distance scales where these particles exist.

---

## 2. Acceleration via Potential Difference

$$\Delta E = q \cdot \Delta U$$

This is the simplest way to gain energy. You drop a charged particle through an electric field.

- **$\Delta E$:** The kinetic energy gained.
    
- **$q$:** The charge of the particle (e.g., $1e$ for a proton).
    
- **$\Delta U$:** The voltage (potential difference).
    

**Exam Question:** "If an electron passes through a 10 million volt gap, what is its energy?"

**How to answer:** It gains $10 \text{ MeV}$ (mega-electronvolts). Note that in circular accelerators, particles pass through these "gaps" thousands of times to reach GeV or TeV levels.

---

## 3. Synchrotron Design Principle

$$R = \frac{p}{qB} \equiv \text{const} \quad \rightarrow \quad B \sim p \sim \gamma$$

In a **Synchrotron**, we want the particle to stay in a ring of a fixed size ($R$) as it gets faster.

- **$R$:** Radius of the ring (constant).
    
- **$B$:** Magnetic field strength.
    
- **$\gamma$:** The Lorentz factor (related to speed).
    

**Exam Question:** "As a particle gains momentum ($p$) in a synchrotron, what must happen to the magnetic field ($B$)?"

**How to answer:** Since $R$ is constant, the magnetic field must increase in perfect synchronization with the particle's momentum ($B \sim p$). This is why it’s called a "synchro"-tron.

---

## 4. Synchrotron Radiation (The "Energy Tax")

$$\Delta E \sim \frac{e^2}{R} \left( \frac{E}{mc^2} \right)^4 = \frac{e^2}{R} \gamma^4$$

This is the biggest hurdle in accelerator physics. Whenever a charged particle is forced into a curve, it "screams" out energy in the form of light (X-rays).

- **$\Delta E$:** Energy lost per single lap (Umlauf).
    
- **$m$:** The mass of the particle.
    
- **$\gamma^4$:** This is the killer. The energy loss increases with the **fourth power** of the energy.
    

**Exam Question:** "Why do we use protons instead of electrons for the world's largest circular accelerators (like the LHC)?"

**How to answer:** Electrons are much lighter than protons. Because $m$ is in the denominator, an electron at the same energy ($E$) loses vastly more energy to radiation than a proton. This makes circular electron accelerators extremely inefficient at high energies.

---

## 5. The Engineering Formula for Energy Loss

$$\Delta E \approx 88.5 \text{ keV} \frac{(E[\text{GeV}])^4}{R[\text{m}]}$$

This is the "plug-and-play" version of the previous formula, specifically for **electrons**.

- **$E$:** Energy in Giga-electronvolts ($GeV$).
    
- **$R$:** Radius in meters ($m$).
    

**Exam Question:** "Calculate the energy loss per turn for a $50 \text{ GeV}$ electron in a ring with a $1000 \text{ m}$ radius."

**How to answer:** $\Delta E = 88.5 \cdot (50^4 / 1000) \approx 553,000 \text{ keV}$ or $553 \text{ MeV}$ per lap. The accelerator's power supply must replace this lost energy every single turn just to keep the particle moving!

---

**Summary for your exam:**

- **Higher Energy** = Smaller wavelength = Better resolution.
    
- **Circular Path** requires $B$ fields to ramp up with $p$.
    
- **Radiation Loss** is the main reason we build bigger rings (large $R$) and use heavier particles (protons).
    

**Would you like to try a "design challenge" where we figure out how large a ring we'd need to keep radiation losses manageable?**