

![[Pasted image 20260125184619.png]]

This is the final lap! Part (d) takes the formula we derived and the parameters we found and asks us to simulate what happens at extreme temperatures.

This is a great exercise because it demonstrates the "Thermometer" concept I mentioned earlier. Let’s break down the calculations and, more importantly, the **physical meaning** behind these huge differences in numbers.

### 1. Translation: The Task

**The Question (Image 4):**

> _d) Berechnen Sie die Intensitätsverhältnisse der entsprechenden Stokes und Antistokes Linien bei T = 70 K und T = 700 K._
> 
> **Translation:**
> 
> "Calculate the intensity ratios of the corresponding Stokes and Anti-Stokes lines at T = 70 K and T = 700 K."

**The Solution (Image 5):**

> _Verwenden von Gleichung 15 und einsetzen der entsprechenden Temperaturen... liefert die neuen Verhältnisse:_
> 
> $\frac{I_S}{I_{AS}}(70K) = 39140$ and $\frac{I_S}{I_{AS}}(700K) = 2.37$
> 
> **Translation:**
> 
> "Using Equation 15 and inserting the corresponding temperatures... yields the new ratios:
> 
> Ratio at 70K = 39,140
> 
> Ratio at 700K = 2.37
> 
> The intensity of the Anti-Stokes scattering increases because at higher temperatures more excited states exist, which favor Anti-Stokes scattering."

---

### 2. The Physics: Cold vs. Hot

Before we check the math, let's visualize what is happening inside the crystal using the Boltzmann distribution.

-   **Ground State (Level 0):** This is where molecules sit when they are "cold."
    
-   **Excited State (Level 1):** This is where molecules must be for **Anti-Stokes** scattering to happen. Remember, Anti-Stokes needs to _steal_ energy from a vibration that already exists.
    

**Scenario A: The Deep Freeze (70 K)**

70 Kelvin is liquid nitrogen temperature. It is very cold.

-   **Physics:** There is very little thermal energy available ($k_B T$). Almost 100% of the molecules are frozen in the Ground State.
    
-   **Result:** There is almost no one in the Excited State to steal energy from. The Anti-Stokes signal should be basically zero.
    

**Scenario B: The Oven (700 K)**

700 Kelvin is over 400°C.

-   **Physics:** There is a lot of thermal energy. Molecules are vigorously vibrating. A significant population has been kicked up into the Excited State.
    
-   **Result:** There are plenty of targets for Anti-Stokes scattering. The signal should be strong.
    

---

### 3. The Calculation

We use the "Master Formula" derived in Part (b), which combines the "frequency factor" (Classics) and the "Boltzmann factor" (Quantum):

$$\text{Ratio} = \frac{I_S}{I_{AS}} = \underbrace{\frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4}}_{\text{Frequency Factor}} \cdot \underbrace{e^{\frac{h\nu_M}{k_B T}}}_{\text{Boltzmann Factor}}$$

From Part (c), we already know our constants:

-   $\nu_0 = 5.8235 \times 10^{14}$ Hz
    
-   $\nu_M = 1.5739 \times 10^{13}$ Hz
    
-   **Frequency Factor:** $\frac{(5.82 - 0.15)^4}{(5.82 + 0.15)^4} \approx 0.81$ (This part stays constant!)
    

Now we just change $T$ in the exponent.

#### **Case 1: T = 70 K**

We plug $T=70$ into the exponent term:

$$\text{Exponent} = \frac{(6.626 \times 10^{-34})(1.5739 \times 10^{13})}{(1.38 \times 10^{-23})(70)} \approx 10.8$$

Now, calculate $e^{10.8}$:

$$e^{10.8} \approx 49,000$$

Combine with the frequency factor (approx 0.81):

$$\text{Ratio} \approx 0.81 \times 49,000 \approx \mathbf{39,690}$$

_(Note: Small differences due to rounding are expected, but it matches the solution's order of magnitude perfectly)._

**Conclusion for 70K:** The ratio is ~39,000 to 1.

For every **39,000** Stokes photons you detect, you see only **1** Anti-Stokes photon. In a real lab, the Anti-Stokes peak would completely disappear from the graph.

#### **Case 2: T = 700 K**

We plug $T=700$ into the exponent term. Since T is 10x larger, the exponent is 10x smaller:

$$\text{Exponent} = \frac{10.8}{10} = 1.08$$

Now, calculate $e^{1.08}$:

$$e^{1.08} \approx 2.94$$

Combine with the frequency factor (0.81):

$$\text{Ratio} \approx 0.81 \times 2.94 \approx \mathbf{2.38}$$

_(This matches the solution's 2.37 almost exactly)._

**Conclusion for 700K:** The ratio is ~2.4 to 1.

The Anti-Stokes line is now huge! It is nearly half the size of the Stokes line.

---

### 4. Summary

You have now completed the full Raman Spectroscopy story! Here is what you should take away for your exam:

1.  **Selection Rules (Part a):** Raman needs a change in **polarizability** (squishiness of the electron cloud).
    
2.  **Intensity Origins (Part b):** Stokes creates a vibration (easy); Anti-Stokes destroys one (hard).
    
3.  **Temperature Dependence (Part c & d):**
    
    -   **Stokes** lines are always strong and don't care much about temperature.
        
    -   **Anti-Stokes** lines are extremely sensitive to temperature.
        
    -   **Cold** = No Anti-Stokes.
        
    -   **Hot** = Strong Anti-Stokes.
        

**Next Step:**

That completes this specific problem sheet! If you have more questions on Solid State Physics (perhaps about Brillouin zones, specific heat, or X-ray diffraction), feel free to upload them. I'm ready when you are!