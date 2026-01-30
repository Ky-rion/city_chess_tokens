

![[Pasted image 20260128114221.png]]

Hello there! Welcome to "Introduction to Particle Detector Design." I am delighted to be your guide.

Don't be intimidated by the equations; particle physics is really just about building a very fancy, high-tech onion. We build detectors in concentric layers, wrapped around the collision point, with each layer designed to stop and measure a specific type of particle.

To answer **part (a)** of your question—finding the total radius of this detector—we simply need to calculate the thickness of each "layer" of our onion and add them all up.

Here is the master equation for the total Radius ($R$):

$$R_{total} = R_{pipe} + R_{tracker} + R_{ECAL} + R_{HCAL} + R_{muon}$$

Let's walk through these five components from the inside out, using the solution you provided.

---

### 1. The Beam Pipe ($R_{beam}$)

This is the innermost layer—the actual tube where the protons (or other particles) travel before they collide.

-   **The Problem:** We are given a **diameter** of $4\text{ cm}$.
    
-   **The Physics:** We define radii from the center point (the interaction point).
    
-   **The Calculation:**
    
    $$R_{beam} = \frac{\text{diameter}}{2} = \frac{4\text{ cm}}{2} = 2\text{ cm} = \mathbf{0.02\text{ m}}$$
    

---

### 2. The Tracking Detector ($R_{track}$)

This is usually the most mathematically complex part. The Tracker records the paths of charged particles. It doesn't stop them; it just watches them curve.

-   **The Physics:** We use a magnetic field ($B$) to bend the path of charged particles. The higher the momentum ($p_T$), the straighter the path. By measuring how much the path curves (the "sagitta"), we calculate the momentum.
    
-   **The Formula:** We use the given empirical formula for momentum resolution. We need to rearrange it to solve for $L$ (the length of the detector track, which corresponds to the radius/thickness of this layer).
    
    The formula provided is:
    
    $$\frac{\sigma(p_T)}{p_T} = \frac{\sigma(x)}{a \cdot B \cdot L^2} \sqrt{\frac{720}{N+4}} \cdot p_T$$
    
    -   **$\frac{\sigma(p_T)}{p_T}$:** This is the resolution required ($1.5\%$ or $0.015$).
        
    -   **$\sigma(x)$:** The precision of the silicon detectors ($30\,\mu\text{m}$ or $30 \cdot 10^{-6}\text{ m}$).
        
    -   **$B$:** The magnetic field strength ($4\text{ T}$).
        
    -   **$N$:** The number of measurement planes ($20$).
        
    -   **$p_T$:** The momentum we want to measure ($100\text{ GeV}/c$).
        
-   **The Calculation:**
    
    We rearrange the algebra to solve for $L$:
    
    $$L = \sqrt{ \frac{\sigma(x) \cdot p_T}{a \cdot B \cdot (\text{Resolution})} \sqrt{\frac{720}{N+4}} }$$
    
    Plugging in the numbers from the solution sheet:
    
    $$L = \left( \frac{30 \cdot 10^{-6}\text{ m}}{0.3 \cdot 4\text{ T}} \cdot \sqrt{\frac{720}{24}} \cdot 100 \cdot \frac{1}{0.015} \right)^{\frac{1}{2}}$$
    
    $$L \approx \mathbf{0.96\text{ m}}$$
    
    _Professor's Note: This means our tracker needs to be almost a meter thick to accurately measure the curve of such high-energy particles!_
    

---

### 3. The Electromagnetic Calorimeter ($R_{ECAL}$)

The "ECAL" is the next layer. Its job is to stop electrons and photons and measure their energy.

-   **The Physics:** Dense materials are rated by their "Radiation Length" ($X_0$). This is the characteristic distance an electron travels before losing most of its energy. The problem states we need a depth of $26 X_0$ to fully contain the energy.
    
-   **The Material:** Lead Tungstate ($\text{PbWO}_4$), which has a very short radiation length of $X_0 = 0.89\text{ cm}$.
    
-   **The Calculation:**
    
    $$R_{ECAL} = (\text{Required } X_0) \times (\text{Length per } X_0)$$
    
    $$R_{ECAL} = 26 \times 0.89\text{ cm} = 23.14\text{ cm} \approx \mathbf{0.23\text{ m}}$$
    

---

### 4. The Hadronic Calorimeter ($R_{HCAL}$)

The "HCAL" stops the heavy particles (hadrons like protons, neutrons, pions) that punched right through the ECAL.

-   **The Physics:** Hadrons interact via the strong nuclear force, so we use a different metric called "Interaction Length" ($\lambda_a$). The problem requires a depth of $7\lambda_a$.
    
-   **The Setup:** This is a "Sampling Calorimeter," meaning it's a sandwich. We have heavy "absorber" plates (Brass) to stop particles, and "active" plates (Scintillator) to detect them.
    
    -   Brass thickness: $5\text{ cm}$.
        
    -   Scintillator thickness: $4\text{ mm} = 0.4\text{ cm}$.
        
    -   $\lambda_a$ for Brass: $18.4\text{ cm}$.
        
-   **The Calculation (Step-by-Step):**
    
    1.  **How much Brass do we need?**
        
        The problem assumes _only_ the brass stops the shower. We need 7 interaction lengths of it.
        
        $$\text{Total Brass Depth} = 7 \times 18.4\text{ cm} = 128.8\text{ cm}$$
        
    2.  **How many layers of Brass is that?**
        
        $$\text{Number of Layers} = \frac{128.8\text{ cm}}{5\text{ cm per layer}} = 25.76$$
        
        Since we can't build 0.76 of a layer, we round up to **26 layers**.
        
    3.  **What is the physical thickness?**
        
        Each of those 26 layers consists of a Brass plate AND a Scintillator plate.
        
        $$\text{Thickness per layer} = 5\text{ cm (Brass)} + 0.4\text{ cm (Scint)} = 5.4\text{ cm}$$
        
        $$R_{HCAL} = 26 \text{ layers} \times 5.4\text{ cm} = 140.4\text{ cm} \approx \mathbf{1.40\text{ m}}$$
        

---

### 5. The Muon Chambers ($R_{muon}$)

The outermost layer. Muons are "ghost" particles that travel through everything else. We put huge iron blocks here to finally track them.

-   **The Physics:** By the time particles get here, everything else has been stopped. If you see a track here, it's a muon.
    
-   **The Calculation:** The problem explicitly tells us the iron yoke thickness.
    
    $$R_{muon} = \mathbf{3.00\text{ m}}$$
    

---

### Summary: The Final Tally

Now we simply sum the radius of every layer to find the size of our machine:

$$R_{total} = 0.02\text{ m (Pipe)} + 0.96\text{ m (Track)} + 0.23\text{ m (ECAL)} + 1.40\text{ m (HCAL)} + 3.00\text{ m (Muon)}$$

$$R_{total} = \mathbf{5.61\text{ meters}}$$

So, the total radius of your detector is **5.61 meters**. This means the full detector (diameter) is over 11 meters tall—about the size of a 3-4 story building!

**Would you like to move on to part (b) or shall I explain any of the specific formulas (like the Tracker resolution) in more detail?**