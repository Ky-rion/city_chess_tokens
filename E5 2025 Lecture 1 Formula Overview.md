

Welcome to the fascinating world of particle physics! It's a pleasure to help you navigate these lecture notes. Think of these formulas as the "language" we use to describe how the smallest building blocks of our universe interact.

Here is a breakdown of your formulas, organized by their role in understanding subatomic collisions.

---

## 1. The "Natural" Conversion Factor

At the top of your notes, you see a specific value for $(\hbar c)^2$. In particle physics, we often use **Natural Units** where we set certain constants to 1 to make the math easier. However, to get a result you can actually measure (like an area), you need this conversion factor.

$$(\hbar c)^2 = 0.389 \text{ GeV}^2 \cdot \text{mb}$$

- **The Letters:**
    
    - $\hbar$ (h-bar): The reduced Planck constant, representing the scale of quantum mechanics.
        
    - $c$: The speed of light.
        
    - $\text{GeV}$: Giga-electronvolts (a unit of energy).
        
    - $\text{mb}$: Millibarns. A "barn" (b) is a unit of area used to describe the size of a target.
        
- **What it's for:** This is your "Rosetta Stone." It allows you to convert between units of energy and units of area (cross-sections).
    

---

## 2. Relativistic Kinematics

These formulas describe how particles behave when they are moving near the speed of light.

$$\gamma = \frac{E}{mc^2}, \quad \vec{\beta}\gamma = \frac{\vec{p}}{mc}, \quad \vec{\beta} = \frac{\vec{p}c}{E}$$

- **The Letters:**
    
    - $E$: Total energy.
        
    - $m$: Invariant mass (rest mass) of the particle.
        
    - $\vec{p}$: Momentum vector.
        
    - $\beta$ (beta): The velocity of the particle as a fraction of the speed of light ($v/c$).
        
    - $\gamma$ (gamma): The Lorentz factor, which tells us how much time dilation or length contraction is occurring.
        
- **What it's for:** We use these to calculate a particle's energy or momentum if we know its speed, or vice-versa. In high-energy physics, particles move so fast that simple Newtonian physics no longer works.
    

---

## 3. Scattering & Luminosity (The "Hit Rate")

These formulas describe the "Wirkungsquerschnitt" (Cross-section) and "Luminosität" (Luminosity).

$$\sigma = \frac{\dot{N}}{\phi_s \cdot N_T}, \quad \mathcal{L} = \phi_s \cdot N_T, \quad \dot{N} = \mathcal{L} \cdot \sigma$$

- **The Letters:**
    
    - $\sigma$ (sigma): The **Cross-section**. Think of this as the "effective size" of the target. The larger the $\sigma$, the more likely a collision will happen.
        
    - $\dot{N}$: The rate of interactions (number of events per second).
        
    - $\phi_s$: Flux density of the incoming beam.
        
    - $N_T$: Number of target particles.
        
    - $\mathcal{L}$: **Luminosity**. This describes the performance of the particle accelerator—essentially how "bright" or intense the beam is.
        
- **What it's for:** If a physicist wants to know how many Higgs Bosons they will find in a year, they multiply the Luminosity of the collider by the Cross-section of the Higgs.
    

---

## 4. Differential Cross-Section

Sometimes we don't just want to know _if_ a particle hit the target, but _where_ it bounced off to.

$$\frac{d\sigma}{d\Omega} = \frac{1}{\mathcal{L}} \frac{d\dot{N}}{d\Omega}$$

- **The Letters:**
    
    - $d\Omega$: The solid angle element (a 3D "cone" or area on a sphere).
        
    - $\frac{d\sigma}{d\Omega}$: The **Differential Cross-section**.
        
- **What it's for:** This tells us the probability of a particle scattering into a specific direction. This is crucial for understanding the internal structure of the target (like how Rutherford discovered the atomic nucleus).
    

---

## 5. Rutherford Scattering

This is the "Granddaddy" of all scattering formulas, describing how charged particles (like Alpha particles) deflect off a nucleus.

$$\left(\frac{d\sigma}{d\Omega}\right)_{\text{Rutherford}} = \frac{z^2 Z^2 \alpha^2 (\hbar c)^2}{16 E_{\text{kin}}^2} \frac{1}{\sin^4 \frac{\theta}{2}}$$

- **The Letters:**
    
    - $z, Z$: The charges of the projectile and the target nucleus.
        
    - $\alpha$: The fine-structure constant (approximately 1/137), which describes the strength of the electromagnetic force.
        
    - $E_{\text{kin}}$: Kinetic energy of the incoming particle.
        
    - $\theta$: The scattering angle.
        
- **What it's for:** This formula predicts how many particles will be deflected at a certain angle $\theta$. Note the $1/\sin^4(\theta/2)$ term—it means that as the angle gets smaller (closer to 0), the number of particles shoots up toward infinity! This is why most particles in these experiments pass almost straight through.
    

Does that help clear up the "alphabet soup" in your notes? Would you like me to walk through a practice calculation using one of these, perhaps to see how we use the conversion factor?