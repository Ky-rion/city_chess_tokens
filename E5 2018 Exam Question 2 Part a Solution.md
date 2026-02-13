

This is a wonderful problem! It’s what we call a classic "Particle Identification" (or **PID**) task. In experimental physics, we never just "know" what a particle is; we have to play detective, collecting clues like momentum, velocity, and charge to build a profile.

Let's break down the clues we have from your problem statement:

- **Charge ($z$):** "Singly charged" (usually means $q = \pm 1e$).
    
- **Momentum ($p$):** $1.25 \text{ GeV}/c$.
    
- **Magnetic Field ($B$):** $1.2 \text{ T}$.
    
- **Flight Distance ($s$):** $1.8 \text{ m}$.
    
- **Flight Time ($t$):** $7.5 \text{ ns}$.
    
- **Refractive Index ($n$):** $1.3$.
    

Now, let's solve this step-by-step.

---

### (a) Radius of Curvature ($R$)

**The Physics:**

When a charged particle flies through a magnetic field, the Lorentz force bends its path into a circle. There is a very famous "Rule of Thumb" formula in high-energy physics that relates Momentum ($p$), Magnetic Field ($B$), and Radius ($R$).

The formula is derived from balancing centripetal force and Lorentz force ($mv^2/R = qvB$), but in "natural units" (GeV, Tesla, Meters), it simplifies to:

$$p [\text{GeV}/c] = 0.3 \cdot z \cdot B [\text{T}] \cdot R [\text{m}]$$

**The Calculation:**

We need to solve for $R$:

$$R = \frac{p}{0.3 \cdot z \cdot B}$$

Substituting our values ($z=1$ because it is singly charged):

$$R = \frac{1.25}{0.3 \cdot 1 \cdot 1.2}$$

$$R = \frac{1.25}{0.36}$$

$$R \approx 3.47 \text{ meters}$$

> **Answer:** The curvature radius of the track is approximately **3.47 m**.

---

### (b) Mass and Identity

**The Physics:**

To find the mass, we need two things: **Momentum** (which we have) and **Velocity** (which we can calculate from distance and time). Once we have those, we use Special Relativity to find the mass.

**Step 1: Calculate Velocity ($\beta$)**

$$v = \frac{s}{t} = \frac{1.8 \text{ m}}{7.5 \times 10^{-9} \text{ s}} = 2.4 \times 10^8 \text{ m/s}$$

Now, let's express this as a fraction of the speed of light ($\beta = v/c$):

$$\beta = \frac{2.4 \times 10^8}{3.0 \times 10^8} = 0.8$$

So, the particle is traveling at **80% the speed of light**.

**Step 2: Calculate the Lorentz Factor ($\gamma$)**

We need $\gamma$ to link momentum and mass.

$$\gamma = \frac{1}{\sqrt{1 - \beta^2}} = \frac{1}{\sqrt{1 - 0.8^2}} = \frac{1}{\sqrt{0.36}} = \frac{1}{0.6} = \frac{5}{3} \approx 1.67$$

**Step 3: Calculate Mass ($m$)**

The definition of relativistic momentum is $p = \gamma m v$. We can rearrange this to solve for mass (using units of $\text{GeV}/c^2$):

$$m = \frac{p}{\gamma \cdot \beta \cdot c}$$

_(Note: Since we usually work in natural units where $c=1$, the formula is effectively $m = p / (\gamma \beta)$)_.

$$m = \frac{1.25 \text{ GeV}/c^2}{1.667 \times 0.8}$$

$$m = \frac{1.25}{1.333} \approx 0.938 \text{ GeV}/c^2$$

**Identification:**

A mass of $0.938 \text{ GeV}/c^2$ (or $938 \text{ MeV}/c^2$) corresponds exactly to the mass of a **Proton**.

> **Answer:** The mass is **0.938 GeV/c²**. Ideally, this is a **Proton**.

---

### (c) Particle vs. Antiparticle

**The Physics:**

We know the magnitude of the charge is $1$, but is it $+1$ (proton) or $-1$ (antiproton)?

In a magnetic field, the direction of the Lorentz Force depends on the sign of the charge ($F = q(\vec{v} \times \vec{B})$).

- A positive particle curves one way (e.g., clockwise).
    
- A negative particle curves the opposite way (e.g., counter-clockwise).
    

> **Answer:** You can distinguish them by observing the **direction of curvature** (left or right) relative to the magnetic field direction. Since we know it's a proton (positive), it will curve in the direction opposite to that of an electron.

---

### (d) Cherenkov Light

**The Physics:**

Cherenkov radiation is like a "sonic boom" for light. It happens when a particle travels through a medium faster than light can travel through that same medium.

- Speed of light in vacuum: $c$
    
- Speed of light in medium: $c_{medium} = c / n$
    

**Step 1: The Condition**

Does the particle produce light?

- Particle speed: $v = 0.8c$
    
- Threshold speed: $c_{medium} = c / 1.3 \approx 0.77c$
    

Since $0.8c > 0.77c$, **Yes**, the particle is moving faster than light in the detector, so it produces Cherenkov radiation.

**Step 2: The Angle ($\theta_c$)**

The formula for the emission angle is:

$$\cos(\theta_c) = \frac{1}{\beta n}$$

$$\cos(\theta_c) = \frac{1}{0.8 \times 1.3} = \frac{1}{1.04} \approx 0.9615$$

Now, take the inverse cosine:

$$\theta_c = \arccos(0.9615) \approx 16.3^\circ$$

> **Answer:** **Yes**, it produces Cherenkov light. The radiation is emitted at an angle of approximately **16.3°** relative to the flight path.

---

### (e) Further Measurement

**The Physics:**

Even though we are pretty sure it's a proton, experimentalists love to be double-sure. What else can we measure?

The most common "partner" to momentum measurement in a tracking chamber is **Specific Energy Loss ($dE/dx$)**.

As charged particles fly through gas (like in the spurkammer/tracking chamber), they ionize the gas atoms and lose energy. The rate of this energy loss is described by the **Bethe-Bloch formula**.

Different particles (protons, pions, kaons) have distinct $dE/dx$ curves for a given momentum. By measuring how much ionization the particle leaves behind, we can confirm if it lies on the "proton curve."

> **Answer:** One could measure the **specific energy loss ($dE/dx$)** of the particle as it traverses the tracking chamber.

---

### Summary for your notes:

- **(a)** $R \approx 3.47$ m
    
- **(b)** $m \approx 0.938$ GeV/$c^2$ (Proton)
    
- **(c)** Check curvature direction.
    
- **(d)** Yes, at $\approx 16^\circ$.
    
- **(e)** Measure $dE/dx$ (ionization energy loss).
    

Would you like to try calculating the angle if the particle had been a Kaon (mass ~0.49 GeV) instead? It's good practice!