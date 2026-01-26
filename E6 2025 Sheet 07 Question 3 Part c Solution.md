

![[Pasted image 20260125185716.png]]

Welcome back to class! You are doing an excellent job following along. We have defined the system (Part a) and measured the bond strength (Part b).

Now, in **Part (c)**, we are going to calculate the **Internal Energy** of the chain.

This is where Thermodynamics meets Quantum Mechanics. We want to know: _How much energy is actually stored in these vibrating atoms when the temperature is 1 Kelvin?_

---

### 1. Translating the Problem

**German:** _"Bestimmen Sie nun die innere Energie pro Einheitslänge des 1D-Gitters... für T = 1K."_

**English:** "Determine now the internal energy per unit length ($u = U/L$) of the 1D lattice for Temperature $T = 1\text{K}$."

**The Setup:**

-   We need to calculate $u$ (energy density).
    
-   **Temperature ($T$):** $1\text{K}$. (This is very cold! Near absolute zero).
    
-   **Debye Temperature ($\Theta_D$):** $\approx 64\text{K}$. (This tells us the temperature scale where all vibrational modes would be active).
    
-   **Hint:** The problem gives you the value of a tricky integral: $\int_0^{64} \frac{x}{e^x-1}dx = 1.64$.
    

---

### 2. The Physics: Adding up the Energy

The formula given in the problem looks scary, but let's take it apart. It is a sum (integral) of the energy of every single vibrational mode.

$$u = \int_{0}^{\omega_D} \underbrace{\frac{D(\omega)}{L}}_{\text{Mode Density}} \cdot \underbrace{\frac{\hbar \omega}{e^{\beta \hbar \omega} - 1}}_{\text{Average Energy per Mode}} d\omega$$

Here is what the pieces mean:

1.  **$\frac{D(\omega)}{L}$**: This is our "Density of States" per meter. It tells us how many vibrational modes exist in one meter of the chain. From the problem hint, we know this is a constant: $\frac{1}{\pi v_s}$.
    
2.  **$\hbar \omega$**: This is the energy of a single **phonon** (a quantum of sound energy).
    
3.  **$\frac{1}{e^{\beta \hbar \omega} - 1}$**: This is the **Planck Distribution** (or Bose-Einstein distribution). It tells us the _average number of phonons_ existing at that frequency for a given temperature.
    

So, the logic is:

**(Modes per meter) $\times$ (Energy per phonon) $\times$ (Number of phonons) = Total Energy Density.**

---

### 3. The Math: The "Substitution Trick"

Physicists hate integrating complex exponentials directly. We always use a substitution to make the variables dimensionless (pure numbers).

We define a new variable $x$:

$$x = \frac{\hbar \omega}{k_B T}$$

-   This represents the ratio of "phonon energy" to "thermal energy."
    

Now we have to swap out all the $\omega$ terms for $x$ terms:

1.  **Frequency:** $\omega = \frac{k_B T}{\hbar} x$
    
2.  **Differential:** $d\omega = \frac{k_B T}{\hbar} dx$
    
3.  **Upper Limit:** When $\omega = \omega_D$, then $x = \frac{\hbar \omega_D}{k_B T}$.
    
    -   _Pro-Tip:_ The quantity $\frac{\hbar \omega_D}{k_B}$ is defined as the **Debye Temperature ($\Theta_D$)**.
        
    -   So the upper limit is simply $\frac{\Theta_D}{T}$.
        
    -   Given $\Theta_D = 64\text{K}$ and $T = 1\text{K}$, our upper limit is **64**.
        

---

### 4. The Derivation (Walking through the Professor's Solution)

Let's look at the red text in the solution line by line.

**Step 1: Pull out constants.**

Since $D(\omega)/L = \frac{1}{\pi v_s}$, we move it outside the integral.

$$u = \frac{1}{\pi v_s} \int_{0}^{\omega_D} \frac{\hbar \omega}{e^{\beta \hbar \omega} - 1} d\omega$$

**Step 2: Apply the substitution ($x$).**

We replace $\omega$ and $d\omega$ with the $x$ expressions we found above.

$$u = \frac{1}{\pi v_s} \int_{0}^{\Theta_D/T} \underbrace{\left( \frac{\hbar k_B T x}{\hbar} \right)}_{\text{was } \hbar \omega} \frac{1}{e^x - 1} \underbrace{\left( \frac{k_B T}{\hbar} dx \right)}_{\text{was } d\omega}$$

_Notice that one $\hbar$ cancels out in the first term, but we divide by another $\hbar$ in the $d\omega$ term._

Grouping the constants together:

$$u = \frac{1}{\pi v_s} \frac{(k_B T)^2}{\hbar} \int_{0}^{64} \frac{x}{e^x - 1} dx$$

**Step 3: Use the Hint.**

The problem stated: $\int_0^{64} \frac{x}{e^x-1}dx = 1.64$.

So we replace the entire integral with **1.64**.

$$u = 1.64 \frac{(k_B T)^2}{\pi \hbar v_s}$$

---

### 5. The Final Calculation

Now we just plug in the numbers. This is where most students make calculator errors, so be careful!

-   $k_B = 1.38 \times 10^{-23} \text{ J/K}$ (Boltzmann constant)
    
-   $\hbar = 1.054 \times 10^{-34} \text{ Js}$ (Reduced Planck constant)
    
-   $v_s = 796 \text{ m/s}$ (Speed of sound from Part a)
    
-   $T = 1 \text{K}$
    

$$u = 1.64 \times \frac{(1.38 \times 10^{-23})^2}{\pi \times (1.054 \times 10^{-34}) \times 796}$$

**Numerator:**

$1.64 \times (1.38 \times 10^{-23})^2 \approx 3.12 \times 10^{-46}$

**Denominator:**

$\pi \times 1.054 \times 10^{-34} \times 796 \approx 2636 \times 10^{-34} \approx 2.64 \times 10^{-31}$

**Result:**

$$u = \frac{3.12 \times 10^{-46}}{2.64 \times 10^{-31}} \approx 1.18 \times 10^{-15} \text{ J/m}$$

The solution provided gives **$1.19 \times 10^{-15} \text{ J/m}$** (likely due to slightly different rounding of constants).

---

### Professor's Summary

The internal energy density is **$1.19 \times 10^{-15}$ Joules per meter**.

This is an **incredibly small amount of energy**.

Why?

1.  **Temperature is low ($1\text{K}$):** There isn't much thermal energy available to excite the atoms.
    
2.  **Quantum Mechanics:** Because $T \ll \Theta_D$ (1K is much less than 64K), most of the high-frequency vibrational modes are "frozen out." They can't be activated because there isn't enough thermal energy to create even a single phonon in those modes.
    

**Next Step:**

That concludes the three parts of this specific problem! You have successfully analyzed the structure ($N$), the bonds ($K$), and the energy ($u$) of a 1D quantum crystal.

Would you like to try a similar problem in **3 Dimensions** (the 3D Debye Model), or would you like to explore what happens to the **Heat Capacity ($C_v$)** of this chain as we change the temperature? (That is usually the favorite exam question!).