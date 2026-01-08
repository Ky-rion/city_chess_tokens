

Here is a "Cheat Sheet" summary of the key formulas and concepts from this problem. These are the essential tools you would need to solve similar particle identification questions on an exam.

### 1. Cherenkov Radiation

This is your primary tool for determining speed.

-   The Condition: Light is emitted only if the particle velocity ($\beta$) exceeds the speed of light in the medium ($c/n$).
    
    $$\beta \geq \frac{1}{n}$$
    
-   **Thresholds:**
    
    -   If a particle triggers a detector with index $n$, it is **fast** ($\beta > 1/n$).
        
    -   If it _fails_ to trigger it, it is **slow** ($\beta < 1/n$).
        
    -   _Tip:_ You can sandwich the speed of a particle between two values if it triggers one layer but fails the next (e.g., triggers $n=1.05$ but not $n=1.01$).
        

### 2. Relativistic Kinematics

You need these to translate between Speed ($\beta$), Momentum ($p$), and Energy ($E$).

-   Lorentz Factor ($\gamma$):
    
    $$\gamma = \frac{1}{\sqrt{1 - \beta^2}}$$
    
-   Momentum ($p$):
    
    $$p = \gamma m v = \gamma m \beta c$$
    
    (Use this to calculate the minimum momentum required to trigger a Cherenkov detector for a specific mass).
    
-   Total Energy ($E$):
    
    $$E = \sqrt{p^2 c^2 + m^2 c^4} = \gamma m c^2$$
    
-   Useful Relation ($\beta \gamma$):
    
    Sometimes it is easier to work with the combined term $\beta\gamma$:
    
    $$\beta\gamma = \frac{\beta}{\sqrt{1-\beta^2}}$$
    
    Example: For $n=1.1$, $\beta \ge 0.909 \implies \beta\gamma \ge 2.18$.
    

### 3. Energy Loss & Mass Estimation

Used when a particle passes through an absorber (like the Iron plate).

-   Energy Balance:
    
    $$E_{final} = E_{initial} - \Delta E_{loss}$$
    
    $$\Delta \gamma \cdot mc^2 = \Delta E_{loss}$$
    
-   Estimating Mass:
    
    If you know the energy loss ($\Delta E$) and the change in speed ($\Delta \gamma$) caused by an absorber, you can set an upper limit on the mass:
    
    $$mc^2 \leq \frac{\Delta E}{\Delta \gamma}$$
    
    (This was used to identify the electron: huge speed drop + small energy loss = very light particle).
    
-   Typical Energy Loss:
    
    For high-energy particles (minimum ionizing), energy loss in Iron is roughly:
    
    $$\approx 2 \text{ MeV} \cdot \text{cm}^2/\text{g} \times \rho \times \text{thickness}$$
    
    (In this problem: $\approx 16 \text{ MeV}$ for 1 cm of Iron).
    

### 4. Particle Signatures

Common "fingerprints" to look for in detector diagrams.

-   **Photon ($\gamma$):**
    
    -   **Tracking:** Invisible (neutral).
        
    -   **Conversion:** Suddenly creates two tracks ($e^+ e^-$) in the middle of the volume (Pair Production).
        
-   **Neutron ($n$):**
    
    -   **Tracking:** Invisible (neutral).
        
    -   **Cherenkov:** Invisible (no charge).
        
    -   **Secondary:** Can only be seen if it hits a nucleus hard enough to create fast charged fragments (requires high energy, $E \gg 100 \text{ MeV}$).
        
-   **Electron ($e^\pm$):**
    
    -   Very light ($0.511 \text{ MeV}$). Even small momentum gives $\beta \approx 1$. Often triggers _all_ Cherenkov thresholds unless explicitly stopped.
        
-   **Pion vs. Kaon:**
    
    -   Heavier particles (Kaons) need **more momentum** to reach the same speed ($\beta$) as lighter particles (Pions).
        
    -   At the same momentum, the lighter particle (Pion) lights up more Cherenkov layers.
        

### 5. Standard Masses (for context)

-   **Electron:** $\approx 0.5 \text{ MeV}/c^2$
    
-   **Pion ($\pi^\pm$):** $\approx 140 \text{ MeV}/c^2$
    
-   **Kaon ($K^\pm$):** $\approx 494 \text{ MeV}/c^2$
    
-   **Proton/Neutron:** $\approx 938 \text{ MeV}/c^2$
    

Would you like me to clarify any of these formulas or show you how to plug the numbers into them?