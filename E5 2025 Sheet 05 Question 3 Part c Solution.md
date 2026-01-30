

![[Pasted image 20260128114910.png]]
![[Pasted image 20260128114917.png]]

This is the finale of our "Storage Rings 101" lesson! Part (c) is the "punchline" that explains the entire history of CERN over the last 30 years.

We are answering the fundamental question: **Why did CERN rip out the LEP machine and replace it with the LHC?**

Let's break down the professor's solution, which uses a brilliant comparison between a "hypothetical" machine and the "real" one.

---

### **1. The Hypothetical Nightmare: Electrons at 7 TeV**

First, the question asks us to imagine a "What If" scenario:

-   **What if** we kept using electrons (like in LEP) but tried to push them to the LHC's energy level ($7 \text{ TeV}$ or $7000 \text{ GeV}$)?
    

**The Calculation:**

We go back to our trusty energy loss formula from the previous part:

$$\Delta E_{synchr} \approx 88.5 \text{ keV} \cdot \frac{E^4}{R}$$

We plug in the new, massive energy:

-   $E = 7000 \text{ GeV}$
    
-   $R = 4297 \text{ m}$
    

$$\Delta E \approx 88.5 \text{ keV} \cdot \frac{(7000)^4}{4297}$$

**The Result:**

$$\Delta E \approx 49.45 \times 10^6 \text{ GeV} = 49,450 \text{ TeV}$$

**Why the professor calls this "Obviously Bogus":**

Look at the numbers.

-   The beam energy is **$7 \text{ TeV}$**.
    
-   The calculated energy loss _per single turn_ is **$49,450 \text{ TeV}$**.
    

This means that in one single lap, the electron would lose **7,000 times more energy than it actually has**.

Physically, this is impossible. It tells us that you simply **cannot** accelerate electrons to $7 \text{ TeV}$ in this tunnel. They would radiate away their energy faster than you could ever pump it in. You would need a power plant the size of a galaxy to make this work!

This is why circular electron accelerators hit a "hard limit" on energy.

---

### **2. The Solution: Switching to Protons**

So, how do we reach $7 \text{ TeV}$ without bankrupting the planet? We switch to **Protons**.

Protons are the heavyweights of the particle world. A proton is roughly **1836 times heavier** than an electron.

**The Physics of Mass and Radiation:**

Synchrotron radiation is caused by the _acceleration_ (change in direction) of the charged particle.

-   Think of it like taking a sharp corner in a car.
    
-   A light car (electron) skids easily and screeches tires (radiates energy).
    
-   A heavy truck (proton) is much harder to push off course, but it handles the turn with much more stability and "screeches" much less.
    

Mathematically, the energy loss scales with the inverse of the mass to the fourth power ($m^{-4}$):

$$\Delta E_{synchr} \propto \frac{1}{m^4}$$

---

### **3. Calculating the Proton Energy Loss**

The professor uses a clever "scaling trick" here instead of starting from scratch. We can just compare the electron and the proton.

$$\frac{\Delta E_p}{\Delta E_e} = \left( \frac{m_e}{m_p} \right)^4$$

-   $m_e = 0.511 \text{ MeV}/c^2$
    
-   $m_p = 938.3 \text{ MeV}/c^2$
    

The ratio is:

$$\left( \frac{0.511}{938.3} \right)^4 \approx 8.797 \times 10^{-14}$$

This number is incredibly tiny! It means a proton radiates **0.00000000000008 times** as much energy as an electron at the same energy.

**Final Calculation:**

We take the "bogus" electron energy loss we calculated in Step 1 and multiply it by this tiny ratio:

$$\Delta E_{synchr, p} = (49.45 \times 10^{18} \text{ eV}) \cdot (8.797 \times 10^{-14})$$

$$\Delta E_{synchr, p} \approx 4.35 \times 10^3 \text{ eV} = 4.35 \text{ keV}$$

---

### **4. Professor's Summary: The Grand Comparison**

Let's look at the final scorecard for the 27km CERN tunnel:

![[Pasted image 20260128123856.png]]

**The Takeaway:**

-   **Electrons** are great for precision because they are point-like particles, but they radiate away all their energy if you try to bend them in a circle.
    
-   **Protons** are "messy" (they are bags of quarks), but they are heavy. Being heavy means they don't radiate much synchrotron radiation. This allows the LHC to reach energies ($7 \text{ TeV}$) that would be impossible for electrons.
    

However, there is no free lunch! Because protons don't radiate energy, they don't "cool down" naturally. This makes the beam dynamics in the LHC very tricky in other ways—but that's a topic for an advanced class!

**Next Step:**

You have now analyzed the magnetic fields (Part a), the power consumption (Part b), and the fundamental physics limits (Part c) of the world's largest machine.

Would you like me to summarize the key formulas we used today into a "Cheat Sheet" for your future studies?