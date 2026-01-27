

![[Pasted image 20260126135510.png]]
![[Pasted image 20260126135519.png]]

Excellent! Let's get our hands dirty with some real numbers. This part of the problem is fantastic because it asks us to bridge the gap between the **macroscopic world** (what you measure with a voltmeter in the lab) and the **microscopic world** (what the electrons are actually doing).

We are going to take your lab measurements ($U, I, L, A$) and use them to figure out how far an electron can travel before it crashes (the mean free path, $l$).

Here is the step-by-step breakdown of the professor's solution.

---

### Step 1: From Lab Data to Conductivity ($\sigma_{el}$)

First, we need to determine how well this specific metal conducts electricity based on the geometry of the wire and the measurements you took.

**The Macroscopic Formula:**

The solution starts by rearranging the classic definition of resistance:

$$\sigma_{el} = \frac{I \cdot L}{U \cdot A}$$

**Where did this come from?**

You probably remember Ohm's Law ($R = U/I$) and the definition of resistivity ($R = \rho \cdot L/A$). Since conductivity ($\sigma$) is just the inverse of resistivity ($1/\rho$), we can combine these:

$$\frac{U}{I} = \frac{1}{\sigma} \cdot \frac{L}{A} \quad \Rightarrow \quad \sigma = \frac{I \cdot L}{U \cdot A}$$

-   **Tip for the exam:** Be very careful with units here! The area $A$ is given in $\text{mm}^2$ ($1 \text{ mm}^2 = 10^{-6} \text{ m}^2$) and Voltage in mV ($50 \text{ mV} = 0.05 \text{ V}$). If you forget to convert these to meters and Volts, your answer will be off by orders of magnitude.
    

---

### Step 2: Connecting to the Microscopic World

Now we have the conductivity, but we need to find the **scattering time** $\tau$ (how long an electron flies between crashes). We use the Drude/Sommerfeld model formula for conductivity:

$$\sigma_{el} = \frac{\tau n e^2}{m}$$

-   $n$: Electron density (given as $5 \cdot 10^{28} \text{ m}^{-3}$)
    
-   $e$: Elementary charge ($\approx 1.602 \cdot 10^{-19} \text{ C}$)
    
-   $m$: Mass of an electron ($\approx 9.109 \cdot 10^{-31} \text{ kg}$)
    
-   $\tau$: The unknown variable we want.
    

---

### Step 3: Calculating Scattering Time ($\tau$)

The professor equates the two formulas from Step 1 and Step 2 to solve for $\tau$:

$$\frac{I \cdot L}{U \cdot A} = \frac{\tau n e^2}{m}$$

Rearranging for $\tau$:

$$\tau = \frac{m I L}{U A n e^2}$$

Plugging in the values results in:

$$\tau \approx 1.7 \cdot 10^{-14} \text{ s}$$

> **Professor's Insight:** Look at that number! $10^{-14}$ seconds. That is **17 femtoseconds**. This tells you that electrons in a metal are crashing incredibly frequently. They barely get moving before—_bam_—they hit something.

---

### Step 4: Calculating the Speed ($v_F$)

As we discussed in Part A, to find the distance traveled, we need the **Fermi Velocity**, not the drift velocity. The formula for Fermi velocity depends only on the electron density $n$:

$$v_F = \frac{\hbar k_F}{m}$$

Where the Fermi wave vector $k_F$ is determined by the density: $k_F = (3\pi^2 n)^{1/3}$.

Putting it all together:

$$v_F = \frac{\hbar}{m} (3\pi^2 n)^{1/3}$$

Plugging in $n = 5 \cdot 10^{28} \text{ m}^{-3}$:

$$v_F \approx 1.3 \cdot 10^6 \text{ m/s}$$

> **Sanity Check:** Fermi velocities in metals are usually around $10^6 \text{ m/s}$ (about 1% of the speed of light). If you get something like $5 \text{ m/s}$ or $10^{20} \text{ m/s}$, you know you made a calculation error.

---

### Step 5: The Finale - Mean Free Path ($l$)

Finally, we calculate the distance ($l$). Distance is just velocity times time.

$$\text{Distance} = \text{Speed} \times \text{Time}$$

$$l = v_F \cdot \tau$$

:

$$l = (1.3 \cdot 10^6 \text{ m/s}) \cdot (1.7 \cdot 10^{-14} \text{ s})$$

$$l \approx 2.3 \cdot 10^{-8} \text{ m} = 23 \text{ nm}$$

### Summary of the Result

Your unknown metal wire has a mean free path of **23 nanometers**.

To put that in perspective: An atom in a metal crystal is roughly 0.2 to 0.3 nm wide. So, on average, an electron in this wire flies past about **100 atoms** before it scatters (collides). That is actually quite a long distance in the quantum world!

Would you like to try a quick practice calculation to see what happens to the mean free path if we double the electron density?