

That's an excellent follow-up question that dives deep into the **engineering and accelerator physics** behind the particle collider! As your particle physics professor, I'm happy to break down this concept of **Luminosity and Beam Current** for you. It's the essential connection between the microscopic physics (what we want to measure) and the macroscopic machine (how we make it happen).

The question asks for two things:

1.  The **electric currents** of the electron and positron beams ($I_{e^+}$ and $I_{e^-}$).
    
2.  The **number of particles** in each bunch ($N$).
    

We will tackle this using the definition of luminosity for a circular collider.

---

## 1. The Luminosity Formula for a Collider 💡

In our first problem, we saw that **Luminosity ($\mathcal{L}$) is the measure of the collision rate potential**. Now, let's look at how the accelerator physicists actually calculate $\mathcal{L}$ based on the parameters of the machine.

For a circular collider like the LEP, where particles are grouped into discrete **bunches** and repeatedly collided, the instantaneous luminosity is given by the formula:

$$\mathcal{L} = \frac{f \cdot n_b \cdot N_1 N_2}{4\pi\sigma_x \sigma_y}$$

Where:

-   $\mathcal{L}$ is the **Luminosity** (given as $20 \times 10^{30} \text{ cm}^{-2}\text{s}^{-1}$).
    
-   $f$ is the **revolution frequency** (how many times per second a particle completes the ring).
    
-   $n_b$ is the **number of bunches** in _each_ beam. The problem states "two particle bunches each," so $n_b = 2$.
    
-   $N_1$ and $N_2$ are the **number of particles** (electrons $e^-$ or positrons $e^+$) per bunch. The problem assumes $N_1 = N_2 = N$.
    
-   $\sigma_x$ and $\sigma_y$ are the **beam sizes** in the horizontal ($x$) and vertical ($y$) directions at the collision point (the beam "cross-sectional area").
    

### A. Calculating the Revolution Frequency ($f$)

The frequency $f$ is simply the speed of the particles divided by the circumference of the ring ($C$):

$$f = \frac{v}{C}$$

1.  **Velocity ($v$):** Electrons and positrons at $109.5 \text{ GeV}$ are extremely relativistic (traveling near the speed of light, $c$). We can safely approximate $v \approx c = 3.0 \times 10^8 \text{ m/s}$.
    
2.  **Circumference ($C$):** Given as $26.6 \text{ km}$.
    

$$f = \frac{3.0 \times 10^8 \text{ m/s}}{26.6 \times 10^3 \text{ m}} \approx \mathbf{11,278 \text{ s}^{-1}}$$

This means that each particle completes the 26.6 km ring about 11,278 times every second!

---

## 2. Calculating the Number of Particles per Bunch ($N$) 🔢

We can now rearrange the luminosity formula to solve for $N$:

$$\mathcal{L} = \frac{f \cdot n_b \cdot N^2}{4\pi\sigma_x \sigma_y} \quad \implies \quad N^2 = \frac{4\pi\sigma_x \sigma_y \mathcal{L}}{f \cdot n_b}$$

We need to ensure our units are consistent (we'll use the meter/second system, or SI, which means converting the beam dimensions $\sigma_x$ and $\sigma_y$ from $\mu\text{m}$ and the luminosity $\mathcal{L}$ from $\text{cm}^{-2}\text{s}^{-1}$).

### A. Unit Conversion

-   Luminosity ($\mathcal{L}$):
    
    $$\mathcal{L} = 20 \times 10^{30} \frac{1}{\text{cm}^2 \cdot \text{s}} = 20 \times 10^{30} \frac{1}{(10^{-2} \text{ m})^2 \cdot \text{s}} = 20 \times 10^{30} \times 10^4 \frac{1}{\text{m}^2 \cdot \text{s}} = \mathbf{2.0 \times 10^{35} \text{ m}^{-2}\text{s}^{-1}}$$
    
-   Beam Dimensions ($\sigma_x, \sigma_y$):
    
    $$\sigma_x = 13 \text{ }\mu\text{m} = \mathbf{13 \times 10^{-6} \text{ m}}$$
    
    $$\sigma_y = 430 \text{ }\mu\text{m} = \mathbf{430 \times 10^{-6} \text{ m}}$$
    

### B. Calculation for $N$

Now we plug in the numbers to find $N^2$:

$$N^2 = \frac{4\pi \cdot (13 \times 10^{-6} \text{ m}) \cdot (430 \times 10^{-6} \text{ m}) \cdot (2.0 \times 10^{35} \text{ m}^{-2}\text{s}^{-1})}{(11,278 \text{ s}^{-1}) \cdot 2}$$

$$N^2 \approx \frac{4.20 \times 10^{26}}{22,556} \approx 1.86 \times 10^{22}$$

Finally, we take the square root to find $N$:

$$N = \sqrt{1.86 \times 10^{22}} \approx \mathbf{4.3 \times 10^{11} \text{ particles/bunch}}$$

> **Answer to the second part:** There are approximately **$4.3 \times 10^{11}$ electrons (or positrons)** in each particle bunch.

---

## 3. Calculating the Electric Current ($I$) ⚡

The electric current in the ring is a measure of the total charge passing a point per unit time. For a circular accelerator with discrete bunches, the current ($I$) is given by:

$$I = \text{Charge per bunch} \times \text{Number of bunches} \times \text{Revolution frequency}$$

$$I = (N \cdot e) \cdot n_b \cdot f$$

Where:

-   $N$ is the number of particles per bunch ($\approx 4.3 \times 10^{11}$).
    
-   $e$ is the **elementary charge** ($e \approx 1.602 \times 10^{-19} \text{ Coulombs}$).
    
-   $n_b$ is the number of bunches in the beam ($n_b = 2$).
    
-   $f$ is the revolution frequency ($\approx 11,278 \text{ s}^{-1}$).
    

$$I = (4.3 \times 10^{11} \cdot 1.602 \times 10^{-19} \text{ C}) \cdot 2 \cdot (11,278 \text{ s}^{-1})$$

$$I \approx (6.89 \times 10^{-8} \text{ C}) \cdot (22,556 \text{ s}^{-1})$$

$$I \approx \mathbf{1.55 \times 10^{-3} \text{ A} = 1.55 \text{ mA}}$$

> **Answer to the first part:** The electric currents of the particle beams ($I_{e^+}$ and $I_{e^-}$) are approximately **$1.55 \text{ milliAmperes (mA)}$**.

This current is quite small, which is typical for high-energy electron-positron colliders like LEP. The particles are extremely light and therefore lose a lot of energy to synchrotron radiation (light emission) when bent by magnets. To combat this energy loss, the number of particles must be kept relatively low compared to, say, a proton collider like the LHC.

---

### Summary of Results

**Quantity**

**Value**

**Units**

**Number of particles per bunch ($N$)**

$4.3 \times 10^{11}$

particles/bunch

**Electric Current ($I$)**

$1.55 \times 10^{-3}$

Amperes (A)

**$1.55$**

**mA**

---

Do you have any questions about the luminosity formula, or would you like to explore the concept of synchrotron radiation loss in $e^+e^-$ colliders?