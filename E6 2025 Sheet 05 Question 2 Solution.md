

Hello again! This is an excellent problem. It takes the abstract concepts of dispersion relations ($\omega$ vs. $k$) and makes them concrete with a real-world example and real numbers.

Let's carefully solve this step-by-step.

First, let's list the information we are given. This is always the best way to start a physics problem.

-   **Material:** KBr (Potassium Bromide)
    
-   **Lattice Constant:** $a = 6.659 \text{ \AA}$ (Ångströms)
    
-   **Phonon Type:** Longitudinal Acoustic
    
-   **Frequency:** $\nu = 1.13 \text{ THz}$ (TeraHertz)
    
-   **Wavevector:** $k = \frac{2\pi}{4a}$
    

We are asked to find four things:

1.  Wavelength ($\lambda$)
    
2.  Phase Velocity ($v_p$)
    
3.  Energy ($E$)
    
4.  Quasimomentum ($p$)
    

Let's tackle them one by one.

---

### 1. Wavelength ($\lambda$)

-   **Concept:** The wavevector ($k$) and the wavelength ($\lambda$) have a fundamental, inverse relationship that defines them. This is true for any wave, whether it's light, sound, or a phonon.
    
-   **Formula:** $k = \frac{2\pi}{\lambda}$
    
-   Calculation:
    
    We are given a value for $k$ and we have this definition. We can simply set them equal to each other to solve for $\lambda$.
    
    $$k = \frac{2\pi}{4a}$$
    
    $$k = \frac{2\pi}{\lambda}$$
    
    Therefore:
    
    $$\frac{2\pi}{\lambda} = \frac{2\pi}{4a}$$
    
    By simple inspection, we can see:
    
    $\lambda = 4a$
    
    Now, we just plug in the value for $a$:
    
    $\lambda = 4 \times (6.659 \text{ \AA})$
    
    $\lambda = 26.636 \text{ \AA}$
    
-   **Professor's Note:** This result is very intuitive! It tells us that the specific vibration we are looking at is a wave that has a wavelength exactly four times the lattice constant. So, the vibrational pattern repeats every four unit cells.
    

---

### 2. Phase Velocity ($v_p$)

-   **Concept:** The phase velocity is the speed at which a single point of constant phase on the wave (like the "crest") propagates through the medium. The most basic wave equation relates velocity, frequency, and wavelength.
    
-   Formula: $v_p = \lambda \times \nu$
    
    (Alternatively, we could use $v_p = \omega / k$, where $\omega = 2\pi\nu$. Both give the exact same result!)
    
-   Calculation:
    
    We must be very careful with our units here! We have $\lambda$ in Ångströms ($\text{\AA}$) and $\nu$ in TeraHertz (THz). Let's convert everything to standard SI units (meters and Hertz).
    
    -   $\lambda = 26.636 \text{ \AA} = 26.636 \times 10^{-10} \text{ m}$
        
    -   $\nu = 1.13 \text{ THz} = 1.13 \times 10^{12} \text{ Hz (or } 1/s)$
        
    
    Now, let's multiply them:
    
    $v_p = (26.636 \times 10^{-10} \text{ m}) \times (1.13 \times 10^{12} \text{ s}^{-1})$
    
    $v_p = (26.636 \times 1.13) \times 10^2 \text{ m/s}$
    
    $v_p = 30.098 \times 10^2 \text{ m/s}$
    
    $v_p \approx 3010 \text{ m/s}$
    
-   **Professor's Note:** This is the phase velocity for _this specific phonon_. Since it's an acoustic phonon, this velocity is related to the speed of sound in KBr. A value of $\sim 3000 \text{ m/s}$ is a very typical and reasonable speed of sound in a solid!
    

---

### 3. Energy ($E$)

-   **Concept:** The energy of any quantum "packet" (a _quantum_), whether it's a photon or a phonon, is directly proportional to its frequency. This is the famous Planck-Einstein relation.
    
-   Formula: $E = h\nu$
    
    (where $h$ is Planck's constant, $h \approx 6.626 \times 10^{-34} \text{ J}\cdot\text{s}$)
    
-   Calculation:
    
    Again, we'll use our SI units.
    
    $E = (6.626 \times 10^{-34} \text{ J}\cdot\text{s}) \times (1.13 \times 10^{12} \text{ s}^{-1})$
    
    $E = (6.626 \times 1.13) \times 10^{-22} \text{ J}$
    
    $E \approx 7.487 \times 10^{-22} \text{ J}$
    
    _In solid-state physics, Joules are a bit inconvenient. We prefer to use **milli-electron-Volts (meV)**. Let's convert it._
    
    -   $1 \text{ eV} \approx 1.602 \times 10^{-19} \text{ J}$
        
    -   $E \text{ (in eV)} = (7.487 \times 10^{-22} \text{ J}) / (1.602 \times 10^{-19} \text{ J/eV}) \approx 4.67 \times 10^{-3} \text{ eV}$
        
    -   **$E \approx 4.67 \text{ meV}$**
        
-   **Professor's Note:** This is a very characteristic energy for an acoustic phonon. For comparison, the thermal energy at room temperature ($k_B T$) is about $25 \text{ meV}$.
    

---

### 4. Quasimomentum ($p$)

-   **Concept:** As we've discussed, a phonon isn't a real particle and doesn't have "real" momentum. But it has a **quasimomentum** (or crystal momentum) that behaves _like_ momentum in interactions. This quantity is defined by the phonon's wavevector $k$.
    
-   Formula: $p = \hbar k$
    
    (where $\hbar$ is the reduced Planck constant, $\hbar = h / (2\pi) \approx 1.054 \times 10^{-34} \text{ J}\cdot\text{s}$)
    
-   Calculation:
    
    First, let's get a numerical value for $k$ in SI units (m⁻¹).
    
    $k = \frac{2\pi}{4a} = \frac{2\pi}{4 \times 6.659 \times 10^{-10} \text{ m}}$
    
    $k = \frac{2\pi}{26.636 \times 10^{-10} \text{ m}}$
    
    $k \approx 2.359 \times 10^9 \text{ m}^{-1}$
    
    Now, we can find the quasimomentum $p$:
    
    $p = (1.054 \times 10^{-34} \text{ J}\cdot\text{s}) \times (2.359 \times 10^9 \text{ m}^{-1})$
    
    $p \approx 2.486 \times 10^{-25} \text{ kg}\cdot\text{m/s}$
    
    (Note: The units $\text{J}\cdot\text{s/m}$ are exactly equivalent to $\text{kg}\cdot\text{m/s}$, the standard unit for momentum!)
    

---

### Summary of Results

Here are our final answers, all neatly compiled:

-   **Wavelength:** $\lambda = 26.636 \text{ \AA}$
    
-   **Phase Velocity:** $v_p \approx 3010 \text{ m/s}$
    
-   **Energy:** $E \approx 7.487 \times 10^{-22} \text{ J}$ (or $4.67 \text{ meV}$)
    
-   **Quasimomentum:** $p \approx 2.486 \times 10^{-25} \text{ kg}\cdot\text{m/s}$
    

I hope this detailed walkthrough makes the connection between the theory and the practical calculations clear! Do you have another problem for us to look at?