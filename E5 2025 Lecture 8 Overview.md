

https://gemini.google.com/share/01b62884e156


Hello there! Welcome to "office hours." It is wonderful to see a student showing such initiative. Deep Inelastic Scattering (DIS) is actually one of my favorite topics because it is historically how we "broke" the proton and discovered that it wasn't a solid ball, but a bag of smaller particles (quarks).

Think of this topic as **Rutherford Scattering 2.0**. In 1911, Rutherford shot alpha particles at gold atoms to find the nucleus. In the late 1960s (at SLAC), we shot high-energy electrons at protons to find the **quarks**.

Here is your comprehensive overview based on the lecture notes, broken down into the concepts you will likely face on your exam.

---

### 1. The Setup: What is Deep Inelastic Scattering?

In this process, we fire a high-energy electron ($e^-$) at a proton ($P$).

- **Elastic Scattering:** The proton stays intact (bounces off).
    
- **Inelastic Scattering:** The proton breaks apart into a new state with a higher mass (resonances like the $\Delta$ baryon).
    
- **Deep Inelastic Scattering (DIS):** We hit the proton _so_ hard ($Q^2$ is very large) that we don't just excite it; we probe its internal structure. The proton breaks into a messy shower of particles (hadronic state $X$).
    

**The Interaction Diagram:**

The electron emits a virtual photon ($\gamma$), which hits the proton.

- $k$: Initial electron momentum.
    
- $k'$: Final electron momentum.
    
- $q$: The momentum transferred by the photon ($q = k - k'$).
    
- $P$: Initial proton momentum.
    

---

### 2. The Vocabulary: Kinematic Variables

For the exam, you **must** memorize these variables. They are the language of DIS.

#### A. The "Resolution": $Q^2$

$$Q^2 = -q^2 = -(k - k')^2$$

This is the **squared momentum transfer**. In simple terms, $Q^2$ tells you how "hard" you hit the proton.

- By the uncertainty principle, high momentum transfer corresponds to a small wavelength.
    
- **High $Q^2$ = High Resolution microscope.** It allows us to "see" very small things inside the proton.
    

#### B. The Energy Transfer: $\nu$ ("Nu")

$$\nu = \frac{P \cdot q}{M} = E - E'$$

This is the energy lost by the electron in the lab frame ($E$ is initial energy, $E'$ is final energy). It tells us how much energy was dumped into the proton.

#### C. The Invariant Mass: $W$

$W$ is the mass of the final hadronic system (the debris created after the collision).

- **Elastic:** $W = M$ (mass of the proton).
    
- **Inelastic:** $W > M$ (the proton broke up).
    

#### D. The Bjorken Variables (Crucial!)

To make sense of the data, we switch to dimensionless variables.

1. **Bjorken-$x$ ($x$):**
    
    $$x = \frac{Q^2}{2 P \cdot q} = \frac{Q^2}{2 M \nu}$$
    
    - **Range:** $0 \le x \le 1$.
        
    - **Physical Meaning:** If the proton is made of point-like particles (partons), $x$ is the **fraction of the proton's momentum** carried by the struck parton.
        
    - $x=1$ implies elastic scattering (the whole proton was hit).
        
2. **Bjorken-$y$ ($y$):**
    
    $$y = \frac{P \cdot q}{P \cdot k} = \frac{\nu}{E}$$
    
    - **Range:** $0 \le y \le 1$.
        
    - **Physical Meaning:** The fraction of the electron's energy transferred to the proton in the lab frame (inelasticity).
        

---

### 3. The Evidence: What do the plots tell us?

Your notes show several key plots that serve as experimental proof for quarks.

#### Plot 1: The Spectrum

This plot shows the cross-section (probability of scattering) vs. $W$ (invariant mass).

- You see the **Elastic Peak** (sharp spike at $W=M_p$).
    
- You see **Resonances** (bumps) corresponding to excited states like $\Delta(1232)$.
    
- As $W$ gets higher, you enter the smooth "continuum." This is the Deep Inelastic region. The fact that we see scattering here suggests the proton has an internal structure.
    

#### Plot 2: Bjorken Scaling

This is the "smoking gun." We define **Structure Functions** $F_1$ and $F_2$ to describe the proton's internal charge distribution.

- If the proton were a soft jelly, $F_2$ would drop rapidly as $Q^2$ increases.
    
- **Observation:** The plot shows $F_2(x, Q^2)$ is roughly **constant** (flat lines) as $Q^2$ changes for a fixed $x$.
    
- **Interpretation:** This is called **Scaling**. It means the electron is scattering off **point-like constituents** (partons/quarks) inside the proton. A point particle has no size, so it looks the same no matter how high the "zoom" ($Q^2$) is.
    

#### Plot 3: The Callan-Gross Relation

We check the ratio of the magnetic structure function ($F_1$) to the electric one ($F_2$).

- The plot shows the ratio $\frac{2xF_1}{F_2} \approx 1$.
    
- **Mathematical Relation:** $2xF_1 = F_2$.
    
- **Physical Meaning:** This proves the point-like constituents have **Spin 1/2**. If they had Spin 0, $F_1$ would be zero.
    
- **Conclusion:** The proton is made of Spin 1/2 point particles. We call them **Quarks**.
    

---

### 4. The Proton Structure: What is inside?

The shape of $F_2(x)$ tells us how momentum is distributed inside the proton.

- **Scenario A (One Quark):** If the proton were just one quark, $F_2$ would be a spike at $x=1$.
    
- **Scenario B (3 Valence Quarks):** If the proton were just 3 equal quarks ($uud$), we would see a peak around $x = 1/3$.
    
- **The Reality (Valence + Sea + Gluons):**
    
    The data shows the distribution is smeared out towards **low x** (small momentum fractions).
    
    - **Valence Quarks:** carry the main quantum numbers (peak around $x \approx 0.18$).
        
    - **Sea Quarks:** Virtual quark-antiquark pairs popping in and out of existence (mostly at low $x$).
        
    - **Gluons:** They hold the quarks together. They carry about 50% of the proton's momentum but don't interact with the photon (since they are neutral), so they don't show up directly in $F_2$, but we infer them because the quarks don't add up to 100% of the momentum.
        

---

### 5. Exam Cheat Sheet (Summary)

If you see these questions on the exam, here are your answers:

1. **What is Bjorken Scaling?**
    
    It is the observation that the structure function $F_2$ depends only on the variable $x$, not on $Q^2$ ($F_2(x, Q^2) \approx F_2(x)$). It implies the proton contains point-like particles.
    
2. **What does the Callan-Gross relation ($2xF_1 = F_2$) tell us?**
    
    It tells us the point-like particles (partons) inside the proton have **Spin 1/2**.
    
3. **What is the physical meaning of $x$?**
    
    It is the fraction of the proton's momentum carried by the struck quark.
    
4. **Why do we see a rise in $F_2$ at low $x$?**
    
    This is due to the "Sea Quarks" (quark-antiquark pairs) and gluons at low momentum.
    

**One Next Step for you:**

Would you like me to walk you through a specific calculation example, such as calculating the "invariant mass" $W$ if I give you the beam energies, or should we focus on interpreting the Feynman diagrams for the exam?