

Here is your "Exam Survival Cheat Sheet" for electron conduction. This covers the key distinctions, formulas, and concepts we just walked through.

### **1. The Two Velocities (Don't mix them up!)**

-   **Drift Velocity ($v_d$):**
    
    -   **What is it?** The slow net movement of the electron "swarm" caused by the electric field (Current).
        
    -   **Magnitude:** Very slow ($\sim \text{mm/s}$).
        
    -   **When to use:** Only when calculating current density $j = -n e v_d$.
        
-   **Fermi Velocity ($v_F$):**
    
    -   **What is it?** The instantaneous speed of electrons at the Fermi energy (the ones actually colliding).
        
    -   **Magnitude:** Very fast ($\sim 10^6 \text{ m/s}$).
        
    -   **Why high?** Due to the Pauli Exclusion Principle, electrons are forced into high energy states even at 0K.
        
    -   **When to use:** For **Mean Free Path ($l$)** and scattering time ($\tau$).
        

---

### **2. Conductivity Formulas ($\sigma$)**

You need to know how to connect the "Lab World" to the "Quantum World."

![[Pasted image 20260127174838.png]]

---

### **3. Calculating Mean Free Path ($l$)**

The "Golden Chain" of calculation:

1.  **Find $\tau$:** Equate the two conductivity formulas above.
    
    $$\tau = \frac{m \cdot \sigma}{n e^2}$$
    
2.  **Find $v_F$:** Depends only on electron density ($n$).
    
    $$v_F = \frac{\hbar}{m} (3\pi^2 n)^{1/3}$$
    
3.  **Find $l$:** Distance = Speed $\times$ Time.
    
    $$l = v_F \cdot \tau$$
    

---

### **4. Temperature Dependence ($\rho$ vs $T$)**

-   **Linear Model (High T):**
    
    -   $\rho(T) \propto T$
        
    -   Caused by scattering off thermal lattice vibrations (phonons).
        
    -   **Formula:** $\rho(T) = \rho_0 + \alpha \cdot T$ (Equation of a line).
        
    -   **Pitfall:** Extrapolating this to $0$ usually gives a "fake" temperature intercept (like the $220\text{K}$ in our problem).
        
-   **Real Behavior (Low T):**
    
    -   **Bloch-Grüneisen Law:** $\rho_{phonon} \propto T^5$ (drops off very fast).
        
    -   **Residual Resistivity ($\rho_0$):** Resistance never hits zero. It hits a floor caused by **impurities and defects**.
        
-   **Matthiessen's Rule:**
    
    $$\rho_{total} = \rho_{thermal}(T) + \rho_{impurity}$$
    
    _(Total Resistance = Shaking Lattice + Static Dirt)_
    

---

### **5. "Professor's Warning" (Unit Traps)**

Measurements in these problems are almost always given in "convenient" units that will break your math if you don't convert them first!

-   **Area ($A$):** Usually given in $\text{mm}^2$.
    
    -   **CONVERT:** $1 \text{ mm}^2 = 10^{-6} \text{ m}^2$.
        
-   **Voltage ($U$):** Usually given in $\text{mV}$.
    
    -   **CONVERT:** $1 \text{ mV} = 10^{-3} \text{ V}$.
        
-   **Length ($L$):** Usually given in $\text{cm}$.
    
    -   **CONVERT:** $1 \text{ cm} = 10^{-2} \text{ m}$.
        

Good luck with your exam preparation! You've got this.