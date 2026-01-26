

![[Pasted image 20260125184604.png]]

Welcome back to the lab! This is where the rubber meets the road. In part (b), we did the heavy lifting of deriving the formula. Now, in part (c), we get to act like real experimental physicists and use that formula to extract real data from a measurement.

This is a very practical problem: **"Can we determine the temperature of a crystal just by shining a laser on it?"** (Spoiler: Yes, and it's 300 Kelvin, but let's see how we get there).

### 1. Translation: What are we asked?

**The Question (Image 1):**

> _c) Im folgenden sehen Sie ein Ramanspektrum, das unter Anregung mit einem Laser der Wellenlänge $\lambda = 514$ nm aufgenommen wurde. Bestimmen Sie die Temperatur $T$, bei der das Spektrum aufgenommen wurde._
> 
> **Translation:**
> 
> "In the following, you see a Raman spectrum recorded under excitation with a laser of wavelength $\lambda = 514$ nm. Determine the temperature $T$ at which the spectrum was recorded."

---

### 2. Reading the Spectrum (The "Sherlock Holmes" Part)

Before we do any math, we have to look at the graph in the question image and extract the variables we need.

1.  **Identify Stokes vs. Anti-Stokes:**
    
    -   We see a central peak at 0 (the laser line/Rayleigh scattering).
        
    -   We see a **tall peak** on the left (at roughly -525 cm$^{-1}$).
        
    -   We see a **tiny peak** on the right (at roughly +525 cm$^{-1}$).
        
    -   _Physics Rule:_ As we learned in part (b), the Stokes probability (creating a vibration) is much higher than Anti-Stokes (destroying an existing vibration). Therefore, the **Tall Peak is Stokes ($I_S$)** and the **Small Peak is Anti-Stokes ($I_{AS}$)**.
        
2.  **Read the Intensities ($I_S / I_{AS}$):**
    
    -   Look at the height of the tall peak. It looks like it is about 10 units high (arbitrary units).
        
    -   Look at the height of the small peak. It looks like it is about 1 unit high.
        
    -   **Ratio:** We estimate $\frac{I_S}{I_{AS}} \approx 10$.
        
3.  **Read the Raman Shift ($\nu_M$):**
    
    -   The peaks are located at roughly 525 cm$^{-1}$ on the x-axis. This is our wavenumber $\tilde{\nu}$.
        

---

### 3. The Calculation (Step-by-Step)

Now we follow the red text in the solution images to calculate the temperature $T$.

#### Step A: Rearrange the Formula

We start with the formula we derived in part (b):

$$\frac{I_S}{I_{AS}} = \frac{(\nu_0 - \nu_M)^4}{(\nu_0 + \nu_M)^4} \cdot e^{\frac{h\nu_M}{k_B T}}$$

We need to solve for $T$.

1.  Isolate the exponential term:
    
    $$e^{\frac{h\nu_M}{k_B T}} = \frac{I_S}{I_{AS}} \cdot \frac{(\nu_0 + \nu_M)^4}{(\nu_0 - \nu_M)^4}$$
    
2.  Take the natural logarithm ($\ln$) of both sides to remove the exponent:
    
    $$\frac{h\nu_M}{k_B T} = \ln \left( \frac{I_S}{I_{AS}} \cdot \frac{(\nu_0 + \nu_M)^4}{(\nu_0 - \nu_M)^4} \right)$$
    
3.  Solve for $T$:
    
    $$T = \frac{h\nu_M}{k_B} \cdot \frac{1}{\ln \left( \frac{I_S}{I_{AS}} \frac{(\nu_0 + \nu_M)^4}{(\nu_0 - \nu_M)^4} \right)}$$
    
    _(This matches Equation 16 in the solution)._
    

#### Step B: Unit Conversions (The Danger Zone!)

Physics requires standard SI units (Hertz, Seconds, Joules), but spectroscopists love using nanometers ($nm$) and inverse centimeters ($cm^{-1}$). We must convert everything.

**1. Calculate Laser Frequency ($\nu_0$):**

Given: $\lambda = 514$ nm $= 514 \times 10^{-9}$ m.

$$\nu_0 = \frac{c}{\lambda} = \frac{2.998 \times 10^8 \text{ m/s}}{514 \times 10^{-9} \text{ m}} = 5.8235 \times 10^{14} \text{ Hz}$$

**2. Calculate Vibration Frequency ($\nu_M$):**

Given: Wavenumber $\tilde{\nu} = 525 \text{ cm}^{-1}$.

_Be careful:_ $1 \text{ cm}^{-1} = 100 \text{ m}^{-1}$.

$$\nu_M = c \cdot \tilde{\nu} = (2.998 \times 10^8 \text{ m/s}) \cdot (525 \cdot 100 \text{ m}^{-1})$$

$$\nu_M = 1.5739 \times 10^{13} \text{ Hz}$$

#### Step C: The Final Plug-in

Now we put it all into our rearranged equation for T.

-   $h$ (Planck constant) $\approx 6.626 \times 10^{-34}$ Js
    
-   $k_B$ (Boltzmann constant) $\approx 1.38 \times 10^{-23}$ J/K
    
-   Ratio $\frac{I_S}{I_{AS}} \approx 10$
    
-   Frequency factor: The term $\frac{(\nu_0 + \nu_M)^4}{(\nu_0 - \nu_M)^4}$ is usually very close to 1 because $\nu_0$ (laser) is much larger than $\nu_M$ (vibration). In this case, it's roughly $1.1$.
    

$$T \approx \frac{(6.626 \times 10^{-34})(1.57 \times 10^{13})}{1.38 \times 10^{-23}} \cdot \frac{1}{\ln(10 \cdot \approx 1.1)}$$

If you type all that into your calculator, you get:

$$\mathbf{T = 300 \text{ K}}$$

---

### 4. Professor's Closing Comment

The result is **300 Kelvin**.

Does this make sense?

$300 \text{ K} \approx 27^\circ \text{C}$. This is essentially **room temperature**.

So, the experiment was likely performed in a standard lab at room temperature. If the Anti-Stokes peak were taller, it would mean the sample was extremely hot! If the Anti-Stokes peak disappeared entirely, the sample would be very cold (near absolute zero).

**Summary for your exam:**

1.  **Read the graph:** Big peak = Stokes, Small peak = Anti-Stokes.
    
2.  **Estimate ratio:** Height of Big / Height of Small.
    
3.  **Convert units:** nm and cm$^{-1}$ must become Hz.
    
4.  **Solve:** Use the log formula to find T.
    

**Next Step:**

That wraps up the "Vibrational Spectroscopy" problem set! Do you have another problem sheet (maybe on crystal structures or band theory), or would you like to recap anything we just covered?