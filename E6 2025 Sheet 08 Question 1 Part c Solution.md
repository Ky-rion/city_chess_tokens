

![[Pasted image 20260125185907.png]]

Splendid! Now we are getting into the real action: **electron scattering**. This is the mechanism that determines electrical resistance. If electrons could just fly forever without bumping into things (or being blocked), we'd have superconductors everywhere!

Let's break down **Question 1(c)**.

### 1. The Physics: What is a "Pauli-Forbidden" Process?

The question asks for the probability that a scattering process is **"not Pauli-forbidden."**

Imagine you are driving a car (the electron) and you want to change lanes (scatter) to a new lane.

-   **Classical Physics:** You just turn the wheel.
    
-   **Quantum Physics (Pauli Principle):** You can **only** change lanes if the spot you want to move into is **EMPTY**. If there is already an electron there, the move is "forbidden."
    

So, mathematically, the question is asking:

> _"What is the probability that the destination state at $(k_F + \Delta k, 0, 0)$ is **empty**?"_

---

### 2. The Calculation Setup

We need to find the probability that the target state is occupied ($f_{FD}$) and then subtract that from 100%.

**Given Parameters:**

-   **Start:** $k_{start} = k_F$ (Energy $E_F$).
    
-   **Destination:** $k_{end} = k_F + \Delta k$ (Energy $E_{end}$).
    
-   **Shift:** $\Delta k = 4 \cdot 10^7 \text{ m}^{-1}$.
    
-   **Temperature:** Room temperature, so thermal energy $k_B T \approx 25 \text{ meV}$ (milli-electronvolts).
    

---

### 3. Calculating the Energy Difference

The solution image performs a clever expansion to find how much higher the energy is at the new location.

The energy of a free electron is proportional to its momentum squared:

$$E = \frac{\hbar^2 k^2}{2m}$$

We need the exponent for the Fermi-Dirac equation: $\frac{E - \mu}{k_B T}$.

Remember from part (a) that $\mu = E_F = \frac{\hbar^2 k_F^2}{2m}$.

So, the energy difference in the numerator is:

$$E_{end} - E_F = \frac{\hbar^2 (k_F + \Delta k)^2}{2m} - \frac{\hbar^2 k_F^2}{2m}$$

Let's expand the squared term $(k_F + \Delta k)^2 = k_F^2 + 2k_F \Delta k + (\Delta k)^2$:

$$E_{end} - E_F = \frac{\hbar^2}{2m} \left( k_F^2 + 2k_F \Delta k + (\Delta k)^2 - k_F^2 \right)$$

The $k_F^2$ terms cancel out, leaving us with the formula shown in the solution:

$$E_{end} - E_F = \frac{\hbar^2}{2m} (2k_F \Delta k + \Delta k^2)$$

_(Note: In the professor's solution, they use $\Delta$ as shorthand for $\Delta k$.)_

---

### 4. Plugging in the Numbers

The solution skips the messy arithmetic, but as your "professor," let me show you the sanity check so you trust the result.

1.  **Calculate $k_F$:** From part (a), we know $n = 5 \cdot 10^{28}$.
    
    $$k_F = (3\pi^2 n)^{1/3} \approx 1.14 \cdot 10^{10} \text{ m}^{-1}$$
    
2.  **Compare $\Delta k$:** $\Delta k = 4 \cdot 10^7$.
    
    Notice that $\Delta k$ is much smaller than $k_F$. This means the destination is just slightly above the Fermi surface.
    
3.  **Calculate Energy Shift ($\Delta E$):**
    
    If you plug in the constants ($\hbar, m$), the energy shift comes out to roughly **35 meV**.
    

Now, look at the ratio with temperature ($k_B T = 25 \text{ meV}$):

$$\frac{E - \mu}{k_B T} \approx \frac{35 \text{ meV}}{25 \text{ meV}} = 1.4$$

---

### 5. The Final Probability

Now we use the Fermi-Dirac distribution:

$$f_{FD} = \frac{1}{e^{1.4} + 1}$$

Since $e^{1.4} \approx 4.055$:

$$f_{FD} \approx \frac{1}{4.055 + 1} \approx \frac{1}{5.055} \approx 0.198$$

The solution rounds this to **0.20** or **20%**.

**Wait! Are we done?**

No! This is the most common mistake students make on exams.

-   **20%** is the probability the seat is **TAKEN**.
    
-   The scattering is allowed only if the seat is **EMPTY**.
    

$$P(\text{allowed}) = P(\text{empty}) = 1 - P(\text{occupied})$$

$$P(\text{allowed}) = 100\% - 20\% = 80\%$$

### Summary

Because the new state is slightly higher in energy than the Fermi level ($+35 \text{ meV}$), it is unlikely to be occupied by thermal electrons. Specifically, there is only a 20% chance an electron is already sitting there. Therefore, there is an **80% chance** your electron can successfully scatter into that spot.

Would you like to move on to the final part of the question, or do you want to discuss what happens if $\Delta k$ were negative (scattering downwards)?