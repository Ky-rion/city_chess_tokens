

This is a fantastic problem because it deals with **Potassium-40 ($^{40}\text{K}$)**, one of the most important isotopes in geology (for dating rocks) and biology (it’s the main source of radioactivity in bananas and human bodies!).

Let’s break this down step-by-step, just like we would on a blackboard.

---

### (a) Reaction Equations and Decay Types

**The Physics:**

We have a parent nucleus, Potassium-40 ($^{40}_{19}\text{K}$), branching into two different daughters. We need to conserve **Charge number ($Z$)** and **Mass number ($A$)** for each path.

1. **Decay to Calcium ($^{40}_{20}\text{Ca}$):**
    
    - The mass number stays $40$, but the proton number increases from $19 \rightarrow 20$.
        
    - To balance the charge, the nucleus must emit a negative charge (an electron).
        
    - This is classic **Beta-minus decay ($\beta^-$)**.
        
    - _Equation:_
        
        $$^{40}_{19}\text{K} \longrightarrow \, ^{40}_{20}\text{Ca} + e^- + \bar{\nu}_e$$
        
    - _(Note: $\bar{\nu}_e$ is the electron antineutrino, required to conserve lepton number)._
        
2. **Decay to Argon ($^{40}_{18}\text{Ar}$):**
    
    - The mass number stays $40$, but the proton number decreases from $19 \rightarrow 18$.
        
    - There are two ways this can happen: emitting a positron ($\beta^+$) or capturing an electron. For $^{40}\text{K}$, the dominant mechanism is **Electron Capture** (often called K-capture because it grabs an electron from the K-shell).
        
    - _Equation:_
        
        $$^{40}_{19}\text{K} + e^- \longrightarrow \, ^{40}_{18}\text{Ar} + \nu_e$$
        
    - _(Note: Here we emit a regular electron neutrino $\nu_e$)._
        

> **Answer:**
> 
> - **To Ca-40:** Beta-minus decay ($\beta^-$).
>     
> - **To Ar-40:** Electron Capture (Elektroneneinfang).
>     

---

### (b) Number of Nuclei in the Sample

**The Physics:**

We are given the **Activity ($A$)**, which tells us how many decays happen per second. We need to find the total number of nuclei ($N$). The bridge between them is the **Decay Constant ($\lambda$)**.

$$A = \lambda \cdot N$$

**Step 1: Convert Half-life to Seconds**

Physics formulas require standard SI units (seconds), but the half-life is given in years.

- $T_{1/2} = 1.25 \times 10^9$ years
    
- Seconds in a year $\approx 365.25 \times 24 \times 3600 \approx 3.156 \times 10^7 \text{ s}$
    

$$T_{1/2} (\text{seconds}) = (1.25 \times 10^9) \times (3.156 \times 10^7) \approx 3.945 \times 10^{16} \text{ s}$$

**Step 2: Calculate the Decay Constant ($\lambda$)**

$$\lambda = \frac{\ln(2)}{T_{1/2}} \approx \frac{0.693}{3.945 \times 10^{16} \text{ s}}$$

$$\lambda \approx 1.757 \times 10^{-17} \text{ s}^{-1}$$

**Step 3: Calculate $N$**

We know $A = 1 \text{ s}^{-1}$ (1 decay per second).

$$N = \frac{A}{\lambda} = \frac{1}{1.757 \times 10^{-17}}$$

$$N \approx 5.69 \times 10^{16}$$

> **Answer:** There are approximately **$5.69 \times 10^{16}$** nuclei of $^{40}\text{K}$ in the sample.

---

### (c) Age of the Sample

**The Physics:**

This is a radio-dating problem. We found $30,000$ Argon atoms. We assume these appeared solely due to the decay of Potassium.

However, there is a catch! **Not every Potassium atom becomes Argon.**

- Only $10.72\%$ become Argon.
    
- The rest ($89.28\%$) become Calcium.
    

**The Logic:**

The rate at which Argon is produced ($R_{Ar}$) is just the branching ratio multiplied by the total activity.

$$R_{Ar} = (\text{Branching Ratio}) \times A_{total}$$

$$R_{Ar} = 0.1072 \times 1 \text{ decay/s} = 0.1072 \text{ Argon atoms/s}$$

**Calculation:**

We have accumulated $N_{Ar} = 3 \times 10^4$ atoms. Since this number is extremely small compared to the total number of K atoms ($10^{16}$), we can assume the Activity ($A$) has been constant during this short time. (We don't need the complex logarithmic dating formula here, a linear approximation is perfect).

$$Time = \frac{\text{Amount Accumulated}}{\text{Production Rate}}$$

$$t = \frac{30,000}{0.1072 \text{ s}^{-1}}$$

$$t \approx 279,850 \text{ seconds}$$

Let's convert that to something human-readable:

$$t \text{ in days} = \frac{279,850}{3600 \times 24} \approx 3.24 \text{ days}$$

> **Answer:** Under the assumption that all Argon came from the decay, the sample is approximately **3.24 days** old.

_(Professor's Note: If this were a geological sample of a rock, we would expect billions of Argon atoms. Finding only 30,000 implies the "clock" was reset—likely by melting or purifying the sample—very recently in the lab!)_