

That is a fantastic idea! A "cheat sheet" is the perfect way to consolidate what we just covered. This problem touched on almost every major concept in relativistic kinematics, so having these formulas handy will serve you well for many other problems.

Here is your **Relativistic Kinematics Cheat Sheet** based on the Belle-II problem.

### 1. The "Golden" Energy-Momentum Relation

This is the most important equation in the course. It relates Energy ($E$), Momentum ($p$), and Mass ($m$).

- **General Formula:** $E^2 = (pc)^2 + (mc^2)^2$
    
- **Natural Units ($c=1$):** $E^2 = p^2 + m^2$
    
- **Massless Approximation ($m \approx 0$):** $E \approx p$ (or $E \approx pc$)
    
    - _Use when:_ $E \gg m$ (Ultra-relativistic limit, e.g., $7 \text{ GeV}$ electrons).
        

---

### 2. Center-of-Mass Energy ($\sqrt{s}$)

This is the total "available" energy for creating new particles in a collision.

- **Invariant Mass Formula:** $s = (E_{tot})^2 - (\vec{p}_{tot})^2$
    
- **For Head-on Collisions:**
    
    - $E_{tot} = E_1 + E_2$
        
    - $|\vec{p}_{tot}| = |p_1 - p_2|$ (Be careful with signs! Opposite directions subtract).
        

---

### 3. Decay Kinematics (Two-Body Decay)

When a parent particle ($M$) at rest decays into two daughters ($m_1, m_2$).

- **Momentum Conservation:** The daughters fly back-to-back with equal momentum $|\vec{p}|$.
    
- **Energy Conservation:** $M = E_1 + E_2 = \sqrt{m_1^2 + p^2} + \sqrt{m_2^2 + p^2}$
    
- **Symmetric Decay ($m_1 = m_2 = m$):**
    
    $$|\vec{p}| = \sqrt{\frac{M^2}{4} - m^2}$$
    
    - _Note:_ If $M \approx 2m$, the momentum $|\vec{p}|$ will be very small (non-relativistic daughters).
        
- **Massless Decay ($m_1 = m_2 \approx 0$):**
    
    $$|\vec{p}| = \frac{M}{2}$$
    
    - _Use when:_ Decaying into neutrinos, photons, or very light particles relative to the parent.
        

---

### 4. Lorentz Transformations & Boosts

Moving from the "Center-of-Mass" (CMS) frame to the "Lab" frame.

- **Velocity of CMS ($\beta$):**
    
    $$\beta_{CMS} = \frac{p_{tot, Lab}}{E_{tot, Lab}}$$
    
    - _Example:_ $\beta = \frac{7-4}{7+4} = \frac{3}{11}$
        
- **Gamma Factor ($\gamma$):**
    
    $$\gamma = \frac{1}{\sqrt{1-\beta^2}}$$
    
- **Momentum-Speed Relation:**
    
    $$p = \gamma m v \quad \rightarrow \quad \frac{p}{m} = \beta\gamma$$
    
    - _Use when:_ You need to prove a particle is non-relativistic (if $\beta\gamma \ll 1$).
        

---

### 5. Flight Distance & Lifetime

How far a particle flies before decaying.

- **Time Dilation:**
    
    $$t_{Lab} = \gamma \tau$$
    
    (where $\tau$ is the proper lifetime given in the problem).
    
- **Distance Formula:**
    
    $$x = v_{Lab} \times t_{Lab} = (\beta c) \times (\gamma \tau) = \beta\gamma c \tau$$
    
    - _Shortcut:_ If you have momentum, use $x = \frac{p}{m} c \tau$.
        

---

### 6. Particles in Magnetic Fields

How a charged particle curves in a detector.

- **The Practical Formula:**
    
    $$p_T [\text{GeV}/c] = 0.3 \cdot B [\text{T}] \cdot R [\text{m}]$$
    
- **Transverse Momentum ($p_T$):**
    
    - The magnetic field only bends the momentum _perpendicular_ to the field lines.
        
    - If the field is along the beam ($z$), then $p_T$ is invariant under boosts along $z$.
        
    - **Max Radius:** Occurs when the particle is emitted perpendicular to the beam ($p = p_T$).
        

---

### Useful Constants (Memorize these!)

- **Speed of Light:** $c \approx 3 \times 10^8 \text{ m/s}$
    
- **Conversion Factor:** $1 \text{ fm} \approx 5 \text{ GeV}^{-1}$ (useful for cross-sections, though not used here).
    
- **Electron Mass:** $\approx 0.511 \text{ MeV}$
    
- **Proton Mass:** $\approx 938 \text{ MeV} \approx 1 \text{ GeV}$
    

Good luck with your exam! You have a solid grasp of these concepts now. Just remember to draw a picture for every collision—it saves you from sign errors every time!