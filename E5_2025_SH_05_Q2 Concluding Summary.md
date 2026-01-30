

This is an excellent idea. In Particle Physics, "identifying the suspect" always comes down to combining these specific relations.

Here is a condensed **Particle ID Cheat Sheet** optimized for your exam.

---

### 1. Relativistic Kinematics (Speed & Time)

-   **Speed ($\beta$):** The velocity as a fraction of the speed of light.
    
    $$\beta = \frac{v}{c} = \frac{\text{Distance}}{\text{Time} \times c}$$
    
    -   _Useful Constant:_ $c \approx 0.3\,\text{m/ns}$ (or $30\,\text{cm/ns}$).
        
-   **Lorentz Factor ($\gamma$):** How "relativistic" the particle is.
    
    $$\gamma = \frac{1}{\sqrt{1 - \beta^2}}$$
    
    -   _Note:_ If $\beta \to 1$, then $\gamma \to \infty$. If $\beta = 0$, then $\gamma = 1$.
        

---

### 2. Energy Loss (Bethe-Bloch)

This is your primary tool for finding **Electric Charge ($z$)**.

-   **The Concept:** Charged particles lose energy by ionizing atoms as they travel.
    
-   **The "MIP" Rule:** A particle is "Minimum Ionizing" (MIP) when $\beta\gamma \approx 3\text{--}4$.
    
    -   For a standard charge ($z=1$), the energy loss here is roughly:
        
        $$\left\langle -\frac{dE}{dx} \right\rangle_{\text{MIP}} \approx 1\text{--}2\,\frac{\text{MeV cm}^2}{\text{g}}$$
        
-   **Scaling Rule:** Energy loss scales with the **charge squared**.
    
    $$\frac{dE}{dx} \propto z^2$$
    
    -   _Exam Tip:_ If the measured loss is $\approx 2$, then $z=1$. If the loss is $\approx 8$, then $z^2=4 \rightarrow z=2$. If the loss is $\approx 18$, then $z^2=9 \rightarrow z=3$.
        

---

### 3. Magnetic Tracking (Curvature)

This is your tool for finding **Momentum ($p$)**.

-   **The Concept:** A magnetic field bends charged particles into a circle. Higher momentum = straighter line (larger Radius $R$).
    
-   **The "Golden Rule" Formula (Practical Units):**
    
    This is the most important shortcut in high-energy physics.
    
    $$p\,[\text{GeV}/c] = 0.3 \cdot z \cdot B\,[\text{T}] \cdot R\,[\text{m}]$$
    
    -   $z$: Charge number (e.g., 1, 2...)
        
    -   $B$: Magnetic field in Tesla
        
    -   $R$: Radius in meters
        
    -   $0.3$: This constant comes from the speed of light conversion.
        

---

### 4. Mass Reconstruction (Identity)

This combines the previous steps to find the **Rest Mass ($m$)**.

-   **The Relation:**
    
    $$p = \gamma m v = (\beta\gamma) \cdot m \cdot c$$
    
-   **Solving for Mass:**
    
    $$m = \frac{p}{\beta \gamma c}$$
    
    -   _Units:_ If $p$ is in GeV/c, and you divide by $c$, your mass $m$ comes out naturally in **GeV/$c^2$**.
        

---

### 5. Common Particle Suspects (Reference)

Memorize these approximate masses to quickly identify your result.

![[Pasted image 20260128123205.png]]

---

Would you like me to give you a quick "mini-quiz" with different numbers (e.g., a different flight time or energy loss) to test if these formulas stick?