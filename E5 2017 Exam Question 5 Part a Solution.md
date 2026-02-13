

Welcome to the subatomic microscope! We are leaving the world of nuclear decay and entering the world of **Scattering Physics**.

This is how we discovered almost everything we know about the universe: we smash things together (scatter them) and see how they bounce off. Specifically, this problem is about **Elastic Electron-Nucleon Scattering**, which led to the Nobel Prize-winning discovery that protons and neutrons are not solid balls, but have an internal structure (quarks).

The formula you see, the **Rosenbluth Formula**, is the master key to unlocking that structure.

---

### (a) Fermi's Golden Rule

**The Professor's Insight:**

In quantum mechanics, if you want to know how likely a transition is (like a particle scattering from state A to state B), you use Fermi's Golden Rule. It is the bridge between the abstract wavefunctions and the numbers we measure in the lab.

**The Rule:**

The transition rate $W$ (probability per unit time) is given by:

$$W = \frac{2\pi}{\hbar} |M_{fi}|^2 \rho(E_f)$$

**The Terms:**

1. **$W$ (Transition Rate):** How fast the reaction happens. This relates directly to the Cross-Section ($\sigma$).
    
2. **$|M_{fi}|^2$ (The Matrix Element squared):** This represents the **physics interaction**. It contains the forces (electromagnetic, weak, etc.) and the wavefunctions of the initial ($i$) and final ($f$) states.
    
3. **$\rho(E_f)$ (Density of States):** This represents the **phase space**. It tells you how many available quantum states exist for the particles to go into. (If there's nowhere to go, the reaction can't happen!)
    

---

### (b) Definition and Measurement of $Q^2$

**The Definition:**

$Q^2$ is the **squared four-momentum transfer**.

In relativity, energy and momentum are combined into a four-vector $k = (E/c, \vec{p})$. When the electron bounces off the proton, it exchanges a "virtual photon" carrying momentum $q = k_{initial} - k_{final}$.

We define $Q^2$ as the negative of the square of this transfer (to make it a positive number):

$$Q^2 = - q^2 = - (k_i - k_f)^2$$

**How to Measure it:**

You don't measure "momentum transfer" directly. You measure the geometry of the scattering.

For an electron with initial energy $E$ scattering at an angle $\theta$ to a final energy $E'$, the formula is:

$$Q^2 \approx 4 E E' \sin^2\left(\frac{\theta}{2}\right)$$

**Answer:** Experimentally, $Q^2$ is determined by measuring the **Scattering Angle ($\theta$)** and the electron energies ($E, E'$).

---

### (c) Why are there two Form Factors $G_E(Q^2)$ and $G_M(Q^2)$?

**The Professor's Insight:**

If the proton were a simple, point-like charged dot (like an electron), there would be no "Form Factors" (or rather, they would just be equal to 1). The Rosenbluth formula would reduce to the simpler "Mott Cross Section".

The existence of Form Factors tells us the target has **internal structure**.

**The Reason for Two:**

The nucleon has two distinct electromagnetic properties:

1. **Electric Charge:** Described by the Electric Form Factor, **$G_E(Q^2)$**. This tells us how the charge is spread out in space.
    
2. **Magnetic Moment:** Described by the Magnetic Form Factor, **$G_M(Q^2)$**. This tells us how the magnetization (currents/spin) is spread out.
    

So, we need two functions to describe these two different physical distributions.

---

### (d) How to determine $G_E$ and $G_M$ from the differential cross-section?

**The Professor's Insight:**

Look closely at the Rosenbluth formula again. It has a specific mathematical structure:

$$\text{Cross Section} = A \cdot [ \dots + B \cdot \tan^2(\theta/2) ]$$

Notice that the $\tan^2(\theta/2)$ term is attached _only_ to the magnetic part ($G_M$). This allows us to separate them using a technique called the **Rosenbluth Separation**.

**The Method:**

1. Perform the experiment multiple times.
    
2. Keep $Q^2$ **constant** (by adjusting Beam Energy $E$ and Angle $\theta$ simultaneously).
    
3. Plot the measured cross-section (divided by the Mott term) on the Y-axis vs. $\tan^2(\theta/2)$ on the X-axis.
    
4. Because the formula is linear ($y = mx + b$):
    
    - The **Slope** of the line gives you **$G_M^2$**.
        
    - The **Y-Intercept** helps you find **$G_E^2$**.
        

---

### (e) Conclusions from the Dipole Fit and Neutron Data

**The Data:**

1. $G_E^p(Q^2)$ drops off quickly (Dipole fit) $\rightarrow$ The proton is not a point; it is a "fuzzy" ball of charge with a radius of about $0.8 \text{ fm}$.
    
2. $G_E^n(Q^2) = 0$ $\rightarrow$ The neutron has zero net electric charge (consistent with being neutral).
    
3. **Crucially:** $G_M^p \approx 2.79$ and $G_M^n \approx -1.91$.
    

**The Conclusions:**

- **Anomalous Magnetic Moments:** A point-like Dirac particle (spin 1/2) should have a magnetic moment factor of $g=2$ (so $\mu \approx 1$). The proton is $2.79$ and the neutron is $-1.91$. This huge deviation proves **they are not fundamental particles**.
    
- **Composite Structure:** The fact that the _neutral_ neutron has a huge magnetic moment ($-1.91$) means there are **charged particles moving inside it**! Their charges cancel out to zero ($G_E^n \approx 0$), but their currents create a strong magnetic field.
    
- **Quarks:** This was one of the smoking guns that led to the **Quark Model**. We now know the proton is $(uud)$ and the neutron is $(udd)$. The charged quarks create the magnetic moments.
    

---

### Professor's Closing

You have now walked through the history of the 1950s and 60s!

- **Aufgabe 1 & 2** taught you how to accelerate and detect particles.
    
- **Aufgabe 3 & 4** taught you about the nucleus as a whole.
    
- **Aufgabe 5** taught you how to break the nucleus apart and see the quarks inside.
    

This covers the full scope of your exam sheet. Is there any specific concept (like the Form Factors or the Center-of-Mass energy) you want to double-check before you head off to study?