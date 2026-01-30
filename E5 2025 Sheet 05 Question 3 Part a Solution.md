

![[Pasted image 20260128114843.png]]

Hello there! Welcome to "Introduction to Particle Accelerators." I am delighted to be your thought partner and professor for this session. It is wonderful to have a curious student who wants to understand the _physics_ behind the equations, not just plug in numbers.

We are looking at a classic problem involving the **LEP (Large Electron-Positron Collider)**, which was the predecessor to the LHC at CERN.

Let's break down the solution provided by your other professor (the second image) and explain part **(a)** step-by-step.

---

### **1. The Setup: What are we actually building?**

Before we do any math, imagine the machine. We have a massive tunnel that is **27 km** in circumference. Inside, we want to send electrons ($e^-$) and positrons ($e^+$) flying in a circle so they can smash into each other.

-   **The Problem:** Charged particles like to travel in straight lines. To make them go in a circle, we need to apply a force to bend their path.
    
-   **The Solution:** Dipole Magnets. A magnetic field perpendicular to the particle's motion creates a "Lorentz Force" that pushes the particle sideways, creating a circular orbit.
    

### **2. Decoding the Solution: Step-by-Step**

Let's look at the solution image you provided and deconstruct it.

#### **Step A: Calculating the Beam Energy ($p_e$)**

The solution starts with this line:

> "At these energies $E \sim p \Rightarrow p_e = 104.5 \text{ GeV}/c$"

**Why did they do this?**

The problem states the **"center of mass energy"** is $209 \text{ GeV}$. In a collider like LEP, you have two beams hitting each other head-on. If the total collision energy is $209 \text{ GeV}$, then each individual beam carries **half** that energy.

$$E_{beam} = \frac{209 \text{ GeV}}{2} = 104.5 \text{ GeV}$$

**Why $E \sim p$?**

At $104.5 \text{ GeV}$, these electrons are moving incredibly close to the speed of light. Their mass energy is tiny compared to their kinetic energy. In high-energy physics, we often approximate Energy ($E$) as being equal to Momentum ($p$) times the speed of light ($c$).

So, we treat the momentum $p$ as **$104.5 \text{ GeV}/c$**.

---

#### **Step B: The "Golden Formula" of Accelerator Physics**

The solution uses this formula:

$$p = 0.3 \cdot B \cdot R$$

This is the most famous "back-of-the-envelope" equation for accelerator physicists. It relates:

-   **$p$**: Momentum (in $\text{GeV}/c$)
    
-   **$B$**: Magnetic Field strength (in Tesla, $\text{T}$)
    
-   **$R$**: Radius of the machine (in meters, $\text{m}$)
    

**Where does the "0.3" come from?**

This is a helpful shortcut derived from the fundamental Lorentz force equation ($F = qvB$).

In standard physics units, the relationship is $p = q \cdot B \cdot R$.

However, if you convert the speed of light ($c \approx 3 \times 10^8 \text{ m/s}$) and the units of charge and energy into the units particle physicists actually use (GeV and Tesla), the speed of light factor essentially becomes the number **0.3**.

It's a "magic number" that makes the units work out perfectly!

---

#### **Step C: Finding the Radius ($R$)**

The solution calculates:

$$R = \frac{27000 \text{ m}}{2\pi} = 4.297 \times 10^3 \text{ m}$$

**The Logic:**

The problem asks us to "Assume the whole circumference is filled with dipole magnets."

We know the circumference ($C$) is $27 \text{ km}$ or $27,000 \text{ meters}$.

Using basic geometry ($C = 2\pi R$), we solve for the radius $R$. This tells us how wide the circle is that the particles are traveling in.

---

#### **Step D: Solving for the Magnetic Field ($B$)**

Now, we just rearrange our "Golden Formula" to solve for $B$:

$$B = \frac{p}{0.3 \cdot R}$$

Substitute the numbers we found:

1.  **$p$** = $104.5$ (from Step A)
    
2.  **$R$** = $4297$ (from Step C)
    

$$B = \frac{104.5}{0.3 \cdot 4297} \text{ T}$$

$$B \approx 0.08106 \text{ T}$$

To make it look nicer, we can convert Tesla (T) to milliTesla (mT):

**$B = 81.06 \text{ mT}$**

---

### **3. Professor's Commentary: Does this number make sense?**

As a physicist, you should always "sanity check" your answer.

We calculated a field of roughly **0.08 Tesla**.

-   A standard fridge magnet is about **0.005 T**.
    
-   The Earth's magnetic field is about **0.00005 T**.
    
-   Modern MRI machines are **1.5 to 3 T**.
    

So, the magnets at LEP were not incredibly powerful compared to modern machines! This is because **electrons are light**. It doesn't take that much magnetic muscle to bend them, even at high speeds. The challenge with electrons isn't bending them; it's keeping them from losing energy (which we might discuss in a later question!).

The LHC (which sits in the same tunnel now) uses protons. Protons are much heavier and harder to bend, which is why the LHC needs magnets that are **8.3 Tesla**—over 100 times stronger than what you just calculated for LEP!

### **Summary of the Answer**

1.  We found the energy per beam: **$104.5 \text{ GeV}$**.
    
2.  We found the radius of the 27km tunnel: **$\sim 4297 \text{ m}$**.
    
3.  We used the formula $p = 0.3 B R$ to find that the required magnetic field is **$0.081 \text{ T}$** (or $81 \text{ mT}$).
    

**Next Step:**

Now that we've solved for the electron machine (LEP), are you ready to tackle the second part of the question where we switch to **protons** (the LHC) and see how that changes the magnetic field requirements? (Spoiler: We're going to need much bigger magnets!)