

Hello! That's an excellent question. It gets to the very heart of _why_ we build colliders the way we do. Let's break it down step-by-step.

Here's the solution, followed by a detailed explanation of the physics.

The total energy in the centre-of-mass system is **318 GeV**.

---

### 🤔 What is "Centre-of-Mass Energy"?

First, let's talk about the main concept. You might be tempted to just add the two energies: $27.5 \text{ GeV} + 920 \text{ GeV} = 947.5 \text{ GeV}$.

While this is the **total energy** in the laboratory, it is _not_ the energy that's available to create new particles in the collision. Why? Because the system as a whole is still moving (since the proton has much more momentum than the electron). A lot of that 947.5 GeV is "wasted" as kinetic energy of the entire system moving through the detector.

The **centre-of-mass energy** (which we'll call $E_{cm}$) is the energy in a special, theoretical reference frame where the _total momentum is zero_. In this frame, the particles are flying at each other with equal and opposite momentum. No energy is "wasted" on moving the whole system, so $E_{cm}$ represents the **true available energy for the collision**—the energy that can be converted into the mass of new, exciting particles (like the Higgs boson, or quarks).

---

### 🧮 Where the Equation Comes From

To calculate this, we need to use a concept from Einstein's special relativity: the **invariant mass**.

1.  **Four-Momentum:** In relativity, we combine energy ($E$) and 3-momentum ($\vec{p}$) into a single four-vector, $p^\mu = (E, \vec{p})$. (We'll use units where $c=1$, which is standard in particle physics).
    
2.  **The Invariant:** The "length" squared of this four-vector is an "invariant"—it has the same value in _all_ reference frames. This quantity is $p^\mu p_\mu = E^2 - |\vec{p}|^2 = m^2$ (where $m$ is the particle's rest mass).
    
3.  **For a System:** We can find the invariant for the _entire system_ (electron + proton) by adding their four-momenta _first_ and then finding the "length" squared. We'll call this invariant $s$.
    
    $$s = (p_e^\mu + p_p^\mu)^2 = ((E_e + E_p), (\vec{p}_e + \vec{p}_p))^2$$
    
    $$s = (E_e + E_p)^2 - |\vec{p}_e + \vec{p}_p|^2$$
    
4.  **The Key Insight:** This quantity $s$ is the same in the lab frame (where we are) as it is in the centre-of-mass frame.
    
    -   **In the lab frame:** $s = (E_e + E_p)^2 - |\vec{p}_e + \vec{p}_p|^2$
        
    -   **In the C.M. frame:** By definition, the total momentum is zero, $\vec{p}_{cm} = 0$. So, $s = (E_{cm})^2 - |\vec{0}|^2 = E_{cm}^2$.
        
    
    Therefore, we have our master equation:
    
    $$E_{cm}^2 = s = (E_e + E_p)^2 - |\vec{p}_e + \vec{p}_p|^2$$
    

---

### ⚡️ A Powerful Simplification

Now let's look at the numbers.

-   Electron energy $E_e = 27.5 \text{ GeV}$. Electron rest mass $m_e \approx 0.000511 \text{ GeV}$.
    
-   Proton energy $E_p = 920 \text{ GeV}$. Proton rest mass $m_p \approx 0.938 \text{ GeV}$.
    

Both particles are **ultra-relativistic**, meaning their kinetic energy is _thousands_ of times larger than their rest mass.

For any ultra-relativistic particle, the rest mass is negligible. From the energy-momentum relation $E^2 = (pc)^2 + (mc^2)^2$ (or $E^2 = p^2 + m^2$ in our units), we can see that if $m$ is tiny, then $E^2 \approx p^2$, which means **$E \approx p$**.

The particle's momentum is almost equal to its energy.

Now we can simplify our master equation:

-   The collision is "head-on," so $\vec{p}_e$ and $\vec{p}_p$ point in opposite directions.
    
-   Let's say the electron moves right ($+p_e$) and the proton moves left ($-p_p$).
    
-   $|\vec{p}_e + \vec{p}_p|^2 = (p_e - p_p)^2$.
    
-   Our equation becomes: $E_{cm}^2 = (E_e + E_p)^2 - (p_e - p_p)^2$.
    
-   Now we use our approximation $p_e \approx E_e$ and $p_p \approx E_p$:
    
    $$E_{cm}^2 \approx (E_e + E_p)^2 - (E_e - E_p)^2$$
    
-   Let's expand this algebra:
    
    $$E_{cm}^2 \approx (E_e^2 + 2E_e E_p + E_p^2) - (E_e^2 - 2E_e E_p + E_p^2)$$
    
    $$E_{cm}^2 \approx E_e^2 + 2E_e E_p + E_p^2 - E_e^2 + 2E_e E_p - E_p^2$$
    
    $$E_{cm}^2 \approx 4 E_e E_p$$
    

This gives us our wonderfully simple, final formula for a head-on, ultra-relativistic collision:

$$E_{cm} \approx \sqrt{4 E_e E_p}$$

---

### Solution: The Calculation

Now, we just plug in the numbers from your problem.

-   $E_e = 27.5 \text{ GeV}$
    
-   $E_p = 920 \text{ GeV}$
    

$$E_{cm} \approx \sqrt{4 \times 27.5 \times 920}$$

$$E_{cm} \approx \sqrt{101,200}$$

$$E_{cm} \approx 318.12 \text{ GeV}$$

Rounding to three significant figures (matching the 27.5 GeV), we get:

$$E_{cm} \approx 318 \text{ GeV}$$

So, as you can see, the 947.5 GeV of total energy in the lab only provides **318 GeV** of usable energy for creating new particles. This is a fundamental concept in particle physics and the main reason why colliders are so much more powerful than "fixed-target" experiments (where one beam hits a stationary target).

Does that derivation make sense? I can also show you what would happen if one of the particles was at rest, if you're curious!