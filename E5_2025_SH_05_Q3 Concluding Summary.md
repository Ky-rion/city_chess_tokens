

Here is a condensed "Cheat Sheet" summary of the key formulas and concepts we covered. This is designed for quick reference during your studies or an exam.

### **Particle Accelerator Physics Cheat Sheet**

#### **1. Beam Bending (The "Golden Formula")**

This relates the momentum of the particle to the magnetic field and the radius of the circle.

$$p [\text{GeV}/c] = 0.3 \cdot B [\text{T}] \cdot R [\text{m}]$$

-   **$p$**: Beam momentum (often $\approx$ Energy $E$ at high speeds).
    
-   **$B$**: Magnetic field strength in Tesla.
    
-   **$R$**: Radius of curvature in meters.
    
-   **$0.3$**: A conversion factor derived from the speed of light ($c$).
    

**Useful rearrangements:**

-   To find B-field:
    
    $$B = \frac{p}{0.3 \cdot R}$$
    
-   To find Radius:
    
    $$R = \frac{p}{0.3 \cdot B}$$
    

---

#### **2. Synchrotron Radiation (Energy Loss)**

Charged particles radiate energy when forced to move in a circle.

**For Electrons:**

$$\Delta E_{turn} [\text{keV}] \approx 88.5 \cdot \frac{E^4 [\text{GeV}]}{R [\text{m}]}$$

-   **Key Insight ($E^4$):** Doubling the energy increases radiation by **16x**. This is the main limit for electron synchrotrons.
    

**For Protons vs. Electrons (Mass Scaling):**

Radiation drops drastically as mass increases.

$$\Delta E \propto \frac{1}{m^4}$$

To compare losses between two particles at the same energy:

$$\frac{\Delta E_p}{\Delta E_e} = \left( \frac{m_e}{m_p} \right)^4$$

_(Since protons are ~2000x heavier, this ratio is effectively zero for most calculations.)_

---

#### **3. Power Consumption**

The power required to restore the lost energy (RF Power).

$$P = I_{beam} \cdot V_{effective}$$

-   **$I_{beam}$**: Beam current (Amperes).
    
-   **$V_{effective}$**: The "voltage kick" needed per turn. If loss is $2.4 \text{ GeV}$, then $V_{eff} = 2.4 \text{ GV}$.
    
-   **Note:** If there are two beams (e.g., $e^+$ and $e^-$), calculate for one and multiply by **2**.
    

---

#### **4. Crucial Exam "Gotchas"**

-   **Center of Mass vs. Beam Energy:**
    
    If the problem says "Center of Mass Energy ($E_{CM}$) = 209 GeV", the energy of a _single_ beam is half that:
    
    $$E_{beam} = \frac{E_{CM}}{2}$$
    
    _(Always use $E_{beam}$ for the formulas above!)_
    
-   **Approximation ($E \approx p$):**
    
    For high-energy particles (GeV/TeV scale), Energy ($E$) and Momentum ($p \cdot c$) are numerically almost identical.
    
    $$E [\text{GeV}] \approx p [\text{GeV}/c]$$
    
-   **Geometric Radius vs. Magnetic Radius (Packing Factor):**
    
    -   **$R_{tunnel}$**: The physical size of the tunnel ($C / 2\pi$).
        
    -   **$R_{magnetic}$**: The actual bending radius inside the magnets.
        
    -   _Reality Check:_ $R_{magnetic}$ is always **smaller** than $R_{tunnel}$ because straight sections (for detectors/RF) don't bend the beam. This means the real B-field must be **higher** than the theoretical minimum.
        

---

**Next Step:**

You are now armed with the theory! Would you like to try a "practice quiz" question where I give you a hypothetical new particle accelerator (maybe on the Moon!) and you calculate the parameters using this cheat sheet?