

That's an excellent next question! This problem deals with **relativistic kinematics** and calculating the **center-of-mass energy ($\sqrt{s}$) ** for a head-on collision, which is the most critical parameter for any particle collider experiment.

The question asks for the **total energy in the center-of-mass system ($E_{\text{CM}}$)** for an electron-proton ($ep$) collision at the **HERA storage ring**.

---

## 1. The Center-of-Mass Energy ($\sqrt{s}$)

In particle physics, the total energy available to create new particles in a collision is determined by the energy in the **center-of-mass (CM)** frame. This is often denoted by $\sqrt{s}$, where $s$ is the square of the total energy.

The general formula for the square of the total energy in a collision between two particles (1 and 2) is derived from the square of the total four-momentum ($P_T = P_1 + P_2$):

$$s = E_{\text{CM}}^2 = (P_1 + P_2)^2$$

$$s = (E_1 + E_2)^2 - (c\mathbf{p}_1 + c\mathbf{p}_2)^2$$

Where $E_1, E_2$ are the total energies and $\mathbf{p}_1, \mathbf{p}_2$ are the momenta vectors.

### A. The Head-On Collision Formula

For a **head-on collision** where the momenta are directly opposite ($\mathbf{p}_1 = -\mathbf{p}_2$, and thus $\mathbf{p}_1 \cdot \mathbf{p}_2 = -p_1 p_2$), the formula simplifies significantly.

Since both the electron and proton are highly relativistic (their energies are much greater than their rest masses), we can use the extreme relativistic approximation:

$$E \approx pc \quad \text{or} \quad p \approx E/c$$

(where $E$ is the total energy and $p$ is the magnitude of the momentum).

For a head-on collision ($p_1$ and $p_2$ are in opposite directions):

$$\mathbf{p}_1 \cdot \mathbf{p}_2 = -p_1 p_2 \approx -(E_1/c)(E_2/c) = -E_1 E_2/c^2$$

Substituting this into the general formula for $s$:

$$s = (E_1 + E_2)^2 - c^2 (\mathbf{p}_1 + \mathbf{p}_2) \cdot (\mathbf{p}_1 + \mathbf{p}_2)$$

$$s = E_1^2 + E_2^2 + 2E_1 E_2 - c^2 (p_1^2 + p_2^2 + 2 \mathbf{p}_1 \cdot \mathbf{p}_2)$$

Using the extreme relativistic approximation ($E^2 \approx (pc)^2$) and the head-on condition:

$$s \approx E_1^2 + E_2^2 + 2E_1 E_2 - c^2 \left( (E_1/c)^2 + (E_2/c)^2 + 2 (-E_1 E_2/c^2) \right)$$

$$s \approx E_1^2 + E_2^2 + 2E_1 E_2 - (E_1^2 + E_2^2 - 2E_1 E_2)$$

$$s \approx 4 E_1 E_2$$

This simple and elegant result, $\mathbf{s \approx 4 E_1 E_2}$, is the key to calculating $E_{\text{CM}}$ for highly relativistic head-on collisions where the rest masses are negligible.

---

## 2. Calculation of $E_{\text{CM}}$

We are given the following energies:

**Particle**

**Symbol**

**Energy (E)**

**Electron**

$E_e$

$27.5 \text{ GeV}$

**Proton**

$E_p$

$920 \text{ GeV}$

### A. Check the Relativistic Condition

To justify using the approximation $s \approx 4 E_e E_p$, we check the rest energies:

-   $E_{0, e} = m_e c^2 \approx 0.000511 \text{ GeV}$
    
-   $E_{0, p} = m_p c^2 \approx 0.938 \text{ GeV}$
    

Since $E_e \gg E_{0, e}$ ($27.5 \text{ GeV}$ vs $0.000511 \text{ GeV}$) and $E_p \gg E_{0, p}$ ($920 \text{ GeV}$ vs $0.938 \text{ GeV}$), the **extreme relativistic approximation is extremely accurate**.

### B. Calculate $s$

$$s \approx 4 E_e E_p$$

$$s \approx 4 \times (27.5 \text{ GeV}) \times (920 \text{ GeV})$$

$$s \approx 4 \times 25300 \text{ GeV}^2$$

$$s \approx 101,200 \text{ GeV}^2$$

### C. Calculate $E_{\text{CM}}$ ($\sqrt{s}$)

The total energy in the center-of-mass system is $\sqrt{s}$:

$$E_{\text{CM}} = \sqrt{s} = \sqrt{101,200 \text{ GeV}^2}$$

$$E_{\text{CM}} \approx \mathbf{318.1 \text{ GeV}}$$

---

## 3. The Full Relativistic Calculation (Verification)

While the approximation is sufficient, let's verify with the full relativistic formula which includes the rest masses for completeness.

The exact relativistic formula for $s$ in a head-on collision is:

$$s = 2(E_e E_p + c^2 p_e p_p) + m_e^2 c^4 + m_p^2 c^4$$

Using the momentum-energy relation $E^2 = (pc)^2 + E_0^2$, we can solve for $p^2 c^2 = E^2 - E_0^2$.

In the extreme relativistic limit, $E \gg E_0$, so $E \approx pc$. Therefore, $E_e E_p \approx (pc)_e (pc)_p$.

The full formula simplifies to the head-on case where $p_e \approx E_e/c$ and $p_p \approx E_p/c$ and $c^2 p_e p_p = E_e E_p$.

$$s \approx 2(E_e E_p + E_e E_p) + E_{0,e}^2 + E_{0,p}^2$$

$$s \approx 4 E_e E_p + E_{0,e}^2 + E_{0,p}^2$$

The rest mass terms $E_{0,e}^2$ and $E_{0,p}^2$ are $(0.000511)^2 \text{ GeV}^2$ and $(0.938)^2 \text{ GeV}^2$, respectively.

-   $E_{0,e}^2 \approx 2.6 \times 10^{-7} \text{ GeV}^2$
    
-   $E_{0,p}^2 \approx 0.880 \text{ GeV}^2$
    

Since $4 E_e E_p \approx 101,200 \text{ GeV}^2$, the rest mass terms contribute almost nothing to the result, confirming that $\mathbf{E_{\text{CM}} \approx \sqrt{4 E_e E_p}}$ is highly accurate.

The calculated total energy in the center-of-mass system is **$318.1 \text{ GeV}$**. This is the maximum energy available in the collision to create new, exotic particles.