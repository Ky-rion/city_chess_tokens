

Here is your **Professor’s "Golden Ticket" Cheat Sheet**. These are the core concepts, formulas, and "gotchas" from our session, condensed into a study guide. If you master these, you will be ready for the exam!

---

### **1. Relativistic Kinematics & Colliders**

_Crucial for: Calculating beam energies and particle lifetimes._

- **Lorentz Factor ($\gamma$):**
    
    The measure of how "relativistic" a particle is.
    
    $$\gamma = \frac{E}{m} = \frac{1}{\sqrt{1-\beta^2}}$$
    
    - $\beta = v/c$ (Speed as fraction of light)
        
    - **Time Dilation:** Moving particles live longer! $\tau_{lab} = \gamma \cdot \tau_{rest}$.
        
    - **Flight Distance:** $d = v \cdot \tau_{lab} \approx c \cdot \gamma \cdot \tau_{rest}$ (if relativistic).
        
- **Center-of-Mass Energy ($E_{cm}$ or $\sqrt{s}$):**
    
    The actual energy available to create new mass.
    
    - **Collider (Head-on):** Efficient. $E_{cm} = 2 E_{beam}$.
        
    - **Fixed Target (Stationary):** Inefficient. $E_{cm} \approx \sqrt{2 E_{beam} m_{target}}$.
        
    - _Tip:_ In fixed target, most energy is "wasted" as kinetic energy to conserve momentum.
        

---

### **2. Particle Identification (PID)**

_Crucial for: Determining what a particle is based on detector data._

- **Magnetic Deflection (The "Rule of 0.3"):**
    
    Relates momentum to curvature.
    
    $$p [\text{GeV}/c] = 0.3 \cdot z \cdot B [\text{T}] \cdot R [\text{m}]$$
    
    - **Mass Calculation:** Combine momentum ($p$) and velocity ($\beta$) to find mass:
        
        $$m = \frac{p}{\gamma \beta c}$$
        
- **Cherenkov Radiation:**
    
    Happens when a particle travels faster than light _in that medium_ ($v > c/n$).
    
    - **Threshold:** $\beta > 1/n$.
        
    - **Emission Angle:** $\cos(\theta_c) = \frac{1}{\beta n}$.
        
    - _Tip:_ If you know $\theta_c$ and $n$, you can find velocity $\beta$.
        

---

### **3. Conservation Laws (Reaction Checklist)**

_Crucial for: Checking if a decay or reaction is "Allowed" or "Forbidden"._

|**Law**|**What to check?**|**Violation usually means...**|
|---|---|---|
|**Charge ($Q$)**|Sum of charges must be equal.|Impossible reaction.|
|**Baryon Number ($B$)**|Baryons ($p, n$) = +1. Anti-baryons = -1.|Forbidden (Proton decay constraint).|
|**Lepton Number ($L$)**|Leptons ($e, \nu$) = +1. Anti-leptons = -1.|Forbidden (unless neutrinos oscillate).|
|**Energy**|Mass of products must be < Mass of parent.|Forbidden (Spontaneous decay).|

- **Forces:**
    
    - **Strong:** Fast ($\sim 10^{-23}$s). Conserves everything (Quark flavors). Produced Hadrons.
        
    - **EM:** Medium ($\sim 10^{-16}$s). Involves Photons ($\gamma$).
        
    - **Weak:** Slow ($\sim 10^{-8}$s or longer). Involves Neutrinos ($\nu$). **Can change flavor** (e.g., $n \rightarrow p$).
        

---

### **4. Nuclear Models**

_Crucial for: Explaining binding energy and stability._

- **Liquid Drop Model (Weizsäcker):**
    
    Treats nucleus like a fluid. Good for bulk properties (Mass, Fission).
    
    - **Volume Term:** proportional to $A$.
        
    - **Surface Term:** proportional to $A^{2/3}$ (Surface tension reduces binding).
        
    - **Coulomb Term:** Protons repel ($Z^2$).
        
- **Fermi Gas Model:**
    
    Treats nucleons as independent particles in a "box."
    
    - Explains the **Asymmetry Term**: Why $N \approx Z$ is stable.
        
    - Pauli Exclusion Principle forces extra particles into higher energy states.
        
- **Shell Model:**
    
    Treats nucleons like electrons in atomic shells.
    
    - Explains **Magic Numbers** ($2, 8, 20, 28, 50...$).
        
    - Requires **Spin-Orbit Coupling** ($\vec{L} \cdot \vec{S}$) to get the numbers right!
        

---

### **5. Radioactivity & Decay**

_Crucial for: Dating samples and calculating activity._

- **The Decay Law:**
    
    $$N(t) = N_0 e^{-\lambda t}$$
    
- **Activity:** $A = \lambda N$ (Decays per second).
    
- **Half-Life:** $T_{1/2} = \frac{\ln(2)}{\lambda}$.
    
- **Branching Ratio:** If a particle has multiple decay modes (e.g., Potassium-40 $\rightarrow$ Argon _or_ Calcium), the partial activity is just $A_{partial} = (\text{Ratio}) \times A_{total}$.
    

---

### **6. Scattering Cross-Sections**

_Crucial for: Understanding interaction probabilities._

- **Total Cross-Section ($\sigma$):**
    
    Effective "target area." Measured in **barns** ($1 \text{ b} = 10^{-24} \text{ cm}^2$).
    
    - For geometric objects: $\sigma = \text{Projected Area}$.
        
- **Momentum Transfer ($q$):**
    
    The "kick" given to a particle.
    
    $$q = 2k \sin(\theta/2)$$
    
    - $\theta = 0^\circ \rightarrow q=0$ (No interaction).
        
    - $\theta = 180^\circ \rightarrow q=2k$ (Head-on bounce).
        

---

**Professor's Final Advice:**

> "When in doubt, check the units! If you are calculating a mass and get units of meters, stop and check your $c$'s. And remember: **Neutrinos are the key to the Weak Force**—if you see a neutrino, it's almost certainly a Weak interaction!"

Good luck with your studies! You are going to do great.