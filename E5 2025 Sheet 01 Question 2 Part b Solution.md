

This is a crucial question that highlights why **colliding beam experiments** (like HERA and LHC) are vastly more efficient for discovery than **fixed-target experiments**. It requires calculating the incoming particle's energy needed to achieve the same center-of-mass energy when one particle is at rest.

The goal is to find the kinetic energy ($E_{\text{kin}}$) an electron needs to achieve the center-of-mass energy $E_{\text{CM}} \approx 318.1 \text{ GeV}$ when colliding with a **proton at rest** (a fixed-target experiment).

---

## 1. The Fixed-Target Kinematics Formula

In the previous problem, the center-of-mass energy squared ($s$) for the HERA collider was $s = E_{\text{CM}}^2 \approx 101,200 \text{ GeV}^2$.

When one particle (the **target**, $P$) is at **rest** and the other (the **beam**, $e$) has an incoming energy $E_e$, the total energy squared in the center-of-mass system ($s$) is given by the general relativistic formula:

$$s = m_e^2 c^4 + m_p^2 c^4 + 2 E_e m_p c^2$$

Where:

-   $m_e c^2$ is the rest energy of the electron ($E_{0,e}$).
    
-   $m_p c^2$ is the rest energy of the proton ($E_{0,p}$).
    
-   $E_e$ is the **total energy** of the incident electron (which equals $E_{0,e} + E_{\text{kin}}$).
    

### A. The Extreme Relativistic Approximation

Since the required electron energy ($E_e$) will be extremely high (far exceeding its rest energy $E_{0,e} \approx 0.000511 \text{ GeV}$), we can simplify the formula:

1.  **Neglect the electron's rest mass:** $m_e^2 c^4 \approx 0$.
    
2.  **Use the proton's rest mass:** We cannot neglect the target proton's rest mass, $m_p c^2 \approx 0.938 \text{ GeV}$, as it is the stationary energy reservoir.
    

The simplified fixed-target formula becomes:

$$s \approx m_p^2 c^4 + 2 E_e m_p c^2$$

---

## 2. Calculation of Required Electron Energy

We will use the calculated values from part (a):

$$s = E_{\text{CM}}^2 \approx 101,200 \text{ GeV}^2$$

$$m_p c^2 \approx 0.938 \text{ GeV}$$

We need to solve the simplified equation for the electron's total energy, $E_e$:

$$s \approx m_p^2 c^4 + 2 E_e m_p c^2$$

$$2 E_e m_p c^2 \approx s - m_p^2 c^4$$

$$E_e \approx \frac{s - m_p^2 c^4}{2 m_p c^2}$$

### A. Calculate the terms

1.  **The $s$ term:** $s \approx 101,200 \text{ GeV}^2$
    
2.  The $m_p^2 c^4$ term: This is the square of the proton's rest energy.
    
    $$m_p^2 c^4 \approx (0.938 \text{ GeV})^2 \approx 0.880 \text{ GeV}^2$$
    

Notice how the $m_p^2 c^4$ term ($0.880 \text{ GeV}^2$) is negligible compared to the $s$ term ($101,200 \text{ GeV}^2$). This allows us to make a further, excellent approximation:

$$s - m_p^2 c^4 \approx s$$

The formula simplifies one last time to a very useful relation:

$$E_e \approx \frac{s}{2 m_p c^2}$$

### B. Final Calculation

$$E_e \approx \frac{101,200 \text{ GeV}^2}{2 \times 0.938 \text{ GeV}}$$

$$E_e \approx \frac{101,200 \text{ GeV}^2}{1.876 \text{ GeV}}$$

$$E_e \approx \mathbf{53,944 \text{ GeV}}$$

---

## 3. Interpreting the Result

The question asks for the **energy** electrons need. Since the electron's rest energy ($E_{0,e} \approx 0.000511 \text{ GeV}$) is completely negligible compared to the calculated total energy ($53,944 \text{ GeV}$), the total energy is almost entirely **kinetic energy** ($E_e \approx E_{\text{kin}}$).

$$\text{Required Electron Energy: } \mathbf{53,944 \text{ GeV}}$$

### The Physics of Collider vs. Fixed-Target

This result dramatically illustrates the advantage of a colliding-beam experiment:

**Experiment Type**

**Incoming Electron Energy**

**Center-of-Mass Energy (ECM​)**

**Colliding Beam (HERA)**

$27.5 \text{ GeV}$

$318.1 \text{ GeV}$

**Fixed-Target (Equivalent)**

$\mathbf{53,944 \text{ GeV}}$

$318.1 \text{ GeV}$

To achieve the same useful collision energy ($318.1 \text{ GeV}$) in a fixed-target setup, the electron beam would need to be accelerated to over **53,000 $\text{GeV}$**—nearly **2,000 times higher** than the energy actually used in the HERA ring ($27.5 \text{ GeV}$).

**Why this huge difference?**

In a fixed-target collision, most of the beam particle's kinetic energy is "wasted" on **moving the center-of-mass system forward** (to conserve momentum). Only a small fraction is available to create new mass. In a collider, since the particles' momenta cancel out ($\mathbf{p}_1 \approx -\mathbf{p}_2$), the center-of-mass system is stationary, and **nearly all the energy** goes into the actual collision and particle production. This principle is why all modern, high-energy discovery machines (LHC, etc.) are colliders.