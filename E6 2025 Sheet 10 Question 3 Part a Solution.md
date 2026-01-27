

![[Pasted image 20260126140759.png]]

Hello! Welcome to Solid State Physics 101. I am delighted to be your guide. Don't worry if this looks intimidating at first—solid state physics is essentially just accounting for electrons, figuring out where they live and how much energy they have to pay to live there.

Let's break down **Part (a)** of your exercise using the solution provided by your other professor.

### 1. The Setup: The "Landscape" of the Electron

First, imagine an electron inside a crystal of Indium Phosphide (InP). It's not free to have just _any_ energy. It lives in a landscape with two main territories separated by a forbidden canyon.

-   **The Valence Band ($E_V$):** Think of this as the "ground floor." It is full of electrons that are stuck to their atoms. They don't move around much.
    
-   **The Band Gap ($E_G$):** This is the "forbidden canyon." No electron is allowed to exist here. In your problem, this gap is **1.344 eV** wide.
    
-   **The Conduction Band ($E_C$):** This is the "upper floor." If an electron gets enough energy to jump up here, it is free to roam and conduct electricity.
    

**Crucial Step:** To do any math, we need to decide where our "zero" height is. The problem statement says "measured from the valence band edge."

-   So, let's set the Valence Band edge to **0 eV**.
    
-   This means the Conduction Band edge is at **1.344 eV**.
    

---

### 2. The Players

Now, let's identify the specific values your other professor used in the solution (the red text in your second image).

**A. The Fermi Energy ($E_F$)**

The Fermi Energy is the most important concept in this course. It is the "sea level" of probability. It represents the chemical potential ($\mu$). The problem tells us to **assume it lies in the middle of the band gap.**

-   Math: $E_F = \frac{\text{Band Gap}}{2}$
    
-   Calculation: $E_F = \frac{1.344 \text{ eV}}{2} = \mathbf{0.672 \text{ eV}}$
    

**B. The Target Energy ($E$)**

The question asks for the probability of finding an electron at a specific energy: $E = E_G + k_B T$.

-   $E_G$ is the top of the gap (1.344 eV).
    
-   $k_B T$ is the "Thermal Energy." At room temperature ($300 \text{ K}$), the universe gives particles a little kick of kinetic energy. This "kick" is worth about **0.0258 eV**.
    
-   So, we are looking for an electron that has jumped across the gap _and_ has a tiny bit of extra thermal energy.
    
-   Calculation: $E = 1.344 \text{ eV} + 0.0258 \text{ eV} = \mathbf{1.3699 \text{ eV}}$
    

---

### 3. The Calculation: The Fermi-Dirac Distribution

Now we ask the big question: **What is the probability an electron is actually up there?**

To answer this, we use the **Fermi-Dirac Distribution function**, which is equation (2) in your image. This formula tells us the probability $f(E)$ that a state at energy $E$ is occupied.

$$f(E) = \frac{1}{1 + e^{\frac{E - \mu}{k_B T}}}$$

Let's plug in the numbers your professor used in the solution image:

1.  **The Energy Difference ($E - \mu$):** This is the numerator of the exponent. It asks: "How much higher is this state than the average sea level ($E_F$)?"
    
    $$1.3699 \text{ eV} - 0.672 \text{ eV} = 0.6979 \text{ eV}$$
    
2.  **The Ratio:** We divide that difference by the thermal energy ($k_B T$). This compares the height of the jump to the available thermal energy.
    
    $$\frac{0.6979 \text{ eV}}{0.0258 \text{ eV}} \approx 27.05$$
    
3.  **The Exponential:** Now we calculate $e^{27.05}$. This is a **massive** number. It means the energy required is _way_ higher than the thermal energy available.
    
4.  **The Final Result:**
    
    $$f(E) \approx \frac{1}{1 + \text{huge number}} \approx \frac{1}{\text{huge number}}$$
    
    $$f(E) = \mathbf{1.98 \times 10^{-12}}$$
    

### 4. Professor's Interpretation

What does this number mean?

The result $1.98 \times 10^{-12}$ is roughly **2 in a trillion**.

This means that at room temperature, it is **extremely unlikely** to find an electron at this energy level in Indium Phosphide. The band gap (1.344 eV) is simply too wide for electrons to jump across it just using room temperature heat. The electrons are mostly stuck downstairs in the valence band.

This is why InP is a semiconductor (and a fairly resistive one in the dark); without extra energy (like light or a voltage), there are almost no electrons in the conduction band to carry current.

---

**Would you like to try part (b) next, or do you have questions about where the $0.0258 \text{ eV}$ value came from?**