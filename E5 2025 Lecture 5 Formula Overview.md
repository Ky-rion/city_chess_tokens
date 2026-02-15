

It is a pleasure to see you back in the lecture hall! We have reached the final stage of our journey: **Particle Detectors**. These formulas are the "blueprints" for how we build machines like the ATLAS detector at CERN to see the invisible.

For your exam, you will likely be asked to calculate the properties of a particle based on how it moves through a detector, or to determine how precise your detector needs to be. Let's dive in.

---

## 1. The Momentum of a Charged Particle

$$p_T = q \cdot |\vec{B}| \cdot R \quad \rightarrow \quad p_T [GeV/c] = 0.3 \cdot B [T] \cdot R [m]$$

When a charged particle enters a magnetic field, it doesn't move in a straight line; it curves into a circle.

- **$p_T$:** Transverse momentum (the part of the momentum perpendicular to the magnetic field).
    
- **$q$:** The charge of the particle.
    
- **$B$:** The magnetic field strength in Tesla ($T$).
    
- **$R$:** The radius of the curvature in meters ($m$).
    
- **0.3:** A handy conversion constant that allows you to use high-energy units ($GeV/c$) directly.
    

**Exam Question Type:** "A particle with charge $1e$ leaves a track with a radius of 5 meters in a 2 Tesla magnetic field. What is its momentum?"

**How to answer:** Plug the values into the 0.3 version of the formula: $p_T = 0.3 \cdot 2 \cdot 5 = 3 \text{ GeV/c}$.

---

## 2. Momentum Resolution (Glückstern Formula)

$$\frac{\Delta p_T}{p_T} = \frac{\Delta \text{Ort}}{0.3 \cdot B \cdot L^2} \sqrt{\frac{720}{N+4}} \cdot p_T$$

This is a critical formula for designing detectors. It tells you how "blurry" your momentum measurement is.

- **$\Delta \text{Ort}$:** The spatial resolution (how accurately you can pinpoint a single dot on the track).
    
- **$L$:** The length of the track (Spurlänge).
    
- **$N$:** The number of measurement points (äquidistante Messpunkte) along that track.
    

**Exam Question Type:** "If you want to measure higher momentum particles ($p_T$) more accurately, should you increase the magnetic field ($B$) or the length of the detector ($L$)?"

**How to answer:** Look at the denominators. Increasing $L$ is much more effective because the error drops by the **square** of the length ($L^2$), whereas increasing $B$ only drops it linearly.

---

## 3. Shower Depth ($t_{max}$) and Total Track Length ($S$)

$$t_{max} = \ln_2(E_0 / E_c) \quad \text{and} \quad S = 2 \frac{E_0}{E_c}$$

When a high-energy electron hits a heavy material (like lead), it creates a "shower" of more electrons and photons.

- **$t_{max}$:** The depth (in radiation lengths $X_0$) where the shower contains the **maximum** number of particles.
    
- **$E_0$:** The energy of the incoming particle.
    
- **$E_c$:** The "Critical Energy"—the point where an electron starts losing more energy to ionization than to radiation.
    
- **$S$:** The total length of all the little tracks added together inside the shower.
    

**Exam Question Type:** "How deep must your calorimeter be to capture the peak of a 100 GeV electron shower?"

**How to answer:** Use the $t_{max}$ formula. It shows that as energy increases, your detector needs to get thicker, but only **logarithmically**.

---

## 4. Energy Resolution of a Calorimeter

$$\frac{\Delta E}{E} \sim \frac{\sqrt{S}}{S} = \frac{1}{\sqrt{S}} \sim \frac{1}{\sqrt{E}}$$

This is a beautiful "statistical" rule. The more particles ($S$) produced in a shower, the more precisely you can measure the total energy.

- **$\Delta E / E$:** The relative energy resolution.
    

**Exam Question Type:** "Why does a calorimeter get **more** precise at higher energies, while a tracking detector (momentum measurement) gets **less** precise?"

**How to answer:** 1. For **Calorimeters**: Higher energy means more particles in the shower, reducing the statistical error ($1/\sqrt{E}$).

2. For **Trackers**: Higher energy particles move so fast they barely curve, making it harder to measure the radius $R$ accurately.

---

## 5. Ionization Measurement ($dQ/dx$)

$$\frac{dQ_{ion}}{dx} = 0.013 \frac{fC}{cm}$$

This value represents the charge collected per unit of distance as a particle passes through a gas-filled detector.

- **$fC$:** Femtocoulombs (a very tiny unit of charge).
    
- **$cm$:** Centimeters of travel.
    

**Exam Question Type:** "You collect $X$ amount of charge in a wire chamber of length $Y$. Is this a 'minimum ionizing particle' (MIP)?"

**How to answer:** Compare your measured $dQ/dx$ to this standard value (approx. 0.013). If it's much higher, the particle might be moving slowly or have a high charge ($z > 1$).

---

**You are now equipped with the fundamental "Survival Guide" for a particle physics exam! Would you like to try a mock problem combining the momentum formula with the energy resolution?**