

![[Pasted image 20260126140817.png]]
![[Pasted image 20260126140826.png]]

Welcome back to class! Grab your seat. We are moving from looking at just one material to comparing two very different "animals" in the solid-state zoo: a **Semiconductor** (InP) and an **Insulator** ($\text{SiO}_2$, which is essentially glass/quartz).

This part of the exercise is fantastic because it mathematically proves why you can build a computer chip out of Indium Phosphide, but if you tried to build one out of window glass, it would never work.

Let's break down the solution in your image step-by-step.

### 1. The Tale of Two Gaps

First, we need to visualize the difference in terrain.

-   **InP (Semiconductor):** As we saw before, the "forbidden gap" is **1.344 eV**. Think of this like a high wall. Hard to jump over, but not impossible.
    
-   **$\text{SiO}_2$ (Insulator):** The problem states the band gap is **8.9 eV**. This is not just a wall; this is Mount Everest. It is enormous in the world of electrons.
    

The question asks us to calculate the probability of finding an electron right at the edge of the conduction band ($E = E_{CB}$) for both materials.

---

### 2. Case 1: Silicon Dioxide ($\text{SiO}_2$)

Let's look at the calculation labeled **(1)** and **(3)** in your solution image.

-   **The Setup:**
    
    -   Band Gap ($E_G$) = $8.9 \text{ eV}$.
        
    -   Fermi Energy ($\mu$): In the middle, so $8.9 / 2 = \mathbf{4.45 \text{ eV}}$.
        
    -   Target Energy ($E$): The bottom of the conduction band, which is at **8.9 eV** (assuming valence band starts at 0).
        
-   **The "Jump" Difficulty:**
    
    We need to see how far the target energy is from the Fermi level:
    
    $$\Delta E = E - \mu = 8.9 \text{ eV} - 4.45 \text{ eV} = \mathbf{4.45 \text{ eV}}$$
    
-   **The Calculation (Eq 3):**
    
    We plug this into the Fermi-Dirac distribution. Note that the professor used $k_B T = 0.0259 \text{ eV}$ here (a slight rounding difference from the previous 0.0258, but that's fine).
    
    $$f(E)_{\text{SiO}_2} = \frac{1}{1 + e^{\frac{4.45}{0.0259}}}$$
    
    The exponent is $4.45 / 0.0259 \approx 171.8$.
    
    $e^{171.8}$ is an astronomically huge number.
    
-   **The Result:**
    
    $$f(E) \approx 2.4 \times 10^{-74}$$
    
    **Professor's Insight:** Do you realize how small $10^{-74}$ is? There are roughly $10^{80}$ atoms in the observable universe. This probability is effectively **zero**. There is essentially **no chance** an electron in a piece of glass will randomly jump to the conduction band at room temperature. This is why glass is such a perfect insulator.
    

---

### 3. Case 2: Indium Phosphide (InP)

Now let's look at the calculation labeled **(2)** and **(4)** in the solution.

-   **The Setup:**
    
    -   Band Gap ($E_G$) = $1.344 \text{ eV}$.
        
    -   Fermi Energy ($\mu$) = $0.672 \text{ eV}$.
        
    -   Target Energy ($E$) = $1.344 \text{ eV}$.
        
-   **The "Jump" Difficulty:**
    
    $$\Delta E = 1.344 - 0.672 = \mathbf{0.672 \text{ eV}}$$
    
-   **The Calculation (Eq 4):**
    
    $$f(E)_{\text{InP}} = \frac{1}{1 + e^{\frac{0.672}{0.0259}}}$$
    
    The exponent is $0.672 / 0.0259 \approx 25.9$.
    
    $e^{25.9}$ is large, but not "universe-breaking" large.
    
-   **The Result:**
    
    $$f(E) \approx 5.39 \times 10^{-12}$$
    

---

### 4. The Final Comparison (and a typo alert!)

Now we compare the two numbers.

-   $\text{SiO}_2$: $10^{-74}$
    
-   $\text{InP}$: $10^{-12}$
    

The text in red at the bottom of your image says:

> _"Bei 300 K ist die Wahrscheinlichkeit... für InP 6 Größenordnung höher als für $\text{SiO}_2$."_
> 
> (At 300 K the probability... for InP is 6 orders of magnitude higher than for $\text{SiO}_2$.)

**Important Note:** I believe your professor made a typo in the text description here.

If you divide the two probabilities:

$$\frac{10^{-12}}{10^{-74}} = 10^{62}$$

The difference is actually **62 orders of magnitude**, not 6!

-   $10^{-12}$ is small (like finding one specific grain of sand on a beach).
    
-   $10^{-74}$ is physically impossible (like finding a specific atom in the entire galaxy).
    

The massive difference between these two numbers is the fundamental definition of why one material conducts (semiconductor) and one blocks (insulator) current at room temperature.

**Would you like me to explain what happens if we heat the $\text{SiO}_2$ up? Would it ever conduct?**