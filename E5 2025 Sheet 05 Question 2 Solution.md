

![[Pasted image 20260128114540.png]]

Hello! Welcome to your first day of Particle Physics "detective school." I am thrilled to be your professor.

In this field, we rarely get to "see" particles directly. Instead, we look at the footprints they leave behind—how fast they move, how much energy they lose in a material, and how they curve in magnetic fields. By combining these clues, we can reconstruct the identity of the invisible suspect.

Let's walk through this solution step-by-step, exactly as if we were at the whiteboard together.

---

### Step 1: How fast is it moving? (Kinematics)

The first clue we have is simple speed. We are told the particle travels **2 meters** in **6.9 nanoseconds**.

In particle physics, we almost always measure speed relative to the speed of light ($c$), which is roughly $3 \times 10^8$ m/s (or exactly $0.3$ meters per nanosecond).

-   **$\beta$ (Beta):** This is just the velocity $v$ divided by the speed of light $c$.
    
    $$\beta = \frac{v}{c} = \frac{\text{distance}}{ \text{time} \times c}$$
    
    $$\beta = \frac{2\,\text{m}}{6.9\,\text{ns} \times 0.3\,\text{m/ns}} \approx \mathbf{0.967}$$
    
    _Professor's Note:_ This particle is moving at 96.7% the speed of light! It is highly relativistic.
    
-   **$\gamma$ (Gamma - The Lorentz Factor):** Because the particle is moving so fast, we need to calculate the relativistic factor $\gamma$. This number tells us how much time is dilating or mass is increasing.
    
    $$\gamma = \frac{1}{\sqrt{1 - \beta^2}}$$
    
    Plugging in our $\beta$:
    
    $$\gamma = \frac{1}{\sqrt{1 - 0.967^2}} \approx \mathbf{3.93}$$
    
-   **$\beta\gamma$:** This combined term appears everywhere in particle physics equations (especially for momentum).
    
    $$\beta\gamma = 0.967 \times 3.93 \approx \mathbf{3.80}$$
    

**Why did we do this?** The hint in the problem asked us to calculate $\beta\gamma$ first. This value ($\approx 3.8$) tells us the particle is in a "sweet spot" called the **Minimum Ionizing** region. This is crucial for the next step.

---

### Step 2: What is the Charge? (Energy Loss)

This is the cleverest part of the solution. We need to find the electric charge ($z$) of the particle.

**The Clue:** The problem states the "Specific Energy Loss" is $8\,\text{MeV}\,\text{cm}^2/\text{g}$.

This value represents how much energy the particle loses as it crashes through the atoms of the detector material.

**The Rule (Bethe-Bloch):** There is a famous equation called the _Bethe-Bloch formula_ that describes this energy loss.

1.  For particles with $\beta\gamma \approx 3\text{--}4$ (which we just found our particle has!), the energy loss is at its **minimum**.
    
2.  For a standard particle with charge +1 (like a proton), this minimum loss is almost always roughly **$2\,\text{MeV}\,\text{cm}^2/\text{g}$**.
    

**The Deduction:**

However, our mystery particle is losing **$8\,\text{MeV}\,\text{cm}^2/\text{g}$**. That is way too high for a standard +1 charge particle.

The Bethe-Bloch formula tells us that energy loss is proportional to the **square of the charge** ($z^2$).

$$\frac{dE}{dx} \propto z^2$$

Let's compare the measured loss to the standard loss:

$$\frac{\text{Measured Loss}}{\text{Standard Loss for } z=1} = \frac{8}{2} = 4$$

Since the ratio is 4, and the loss scales with $z^2$:

$$z^2 = 4 \implies \mathbf{z = 2}$$

**Conclusion:** The particle has a charge of **+2** (twice the charge of an electron/proton).

---

### Step 3: What is the Momentum? (Magnetic Curvature)

Now we look at how the particle curves. Charged particles moving in a magnetic field travel in circles.

-   **The Radius ($R$):** 25 meters.
    
-   **The Magnetic Field ($B$):** 1 Tesla.
    
-   **The Charge ($q$):** We just found $z=2$, so $q = 2e$ ($2 \times 1.6 \times 10^{-19}\,\text{C}$).
    

**The Formula:** The momentum ($p$) relates to the radius of curvature.

$$p = q \cdot B \cdot R$$

_Professor's Trick:_ In particle physics, we use a shortcut formula to get the answer directly in our favorite unit, GeV/c:

$$p\,[\text{GeV}/c] = 0.3 \times z \times B\,[\text{T}] \times R\,[\text{m}]$$

$$p = 0.3 \times 2 \times 1 \times 25 = \mathbf{15\,\text{GeV}/c}$$

_The long way shown in the solution:_

They calculated it in standard SI units (Newton-seconds) first:

$$p = (2 \cdot 1.6 \times 10^{-19}\,\text{C}) \cdot (25\,\text{m}) \cdot (1\,\text{T}) = 8.0 \times 10^{-18}\,\text{Ns}$$

Then converted to GeV/c, arriving at the same answer: **15.0 GeV/c**.

---

### Step 4: What is the Mass? (Identification)

Now we have the momentum ($p$) and the kinematic factors ($\beta$ and $\gamma$). We can weigh the ghost!

**The Formula:** Relativistic momentum is defined as:

$$p = \gamma m v = \gamma m (\beta c)$$

Rearranging to solve for mass ($m$):

$$m = \frac{p}{\beta \gamma c}$$

We know $p = 15\,\text{GeV}/c$ and $\beta\gamma = 3.80$.

$$m = \frac{15.0\,\text{GeV}/c}{3.80 \times c}$$

_(Note: The $c$'s cancel out nicely to give us mass units of $\text{GeV}/c^2$)_

$$m = \frac{15.0}{3.80}\,\text{GeV}/c^2 \approx \mathbf{3.95\,\text{GeV}/c^2}$$

---

### Step 5: The Verdict

Let's look at our suspect profile:

1.  **Charge:** +2
    
2.  **Mass:** $\approx 4\,\text{GeV}/c^2$
    

Let's look at the lineup of known particles:

-   **Proton:** Charge +1, Mass $\approx 1\,\text{GeV}/c^2$. (No match)
    
-   **Electron:** Charge -1, Mass $\approx 0.0005\,\text{GeV}/c^2$. (Definitely not)
    
-   **Alpha Particle (Helium Nucleus):** This consists of 2 protons and 2 neutrons.
    
    -   Charge: 2 protons $\to$ **+2**. (Match!)
        
    -   Mass: 2 protons + 2 neutrons $\approx 4 \times 1\,\text{GeV}/c^2 \to$ **$4\,\text{GeV}/c^2$**. (Match!)
        

**Final Answer:** The particle is an **Alpha particle** (a Helium-4 nucleus).

---

### Helpful summary for your notes:

-   **$\beta$ & $\gamma$:** Tell you the speed and relativistic effects.
    
-   **Energy Loss ($dE/dx$):** Tells you the **Charge** ($z$). Remember the "Minimum Ionizing" value is usually $\approx 2$.
    
-   **Curvature ($R$):** Tells you the **Momentum** ($p$).
    
-   **Momentum + Speed:** Tells you the **Mass** ($m$).
    

Does that help clear up the "detective work" required here? Would you like me to clarify the "0.3" shortcut formula for momentum—it's a lifesaver on exams!