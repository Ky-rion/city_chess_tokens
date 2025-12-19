

This is a great question! It moves us from the abstract math to the brilliant real-world application. Here is the principle of carbon-14 dating, broken down logically.

---

### 1. Carbon is Life

All living things—plants, animals, people—are built from carbon. We get this carbon from our environment.

-   **Plants** get it from carbon dioxide ($CO_2$) in the atmosphere through photosynthesis.
    
-   **Animals** get it by eating plants (or by eating other animals that ate plants).
    

### 2. The Two Types of Carbon

In the atmosphere, carbon exists in a few different forms (isotopes). For our purposes, the two most important are:

-   **Carbon-12 ($^{12}$C):** This is the normal, common, **stable** form of carbon. "Stable" means it _does not_ decay. It sticks around forever.
    
-   **Carbon-14 ($^{14}$C):** This is a much rarer, **radioactive** isotope. It is created in the upper atmosphere when cosmic rays strike nitrogen atoms. This $^{14}$C _does_ decay, as we've been discussing, with a half-life of 5,730 years.
    

### 3. The "Living" State: A Fixed Ratio

As long as an organism is **alive**, it is constantly exchanging carbon with the environment (e.g., the tree is taking in $CO_2$). This means the ratio of $^{14}$C to $^{12}$C inside the living organism is exactly the **same** as the ratio in the atmosphere.

Think of it like a leaky bucket:

-   The water in the bucket is the $^{14}$C.
    
-   The "leak" is the radioactive decay, slowly removing $^{14}$C.
    
-   The "faucet" is the organism's metabolism (breathing, eating, photosynthesizing), constantly pouring _new_ $^{14}$C in from the environment.
    

As long as the organism is alive, the faucet is on, and the water level (the $^{14}$C ratio) stays constant. The problem gives us this fixed, living ratio: $\frac{\text{Number of }^{12}\text{C atoms}}{\text{Number of }^{14}\text{C atoms}} = 7.85 \times 10^{11}$.

### 4. The "Death" State: The Clock Starts

The moment the organism **dies** (e.g., the tree is cut down to make the wood splinter), it **stops** exchanging carbon with the environment.

-   The "faucet" of new $^{14}$C is turned **off**.
    
-   The "leak" of radioactive decay **continues**.
    

From this point forward, the stable $^{12}$C just sits there, but the radioactive $^{14}$C begins to disappear, decaying into nitrogen-14.

### 5. Measuring the Age: The "Ticking" Clock

This is the brilliant part. We can use the radioactive decay law we derived as a clock.

1.  **Find the Original Amount ($A_0$ or $N_0$):** We use the _total carbon_ in the sample (which is almost all $^{12}$C) and the known atmospheric ratio to calculate how much $^{14}$C _must have been_ in the sample when it died. This gives us our starting point, $N_0$, and thus our starting activity, $A_0 = \lambda N_0$.
    
2.  **Measure the Current Amount ($A(t)$ or $N(t)$):** We use a detector (like the "counting tube" in the problem) to measure the _current_ number of decays per hour. This is our current activity, $A(t) = 845$ decays/hour. This $A(t)$ is directly proportional to the amount of $^{14}$C _still remaining_, $N(t)$.
    
3.  **Calculate the Time ($t$):** We now know:
    
    -   The starting activity, $A_0$ (which we'll calculate).
        
    -   The current activity, $A(t)$ (which we measured).
        
    -   The decay constant, $\lambda$ (which we know from the half-life).
        
    
    We just plug these into our decay law $A(t) = A_0 e^{-\lambda t}$ and solve for the only remaining unknown: **$t$**, the time that has passed since the organism died.
    

In short: **We compare how much $^{14}$C is left in an ancient sample to how much it started with. The difference, governed by the 5,730-year half-life, tells us exactly how old the sample is.**

---

It's a truly elegant method! Are you ready to move on to the final part and actually calculate the age of our wood splinter?