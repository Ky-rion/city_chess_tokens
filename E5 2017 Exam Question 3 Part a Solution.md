

We are jumping from the massive scale of particle accelerators to the quantum probability of the atomic nucleus. This is a classic nuclear physics problem involving **Bismuth-212 ($^{212}\text{Bi}$)**.

This isotope is particularly interesting because it "can't decide" how to decay—it has two options! This is called a **branching decay**.

Here is the translation of the setup:

> **Isotope:** $^{212}_{83}\text{Bi}$ (Bismuth-212)
> 
> **Half-life ($T_{1/2}$):** 60 minutes
> 
> **Decay Modes:**
> 
> - **64%** via $\beta^-$-decay into Polonium (Po)
>     
> - **36%** via $\alpha$-decay into Thallium (Tl)
>     

---

### (a) Reaction equations with mass and atomic numbers

**The Professor's Insight:**

To write these equations, we must conserve two things:

1. **Mass Number ($A$, top number):** The total number of protons + neutrons must stay the same.
    
2. **Atomic Number ($Z$, bottom number):** The total charge must be conserved.
    

**1. Alpha Decay ($\alpha$):**

An $\alpha$-particle is a Helium nucleus ($^4_2\text{He}$). It takes away 4 mass units and 2 protons.

- Parent: $^{212}_{83}\text{Bi}$
    
- Daughter Mass ($A$): $212 - 4 = 208$
    
- Daughter Charge ($Z$): $83 - 2 = 81$ (Element 81 is Thallium, Tl)
    

$${}^{212}_{83}\text{Bi} \longrightarrow {}^{208}_{81}\text{Tl} + {}^{4}_{2}\text{He}$$

**2. Beta Minus Decay ($\beta^-$):**

A neutron turns into a proton, emitting an electron ($e^-$) and an electron-antineutrino ($\bar{\nu}_e$). The mass number stays the same, but the atomic number goes _up_ by 1.

- Parent: $^{212}_{83}\text{Bi}$
    
- Daughter Mass ($A$): $212$ (unchanged)
    
- Daughter Charge ($Z$): $83 + 1 = 84$ (Element 84 is Polonium, Po)
    

$${}^{212}_{83}\text{Bi} \longrightarrow {}^{212}_{84}\text{Po} + e^- + \bar{\nu}_e$$

---

### (b) Determine the partial widths of both decays.

**The Professor's Insight:**

In particle physics, we often measure "lifetime" in terms of energy width ($\Gamma$), using the Uncertainty Principle ($\Delta E \Delta t \approx \hbar$).

- **Total Width ($\Gamma_{tot}$):** Represents the total probability of decay.
    
- **Partial Width ($\Gamma_i$):** Represents the probability of a _specific_ decay channel.
    

**Step 1: Calculate the Total Width**

First, we find the decay constant $\lambda$ in seconds.

$$T_{1/2} = 60 \text{ min} = 3600 \text{ s}$$

$$\lambda = \frac{\ln 2}{T_{1/2}} \approx \frac{0.693}{3600 \text{ s}} \approx 1.925 \times 10^{-4} \text{ s}^{-1}$$

Now, convert this rate into energy units (eV) using the reduced Planck constant $\hbar \approx 6.582 \times 10^{-16} \text{ eV}\cdot\text{s}$.

$$\Gamma_{tot} = \hbar \cdot \lambda$$

$$\Gamma_{tot} = (6.582 \times 10^{-16} \text{ eV}\cdot\text{s}) \cdot (1.925 \times 10^{-4} \text{ s}^{-1})$$

$$\Gamma_{tot} \approx 1.267 \times 10^{-19} \text{ eV}$$

**Step 2: Calculate Partial Widths**

The partial width is just the total width multiplied by the branching fraction (percentage).

**For Beta Decay (64%):**

$$\Gamma_{\beta} = 0.64 \times \Gamma_{tot} \approx \mathbf{8.11 \times 10^{-20} \text{ eV}}$$

**For Alpha Decay (36%):**

$$\Gamma_{\alpha} = 0.36 \times \Gamma_{tot} \approx \mathbf{4.56 \times 10^{-20} \text{ eV}}$$

---

### (c) Activity of a sample of $10^5$ nuclei? Activity after one day?

**The Professor's Insight:**

"Activity" ($A$) is just the number of decays per second. It's measured in Becquerels (Bq).

**1. Initial Activity ($A_0$)**

We have $N_0 = 10^5$ nuclei. We already calculated $\lambda \approx 1.925 \times 10^{-4} \text{ s}^{-1}$.

$$A_0 = \lambda \cdot N_0$$

$$A_0 = (1.925 \times 10^{-4} \text{ s}^{-1}) \cdot 10^5$$

$$A_0 = \mathbf{19.25 \text{ Bq}}$$

_(This means roughly 19 decays per second. A very weak source!)_

**2. Activity after 1 Day ($A(t)$)**

This is a trick question to test your intuition!

- Half-life = 1 hour ($60$ min).
    
- Time elapsed = 1 day = 24 hours.
    
- That means **24 half-lives** have passed.
    

Each half-life cuts the amount in half. So we multiply by $(1/2)^{24}$.

$$A(1\text{d}) = A_0 \cdot \left(\frac{1}{2}\right)^{24}$$

$$(1/2)^{24} \approx \frac{1}{16,777,216} \approx 6 \times 10^{-8}$$

$$A(1\text{d}) = 19.25 \cdot (6 \times 10^{-8}) \approx \mathbf{1.15 \times 10^{-6} \text{ Bq}}$$

**Answer:** After one day, the activity is effectively **zero**. There is statistically likely to be no radioactive Bismuth left in your sample.

---

### (d) Decay chain from Thorium-232 to Bismuth-212

**The Professor's Insight:**

We are looking at a "family tree" of elements. We start at ancestor $^{232}_{90}\text{Th}$ and end at descendant $^{212}_{83}\text{Bi}$.

We need to count how many $\alpha$ and $\beta$ steps it took to get there.

- **Alpha ($\alpha$):** Change in $A = -4$. Change in $Z = -2$.
    
- **Beta ($\beta^-$):** Change in $A = 0$. Change in $Z = +1$.
    

**Step 1: Count Alphas using Mass Number ($A$)**

Only alpha decays change the mass number.

- Start Mass: 232
    
- End Mass: 212
    
- Total Mass Loss: $\Delta A = 232 - 212 = 20$
    

Since each alpha removes 4 mass units:

$$\text{Number of } \alpha = \frac{20}{4} = \mathbf{5}$$

**Step 2: Count Betas using Atomic Number ($Z$)**

Now we look at the charge ($Z$).

- Start Z: 90
    
- End Z: 83
    
- Total Z change required: $83 - 90 = -7$
    

Let's see what the 5 alphas did to the charge:

$$Z_{\text{change from } \alpha} = 5 \times (-2) = -10$$

Wait! If we only had alphas, we would be at $Z = 90 - 10 = 80$.

But we need to end up at $Z = 83$.

We are "short" by $+3$ protons. Since each $\beta$-decay adds $+1$ to $Z$:

$$\text{Number of } \beta = 83 - 80 = \mathbf{3}$$

**Final Answer:**

The decay chain from $^{232}\text{Th}$ to $^{212}\text{Bi}$ involves **5 $\alpha$-decays** and **3 $\beta$-decays**.

---

### Professor's Check-in

You have now covered:

1. **Accelerator kinematics** (colliding muons)
    
2. **Particle Detection** (Geiger counters and tracking)
    
3. **Radioactivity** (Decay chains and widths)
    

This covers the "Lifecycle" of a particle physics experiment! Do you feel confident with these concepts, or would you like to review any specific part, like the "Partial Width" concept which is often confusing for students?