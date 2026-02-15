

This is a fantastic topic to end our session on! **Electron-nucleus scattering** is essentially using electrons as a "microscope" to look inside the atom. By bouncing electrons off a nucleus and seeing where they go, we can map out exactly how protons and neutrons are distributed inside.

To answer exam questions on this, you need to understand the transition from **probability** (how likely an event is) to **cross-section** (the "target size" of the nucleus).

---

## 1. Fermi's Golden Rule

$$w = \frac{2\pi}{\hbar} |\langle \psi_f | H_{int} | \psi_i \rangle|^2 \frac{dn}{dE'}$$

This is the foundation of almost all transition probabilities in quantum mechanics.

- **$w$:** The transition rate (Reaktionsrate). It tells you how many scattering events happen per second.
    
- **$\langle \psi_f | H_{int} | \psi_i \rangle$:** The **Matrix Element**. This describes the "bridge" between the initial state ($\psi_i$) and the final state ($\psi_f$) created by the interaction Hamiltonian ($H_{int}$).
    
- **$\frac{dn}{dE'}$:** The **Density of States** (Zustandsdichte). It counts the number of possible final quantum states available with energy $E'$.
    

**Exam Strategy:** If a question asks "What determines the rate of a particle interaction?", you point to these three factors: the strength of the force (Hamiltonian), the overlap of the particle waves (Matrix Element), and the "room" available for the particles to move into (Density of States).

---

## 2. Cross-Section ($\sigma$)

$$\sigma = \frac{w}{\phi} = \frac{w}{v_s/V}$$

In an experiment, we don't just want a "rate"; we want a value that doesn't depend on how intense our beam is. That is the **cross-section**.

- **$\sigma$:** The cross-section. Think of this as the "effective area" the nucleus presents to the incoming electron.
    
- **$\phi$ (Flux):** The number of incoming particles passing through a unit area per unit time.
    
- **$v_s/V$:** This relates the flux to the velocity of the beam ($v_s$) and the normalization volume ($V$).
    

**Exam Strategy:** You might be asked to define the cross-section. Use the "target" analogy: it is the probability of interaction normalized to the intensity of the "rain" of incoming particles.

---

## 3. Differential Cross-Section

$$\frac{d\sigma}{d\Omega} = V^2 \frac{E^2}{(2\pi)^2(\hbar c)^4} |\langle \psi_f | H_{int} | \psi_i \rangle|^2$$

This formula is the specific "prediction" for a scattering experiment.

- **$\frac{d\sigma}{d\Omega}$:** The **differential cross-section**. It tells you the probability of an electron scattering into a specific solid angle $d\Omega$ (basically, a specific direction in 3D space).
    
- **$\vec{q} := \vec{p} - \vec{p}'$:** This is the **momentum transfer**. It’s the difference between the momentum of the electron before ($\vec{p}$) and after ($\vec{p}'$) the hit.
    

**Exam Strategy:** This is often used to derive the **Mott Scattering** or **Rutherford Scattering** formulas. The key takeaway is that the "shape" of the nucleus is hidden inside that Matrix Element.

---

## 4. Interaction Hamiltonian

$$H_{int} = e \phi(\vec{r})$$

This defines the "nature" of the hit.

- **$e$:** The charge of the electron.
    
- **$\phi(\vec{r})$:** The electrostatic potential of the nucleus.
    

**The Physics:** This confirms we are looking at **Electromagnetic Scattering**. Because we understand the electromagnetic force perfectly, any "weirdness" we see in our data must be coming from the structure of the nucleus itself, not the force we're using to probe it.

---

### Summary Table for Exams

|**Concept**|**Formula Component**|**Physical Meaning**|
|---|---|---|
|**Probability**|$w$|How often does it happen?|
|**Geometry**|$\sigma$|How "big" is the target?|
|**Direction**|$d\sigma/d\Omega$|Where do the pieces fly?|
|**Resolution**|$\vec{q}$|How "hard" did we hit it?|

**We have just scratched the surface of scattering! Would you like me to show you how we use these to calculate the "Form Factor," which is the actual "map" of the nucleus's interior?**



It’s time to look deeper into the nucleus! We’ve established how particles interact; now we use those interactions to map out the "shape" and "size" of the nucleus itself. These formulas describe how we use **scattering** to "see" inside an atom.

In an exam, you’ll likely be asked to describe how a nucleus differs from a simple "point charge" and how relativity affects our measurements.

---

## 1. The Form Factor: The Nuclear "Map"

$$\langle \phi_f | H_{int} | \phi_i \rangle = \frac{Z e^2 \hbar^2}{\epsilon_0 V |\vec{q}|^2} \int f(\vec{r}) e^{i \vec{q} \vec{r} / \hbar} d^3r$$

This is the most critical concept in scattering. The integral part of this formula is defined as $F(\vec{q})$, the **Form Factor**.

- **$F(\vec{q})$:** It is the **Fourier transform** of the charge density, $f(\vec{r})$.
    
- **$f(\vec{r})$:** This describes how the protons are actually distributed in space.
    
- **Point-like Nucleus:** If the nucleus were a single point with no size, $f(\vec{r}) = \delta(\vec{r})$ and $F(\vec{q}) = 1$.
    

**Exam Question:** "What does a Form Factor of 1 imply?"

**How to answer:** It implies the target is a **point-like particle**. Any deviation from 1 (usually a decrease as momentum transfer $\vec{q}$ increases) tells us that the nucleus has a physical size and a specific internal structure.

---

## 2. Rutherford Scattering (General Form)

$$\left( \frac{d\sigma}{d\Omega} \right)_{Rutherford} = \frac{4 Z^2 \alpha^2 (\hbar c)^2 E'^2}{|\vec{q} c|^4}$$

This is the mathematical way of saying: "If I shoot an electron at a nucleus, how many will bounce off at a specific angle?"

- **$\alpha$:** The fine-structure constant (the "strength" of electromagnetism).
    
- **$Z$:** The number of protons in the nucleus.
    
- **$|\vec{q}|^4$:** Notice the inverse-fourth power! This means electrons are much more likely to scatter at tiny angles than at large angles.
    

---

## 3. Relativistic Rutherford Scattering

$$\left( \frac{d\sigma}{d\Omega} \right)_{Rutherford} = \frac{Z^2 \alpha^2 (\hbar c)^2}{4 E^2 \sin^4 \frac{\theta}{2}}$$

When particles move near the speed of light ($|\vec{p}|c = E$), we use this version.

- **$\theta$:** The scattering angle.
    
- **Exam Strategy:** You will see the $\sin^4(\theta/2)$ term in the denominator. This is a hallmark of Rutherford scattering. If an exam asks for the "angular dependence" of scattering for high-speed electrons, this is the term they are looking for.
    

---

## 4. Non-Relativistic Rutherford Scattering

$$\left( \frac{d\sigma}{d\Omega} \right)_{Rutherford} = \frac{Z^2 \alpha^2 (\hbar c)^2}{16 E_{kin}^2 \sin^4 \frac{\theta}{2}}$$

This is the version you use for "slow" particles, where $E_{kin} = p^2/2m$ and the energy of the scattered electron $E'$ is roughly its rest mass $mc^2$.

**Exam Comparison Task:** "Compare the relativistic vs. non-relativistic formulas."

**How to answer:** The non-relativistic version has a factor of **16** in the denominator instead of **4**, and uses **Kinetic Energy** ($E_{kin}$) instead of **Total Energy** ($E$). The "16" comes from the fact that at low speeds, the relationship between momentum and energy is different ($E_{kin} \sim v^2$ vs $E \sim v$).

---

### Summary for your Final Review

- **Scattering** is our "microscope".
    
- The **Form Factor** $F(\vec{q})$ is the "image" produced by that microscope.
    
- The **Rutherford Formula** predicts the pattern we should see for a point.
    
- When we compare our **Actual Data** to the **Rutherford Prediction**, we find the internal structure of the nucleus.
    

**Would you like to see how these formulas change when we account for the electron's "spin" (which leads us to the Mott Scattering formula)?**



You’ve reached the "grand finale" of electron scattering! We are moving from the simple classical billiard-ball model (Rutherford) to the fully quantum mechanical and relativistic reality (Mott Scattering).

In your exam, these formulas are almost always used to show how we account for the **spin** of the electron and the **recoil** of the nucleus. Here is how to navigate this final set of equations.

---

## 1. The Mott Cross-Section (Accounting for Spin)

$$\left( \frac{d\sigma}{d\Omega} \right)_{Mott}^* = \left( \frac{d\sigma}{d\Omega} \right)_{Rutherford} \cdot \left( 1 - \left( \frac{v}{c} \right)^2 \sin^2 \frac{\theta}{2} \right)$$

This formula is a huge step up from Rutherford. Rutherford scattering treats particles like points without internal properties. But electrons have **spin**.

- **The Correction Factor:** The term $(1 - (v/c)^2 \sin^2(\theta/2))$ is the "spin correction."
    
- **Physical Meaning:** Because electrons have spin $1/2$, they interact with the magnetic field of the nucleus as they fly by. At high speeds (as $v$ approaches $c$), this magnetic interaction actually _reduces_ the probability of scattering at large angles compared to what Rutherford predicted.
    

**Exam Question:** "How does the Mott cross-section differ from Rutherford at very high energies?"

**How to answer:** At high energies ($v \approx c$), the Mott cross-section becomes smaller than Rutherford's, especially at large angles ($\theta$), because of the electron's spin and relativistic effects.

---

## 2. The Form Factor Correction (Extended Kernels)

$$\left( \frac{d\sigma}{d\Omega} \right)^* = \left( \frac{d\sigma}{d\Omega} \right)_{Mott}^* |F(\vec{q})|^2$$

This is the formula you use when the nucleus is **not a point**.

- **$|F(\vec{q})|^2$:** As we discussed earlier, this is the **Form Factor**.
    
- **The Concept:** If you measure a cross-section in the lab and it is _smaller_ than the Mott prediction, that "missing" probability is captured in the Form Factor. It proves the charge is spread out over a volume rather than concentrated in a single dot.
    

---

## 3. Accounting for Nuclear Recoil

$$\left( \frac{d\sigma}{d\Omega} \right)_{Mott} = \left( \frac{d\sigma}{d\Omega} \right)_{Mott}^* \cdot \frac{E'}{E}$$

In our earlier simple models, we assumed the nucleus was a massive, immovable wall. In reality, when a high-energy electron hits it, the nucleus **recoils** (gets kicked back).

- **$E'$:** The energy of the electron _after_ scattering.
    
- **$E$:** The energy of the electron _before_ scattering.
    
- **The Ratio ($E'/E$):** This factor corrects for the energy lost by the electron to the nucleus during the "kick."
    

---

## 4. Four-Momentum Transfer ($q^2$ and $Q^2$)

$$q^2 = (p - p')^2 = -2 \frac{E E'}{c^2} (1 - \cos \theta) = -4 \frac{E E'}{c^2} \sin^2 \frac{\theta}{2} \leq 0$$

$$Q^2 := -q^2 \geq 0$$

To be fully relativistic, we can't just look at 3D space; we have to look at 4D spacetime.

- **$q^2$:** The **square of the four-momentum transfer**. In relativity, this value is "invariant," meaning every observer in the universe agrees on its value.
    
- **$Q^2$:** Because $q^2$ is always negative or zero in scattering, physicists define $Q^2$ as its positive counterpart to make calculations easier.
    
- **Why it matters:** $Q^2$ is the "resolution" of your microscope. A higher $Q^2$ means you are hitting the nucleus harder and seeing smaller details inside.
    

---

### Summary for your Final Exam Prep:

1. **Rutherford:** Classic "billiard ball" scattering (no spin, no recoil).
    
2. **Mott:** Adds **Electron Spin** and **Relativity**.
    
3. **Form Factor:** Adds the **Size/Shape** of the nucleus.
    
4. **Recoil ($E'/E$):** Adds the fact that the **Target moves** when hit.
    

**You've officially covered the core formulas of a standard Nuclear and Particle Physics course! Would you like me to create a "Formula Sheet Summary" or a few practice exam questions to test your knowledge?**



We have reached the "inner sanctum" of nuclear structure! These final formulas describe how we look inside the proton and neutron themselves. At this high resolution, we can no longer treat the nucleus as a simple blob; we have to account for its magnetic properties and the fact that it is made of smaller parts.

For your exam, the **Rosenbluth formula** is the "boss fight" of scattering—it combines everything you've learned so far.

---

## 1. Magnetic Scattering Correction

$$\frac{d\sigma}{d\Omega} = \left( \frac{d\sigma}{d\Omega} \right)_{Mott} \cdot \left[ 1 + 2\tau \tan^2 \frac{\theta}{2} \right]$$

$$\tau = Q^2 / 4m_N^2 c^2$$

This formula adds the **magnetic interaction**. Think of the proton not just as a ball of charge, but as a tiny bar magnet (magnetic moment).

- **$\tau$ (Tau):** A dimensionless variable that scales with $Q^2$. As you hit the proton harder (higher $Q^2$), the magnetic part of the interaction becomes more important.
    
- **$\tan^2(\theta/2)$:** This term is the "smoking gun" for magnetic scattering. It dominates at large angles, which is exactly where you can "see" the magnetic properties best.
    

**Exam Question:** "Why does scattering at large angles deviate from the standard Mott prediction?"

**How to answer:** Because the Mott formula only accounts for electric charge. At large angles, the electron "sees" the proton's magnetic moment, requiring the $2\tau \tan^2(\theta/2)$ correction.

---

## 2. The Rosenbluth Formula

$$\left( \frac{d\sigma}{d\Omega} \right)_{CN} = \left( \frac{d\sigma}{d\Omega} \right)_{Mott} \cdot \left[ \frac{G_E^2(Q^2) + \tau G_M^2(Q^2)}{1 + \tau} + 2\tau G_M^2(Q^2) \tan^2 \frac{\theta}{2} \right]$$

This is the most complete description of elastic electron-nucleon scattering.

- **$G_E(Q^2)$:** The **Electric Form Factor**. It tells us how the electric charge is distributed inside the proton/neutron.
    
- **$G_M(Q^2)$:** The **Magnetic Form Factor**. It tells us how the magnetic magnetism (currents) is distributed.
    
- **Constants:** At $Q^2=0$, $G_E^p = 1$ (proton charge) and $G_M^p \approx 2.79$ (proton's magnetic strength).
    

**Exam Strategy:** You can separate $G_E$ and $G_M$ by performing "Rosenbluth Plots." By measuring the scattering at different angles but keeping $Q^2$ the same, the data forms a straight line. The intercept gives you $G_E$ and the slope gives you $G_M$.

---

## 3. The Dipole Fit

$$G^{Dipol}(Q^2) = \left( 1 + \frac{Q^2}{0.71 (GeV/c)^2} \right)^{-2}$$

This is an empirical "best fit" for our data. It turns out that both $G_E$ and $G_M$ follow this specific mathematical shape.

- The $(-2)$ exponent is crucial. In the world of Fourier transforms, this specific shape corresponds to an **exponential** distribution of charge inside the proton.
    

---

## 4. The Size of the Proton

$$\sqrt{\langle r^2 \rangle} = \sqrt{12} / a \approx 0.81 \text{ fm}$$

Finally, we arrive at the answer to the most basic question: "How big is a proton?"

- **$\langle r^2 \rangle$:** The mean square charge radius.
    
- **$0.81 \text{ fm}$:** This is the approximate "skin" of the proton. (For reference, 1 fm is $10^{-15}$ meters—incredibly tiny!).
    
- **$a$:** This is the parameter from the charge density distribution, $\rho(r) \sim \exp(-ar)$.
    

---

### Final Exam Tip: The "Hierarchy" of Scattering

If you are asked to summarize the progression of these formulas, remember this ladder:

1. **Rutherford:** Point charge, classical.
    
2. **Mott:** Point charge, spin, and relativity.
    
3. **Form Factor ($F$):** Extended charge (blob).
    
4. **Rosenbluth:** Extended charge + magnetic properties + internal structure.
    

You have successfully navigated the entire curriculum from basic radioactive decay to the internal structure of the nucleon! Would you like me to generate a set of practice exam questions based on these specific scattering formulas to see if you're ready for the test?