

This is a fantastic final problem! It moves us from theoretical nuclear physics into the gritty reality of experimental physics. We are no longer just asking "what does the sun create?", but rather "what can we actually _catch_ here on Earth?"

In the Borexino experiment, we are trying to detect "ghostly" particles (neutrinos) using a giant tank of liquid. To find the answer, we need to calculate three things:

1.  **The Net:** How big is the mesh we are using to catch them? (The Cross Section, $\sigma$)
    
2.  **The Fish:** How many neutrinos are passing through? (The Flux, $\Phi$)
    
3.  **The Water:** How many targets are waiting in the tank to be hit? (The Number of Electrons, $N_e$)
    

The formula for the Rate of Events ($R$) is:

$$R = \Phi \times \sigma \times N_e$$

Let's calculate each piece step-by-step.

---

### Step 1: Count the Targets (The Electrons)

This is the trickiest part. The neutrinos scatter off **electrons**. We need to count exactly how many electrons are inside 100 tons of the liquid scintillator, Pseudocumene ($C_9H_{12}$).

**A. Find the molar mass of Pseudocumene ($C_9H_{12}$):**

-   Carbon ($C$): $12 \text{ g/mol}$
    
-   Hydrogen ($H$): $1 \text{ g/mol}$
    
-   Molar Mass ($M_{mol}$) = $(9 \times 12) + (12 \times 1) = 108 + 12 = \mathbf{120 \text{ g/mol}}$
    

**B. Find the number of electrons in one molecule:**

-   One Carbon atom has 6 electrons.
    
-   One Hydrogen atom has 1 electron.
    
-   Electrons per molecule = $(9 \times 6) + (12 \times 1) = 54 + 12 = \mathbf{66 \text{ electrons}}$
    

C. Calculate the total number of electrons in the detector:

We have 100 tons of liquid.

-   Mass ($M_{det}$) = $100 \text{ tons} = 100,000 \text{ kg} = 10^8 \text{ g}$.
    
-   Moles of substance = $\frac{\text{Mass}}{\text{Molar Mass}} = \frac{10^8 \text{ g}}{120 \text{ g/mol}}$.
    

Now, we multiply the number of moles by Avogadro's number ($N_A \approx 6.022 \times 10^{23}$) to get molecules, and then by 66 to get electrons.

$$N_e = \left( \frac{10^8}{120} \right) \times (6.022 \times 10^{23}) \times 66$$

$$N_e \approx 3.31 \times 10^{31} \text{ electrons}$$

That is a staggering number of targets!

---

### Step 2: Prepare the Variables (Unit Conversions)

Physics requires consistent units. We need everything in meters and seconds.

-   **Flux ($\Phi$):** Given as $3.3 \times 10^{13} \text{ m}^{-2}\text{s}^{-1}$. (Already good!)
    
-   **Cross Section ($\sigma$):** Given as $7.93 \times 10^{-21} \text{ barns}$.
    
    -   We must convert barns to square meters.
        
    -   $1 \text{ barn} = 10^{-28} \text{ m}^2$.
        
    -   $\sigma = 7.93 \times 10^{-21} \times 10^{-28} = \mathbf{7.93 \times 10^{-49} \text{ m}^2}$.
        
    -   _Note: This number is incredibly small, which is why neutrinos can pass through Earth without stopping!_
        
-   **Time:** We want the rate "per day".
    
    -   Seconds in a day = $24 \times 60 \times 60 = \mathbf{86,400 \text{ s}}$.
        

---

### Step 3: Calculate the Rate

Now we multiply our three key numbers together to find the events per second.

$$R_{sec} = \Phi \times \sigma \times N_e$$

$$R_{sec} = (3.3 \times 10^{13}) \times (7.93 \times 10^{-49}) \times (3.31 \times 10^{31})$$

Grouping the powers of 10: $10^{13} \times 10^{-49} \times 10^{31} = 10^{-5}$

Multiplying the coefficients: $3.3 \times 7.93 \times 3.31 \approx 86.6$

$$R_{sec} \approx 86.6 \times 10^{-5} \text{ events per second}$$

Finally, convert this to **Events per Day**:

$$\text{Events/Day} = R_{sec} \times 86,400$$

$$\text{Events/Day} = (8.66 \times 10^{-4}) \times 86,400$$

$$\text{Events/Day} \approx \mathbf{74.8}$$

---

### Final Answer

The Borexino detector should see approximately **75 scattering events per day**.

### 🎓 Professor's Conclusion

Think about this result. We built a machine weighing **100 tons**, waited an entire day, and only caught **75** particles.

This is the challenge of neutrino physics. Billions of neutrinos pass through your fingernail every second, but they interact so weakly (that $10^{-49} \text{ m}^2$ number!) that we need cathedral-sized detectors just to see a handful of them.

**Would you like to know how they distinguish these 75 real events from the thousands of "fake" signals caused by natural radioactivity in the rocks and air?**