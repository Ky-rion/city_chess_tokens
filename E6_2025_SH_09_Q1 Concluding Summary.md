

An exam cheat sheet is a great idea. In solid-state physics, knowing _why_ a formula works is often just as important as the formula itself, so I’ve included brief "concept tags" next to the math.

Here is your **Drude-Sommerfeld Transport Cheat Sheet**.

---

### **1. Core Variables**

-   **$\vec{k}$**: Wavevector (The quantum "address" of the electron state).
    
-   **$\vec{p} = \hbar\vec{k}$**: Momentum (The connection between quantum $\vec{k}$ and classical motion).
    
-   **$\vec{v} = \frac{\hbar\vec{k}}{m}$**: Velocity.
    
-   **$\tau$ (Tau)**: Relaxation Time (Average time between collisions/scattering events).
    
-   **$n$**: Electron density (Number of electrons per unit volume).
    

---

### **2. The Three-Step Derivation**

#### **Step 1: Acceleration (The Push)**

-   **Concept:** Electric field $\vec{E}$ applies force, changing momentum over time.
    
-   **Formula:**
    
    $$\vec{F} = -e\vec{E} = \hbar \frac{\partial \vec{k}}{\partial t}$$
    
    $$\Rightarrow \left. \frac{\partial \vec{k}}{\partial t} \right|_{el} = -\frac{e\vec{E}}{\hbar}$$
    
    _Note: The sphere shifts linearly with time if no scattering exists._
    

#### **Step 2: Relaxation (The Friction)**

-   **Concept:** When the field is off, scattering restores equilibrium exponentially ($\delta \vec{k} \propto e^{-t/\tau}$).
    
-   **Formula:**
    
    $$\left. \frac{\partial \vec{k}}{\partial t} \right|_{scat} = -\frac{\delta \vec{k}}{\tau}$$
    
    _Note: The further from equilibrium ($\delta \vec{k}$), the faster it relaxes._
    

#### **Step 3: Steady State (Equilibrium)**

-   **Concept:** Constant current means the "Push" equals the "Friction." Total change is zero.
    
-   **Condition:**
    
    $$\frac{d\vec{k}}{dt} = \left. \frac{\partial \vec{k}}{\partial t} \right|_{el} + \left. \frac{\partial \vec{k}}{\partial t} \right|_{scat} = 0$$
    
-   **Result (The Shift):**
    
    $$\delta \vec{k} = -\frac{e\tau}{\hbar}\vec{E}$$
    
    _Note: This shift $\delta \vec{k}$ is constant in time for a DC field._
    

---

### **3. The Final Transport Formulas**

#### **Current Density ($\vec{J}$)**

-   **Definition:** $\vec{J} = -e n \vec{v}_{drift}$
    
-   **Substitute $\vec{v}$:** $\vec{J} = -e n \left( \frac{\hbar}{m} \delta \vec{k} \right)$
    
-   **Final Form:**
    
    $$\vec{J} = \frac{n e^2 \tau}{m} \vec{E}$$
    

#### **Electrical Conductivity ($\sigma$)**

-   **Definition:** Derived from Ohm's Law $\vec{J} = \sigma \vec{E}$.
    
-   **The Drude Formula:**
    
    $$\sigma = \frac{n e^2 \tau}{m}$$
    

---

### **4. "Sanity Check" Concepts (For Conceptual Questions)**

-   **Why is current constant?** Because the acceleration from the field is exactly balanced by the deceleration from scattering events.
    
-   **What increases conductivity?**
    
    -   **Higher $n$**: More carriers (metals vs semiconductors).
        
    -   **Higher $\tau$**: Less scattering (colder temperatures, purer crystals).
        
    -   **Lower $m$**: Lighter effective mass (easier to accelerate).
        

Good luck with your exam preparation! Is there anything else you'd like to review?