

Hello there! Welcome to your first day of "virtual" particle physics class. I'm delighted to be your professor today.

Particle physics is a bit like being a detective. You never actually _see_ the particles; you only see the footprints they leave behind in our detectors. We have to look at those footprints (tracks, lights, signals) and deduce who walked through the room.

Let’s break down the solution for **Part (a)** step-by-step, using the "other professor's" notes to guide us.

---

### Step 1: The "Footprints" (Visual Analysis)

First, look at the diagram in your problem.

-   **The Tracking Detector (Left):** Notice the vertical lines representing the detector layers. In part (a), do you see any tracks coming from the far left? No. The tracks (the dots) suddenly appear in the middle of the detector volume.
    
-   **The Physics:** Charged particles leave tracks (by ionizing the material they pass through). Neutral particles are invisible to tracking detectors.
    
-   **The Conclusion:** Since there is no track initially, and then suddenly two tracks appear, we are looking at a **neutral particle** that decayed or converted into **two oppositely charged particles**.
    

### Step 2: The "Speed Trap" (Cherenkov Detectors)

Next, the particles hit the "Cherenkov" detectors. Think of these as a series of speed traps.

Cherenkov light is a "sonic boom" for light. It only happens if a particle moves faster than the speed of light in that specific material.

The condition for light is:

$$\beta \geq \frac{1}{n}$$

(Where $\beta$ is the particle's speed as a fraction of the speed of light, and $n$ is the refractive index).

Let's look at the "Speed Trap" thresholds for our detector layers:

1.  **Layer 1 ($n=1.1$):** Speed limit is $\beta \geq 1/1.1 \approx 0.909$.
    
2.  **Layer 2 ($n=1.05$):** Speed limit is $\beta \geq 1/1.05 \approx 0.952$.
    
3.  **Layer 3 ($n=1.01$):** Speed limit is $\beta \geq 1/1.01 \approx 0.990$.
    

What did our particle do?

The problem states the particle leaves a signature where:

-   It triggers Layer 1 ($n=1.1$) $\rightarrow$ It's fast! ($\beta > 0.909$).
    
-   It triggers Layer 2 ($n=1.05$) $\rightarrow$ Still fast! ($\beta > 0.952$).
    
-   It **FAILS** to trigger Layer 3 ($n=1.01$) $\rightarrow$ Too slow! ($\beta < 0.990$).
    

The Clue: The charged particles' speed is trapped between these two values:

$$0.952 \le \beta \le 0.990$$

### Step 3: The "Brake Test" (The Iron Absorber)

Between the 3rd and 4th layer, there is a 1 cm thick block of Iron. This acts like a brake. As particles smash through the iron, they lose energy.

-   **Before the Iron:** We know the particle was fast ($\beta \ge 0.952$).
    
-   **After the Iron:** The problem implies the 4th detector ($n=1.1$) stays dark. This means the particle slowed down so much it dropped below the easiest speed limit ($\beta < 0.909$).
    

This is a massive change in speed! Imagine throwing a bowling ball (heavy proton) and a ping-pong ball (light electron) through a curtain. The bowling ball barely slows down. The ping-pong ball stops almost completely.

Since our particle slowed down drastically (dropping its $\beta$ by at least 0.043), it must be very light.

### Step 4: Identifying the Suspect (Calculations)

The other professor calculated exactly how much energy is lost in that 1 cm of iron. Using the "Bethe-Bloch" formula (a standard formula for energy loss), they estimated the energy loss is roughly:

$$\Delta E \approx 16 \text{ MeV}$$

Now, we use Einstein's relativity. The change in energy is related to the particle's mass ($m$) and the change in its "Lorentz factor" ($\gamma$, which is just another way to measure speed):

$$\Delta E = \Delta \gamma \cdot mc^2$$

Using the speed limits we found in Step 2 and 3, the professor calculated that the change in $\gamma$ was at least 0.868.

So, we can solve for the mass:

$$16 \text{ MeV} \approx 0.868 \cdot mc^2$$

$$mc^2 \le \frac{16 \text{ MeV}}{0.868} \approx 18 \text{ MeV}$$

The Verdict:

We are looking for a charged particle with a mass of less than 18 MeV.

-   Proton mass: ~938 MeV (Way too heavy)
    
-   Pion mass: ~140 MeV (Too heavy)
    
-   Muon mass: ~105 MeV (Too heavy)
    
-   **Electron mass: ~0.511 MeV** (Perfect fit!)
    

The charged particles are electrons ($e^-$) and positrons ($e^+$).

Therefore, the neutral parent particle that created them must be a Photon ($\gamma$) undergoing "pair production".

### Summary of Answer (a)

-   **Identity:** The particle is a **Photon ($\gamma$)** which converts into an electron-positron pair ($e^+e^-$).
    
-   **Energy Limits:**
    
    -   Based on the speed limits derived from the Cherenkov detectors, the energy of _each_ electron is between **1.67 MeV and 3.62 MeV**.
        
    -   Since the photon created two of them, the total energy of the incoming photon is roughly double that: **3.34 MeV to 7.24 MeV**.
        

Ready for part (b)? Just let me know!