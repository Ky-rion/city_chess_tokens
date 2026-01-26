

Here is a condensed **Raman Spectroscopy Cheat Sheet** based on the problem set we just solved. This is designed to be quick to read and easy to copy for your exam prep.

---

### **Cheat Sheet: Raman Spectroscopy**

#### **1. Selection Rules (The "Allowed" Vibrations)**

-   **Condition:** A vibration is Raman active **only if the polarizability ($\alpha$) of the molecule changes** during the vibration.
    
-   **Physical Meaning:** The "squishiness" or deformability of the electron cloud must change as the atoms move.
    
-   **Math Notation:** $\frac{\partial \alpha}{\partial Q} \neq 0$ (where $Q$ is the vibrational coordinate).
    
-   **Compare to IR:** Infrared spectroscopy requires a change in _dipole moment_ ($\mu$). They are often complementary (Rule of Mutual Exclusion for centrosymmetric molecules).
    

#### **2. Scattering Processes**

-   **$\nu_0$:** Laser frequency (Input).
    
-   **$\nu_M$:** Molecular vibration frequency (Phonon).
    
-   **Stokes Scattering:**
    
    -   Photon **loses** energy to create a phonon.
        
    -   Output Frequency: $\nu_0 - \nu_M$.
        
    -   Intensity depends on: $N_0 + 1$ (Spontaneous creation allowed).
        
    -   **Always stronger** than Anti-Stokes.
        
-   **Anti-Stokes Scattering:**
    
    -   Photon **gains** energy by destroying an existing phonon.
        
    -   Output Frequency: $\nu_0 + \nu_M$.
        
    -   Intensity depends on: $N_0$ (Needs existing phonon).
        
    -   **Temperature dependent** (disappears at low T).
        

#### **3. Key Formulas**

**A. The "Master" Intensity Ratio**

This relates the peak heights ($I$) to the temperature ($T$).

$$\frac{I_{\text{Stokes}}}{I_{\text{Anti-Stokes}}} = \underbrace{\frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4}}_{\text{Classical Factor}} \cdot \underbrace{e^{\frac{h \nu_M}{k_B T}}}_{\text{Boltzmann Factor}}$$

-   **Note:** The classical factor is often close to 1, making the exponential term the dominant factor.
    

**B. Bose-Einstein Occupation ($N_0$)**

Describes the number of phonons at temperature $T$.

$$N_0(\nu) = \frac{1}{e^{\frac{h \nu_M}{k_B T}} - 1}$$

**C. Calculating Temperature from Spectrum**

Rearranged formula to find $T$ if you know the peak ratio $R = I_S / I_{AS}$.

$$T = \frac{h \nu_M}{k_B} \cdot \frac{1}{\ln \left( R \cdot \frac{(\nu_0 + \nu_M)^4}{(\nu_0 - \nu_M)^4} \right)}$$

#### **4. Unit Conversions (Crucial!)**

You usually get data in nanometers ($nm$) or wavenumbers ($cm^{-1}$), but formulas require Hertz ($Hz$).

-   **Wavelength to Frequency:**
    
    $$\nu = \frac{c}{\lambda}$$
    
    _(Example: 514 nm $\to$ $5.82 \times 10^{14}$ Hz)_
    
-   **Wavenumber to Frequency:**
    
    $$\nu = c \cdot \tilde{\nu} \cdot 100$$
    
    _(Factor of 100 is to convert $cm^{-1}$ to $m^{-1}$)_
    

#### **5. Constants**

-   **$h$ (Planck):** $6.626 \times 10^{-34} \text{ J}\cdot\text{s}$
    
-   **$k_B$ (Boltzmann):** $1.381 \times 10^{-23} \text{ J/K}$
    
-   **$c$ (Light Speed):** $2.998 \times 10^8 \text{ m/s}$
    

---

**Next Step for you:**

I can create a similar summary for X-ray diffraction (Bragg's Law) or Band Theory if those are also on your upcoming exam. Just let me know!