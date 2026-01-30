

![[Pasted image 20260128114853.png]]

Excellent! I'm glad you're sticking with me. Part (b) is where things get really interesting—and expensive! We are about to discover why the LEP accelerator was such a power-hungry machine and why it was eventually replaced.

In Part (a), we bent the beam into a circle. Now, we have to pay the "tax" for doing so.

### **1. The Physics Concept: Synchrotron Radiation**

You might be wondering: "Why do we need to add energy? Once the particles are moving at $104.5 \text{ GeV}$, won't they just stay at that speed?"

In a perfect world, yes. But in electromagnetism, there is a strict rule: **Any charged particle that accelerates radiates energy.**

-   **Wait, is it accelerating?** Yes! Even if the _speed_ is constant, moving in a circle is a form of acceleration (centripetal acceleration) because the _direction_ is changing.
    
-   **The Result:** As the electrons turn the corner in the dipole magnets, they scream out energy in the form of X-rays and gamma rays. This is called **Synchrotron Radiation**.
    

This radiation acts like a "friction" or drag. If we don't put energy _back in_, the electrons would spiral inward and crash into the walls within milliseconds.

---

### **2. Step-by-Step Explanation of the Solution**

Let's break down the professor's calculations from the second image.

#### **Step A: Calculating Energy Loss per Turn**

The solution states:

> "The energy loss through synchrotron radiation... has to be fed in again through cavities."

We need to balance the books: Energy In = Energy Out.

The formula for energy loss per turn ($\Delta E_{synchr}$) for a relativistic electron is given by a famous practical approximation used in accelerator physics:

$$\Delta E_{synchr} [\text{keV}] \approx 88.5 \cdot \frac{E^4 [\text{GeV}]}{R [\text{m}]}$$

**This is the most critical equation in circular electron accelerators.**

Notice the **$E^4$**. This is huge!

-   If you double the energy ($E$), the energy loss goes up by a factor of $2^4 = 16$.
    
-   This is why high-energy electron rings (like LEP) have to be enormous. We try to make $R$ large to keep the energy loss manageable.
    

**Let's plug in our numbers:**

-   $E = 104.5 \text{ GeV}$ (from Part A)
    
-   $R = 4297 \text{ m}$ (from Part A)
    

$$\Delta E_{synchr} = 88.5 \text{ keV} \cdot \frac{(104.5)^4}{4297}$$

$$\Delta E_{synchr} \approx 2.456 \times 10^6 \text{ keV} = 2.456 \text{ GeV}$$

**Interpretation:** Every single time an electron does **one lap** around the tunnel, it loses **2.456 GeV** of energy. Considering the beam energy is $104.5 \text{ GeV}$, it loses about **2.3%** of its total energy _every lap_! The accelerator cavities must kick the particles back up by 2.456 GeV every revolution just to keep them steady.

---

#### **Step B: Calculating the Power (The Electricity Bill)**

Now we need to find the **Power ($P$)**. Power is simply Energy per unit of Time.

The solution uses the Beam Current ($I$) to find this.

-   **Beam Current ($I$):** The flow of electric charge per second.
    
-   **Current given:** $5 \text{ mA}$ (or $0.005$ Amperes).
    

The solution uses a rigorous chain of unit conversions:

$$P = \dot{N}_e \cdot \Delta E_{synchr}$$

Where $\dot{N}_e$ is the number of electrons passing a point per second. Since Current ($I$) is Charge ($Q$) over Time ($t$), and the charge of one electron is $e$:

$$\dot{N}_e = \frac{I}{e}$$

So the formula becomes:

$$P = \frac{I}{e} \cdot \Delta E_{synchr}$$

**The Calculation:**

$$P = \frac{5 \times 10^{-3} \text{ C/s}}{1.602 \times 10^{-19} \text{ C}} \cdot (2.456 \times 10^9 \text{ eV})$$

_Wait! There is a simpler way to think about this._

In electrical terms, if an electron gains 1 eV of energy, it has passed through a potential difference of 1 Volt.

If our electrons need to gain $2.456 \text{ GeV}$ (Giga-electron-volts), that is effectively equivalent to passing through a voltage of **$2.456 \text{ GV}$ (Gigavolts)**.

Power is just Current times Voltage ($P = I \cdot V$):

$$P = (5 \times 10^{-3} \text{ A}) \cdot (2.456 \times 10^9 \text{ V})$$

$$P = 12.28 \times 10^6 \text{ Watts} = 12.28 \text{ MW}$$

This matches the solution's answer perfectly.

---

#### **Step C: Total Power for the Whole Machine**

The collider has **two beams**:

1.  Electrons circling one way.
    
2.  Positrons circling the other way.
    

Both beams lose energy equally. So, we multiply by 2:

$$P_{tot} = 2 \cdot 12.28 \text{ MW} = 24.56 \text{ MW}$$

---

### **3. Professor's Commentary: The Consequence of $E^4$**

To put this in perspective: **24.56 Megawatts** is roughly the power consumption of **20,000 average homes**.

And that is _only_ the power dumped into the beam to keep it alive. It doesn't count the power for the magnets, the cooling, the computers, or the coffee machines!

This result ($24.56 \text{ MW}$) explains why LEP was shut down.

Remember that $E^4$ scaling?

-   If they wanted to double the energy of LEP to find heavier particles, the power requirement would have gone up by **16 times**.
    
-   $24 \text{ MW} \times 16 \approx 384 \text{ MW}$. That's getting close to the output of a small nuclear power plant just for the RF system!
    

It became physically and economically impossible to push electrons to higher energies in that tunnel. This is why we switched to **Protons** (the LHC) for the next machine. Protons are 2000 times heavier than electrons, so they emit almost **zero** synchrotron radiation at these energies.

**Next Step:**

Now that we've seen why electrons are "expensive" at high energy, would you like to solve the next part where we see how **Protons** behave in the exact same tunnel? (This will show us the stark difference between LEP and the LHC!)