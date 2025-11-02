

This is an excellent question! It's where the abstract theory meets the actual experimental data. Let's get right to it.

The question asks us to calculate the "exact rate" (which means the probability) that an alpha particle will scatter by more than $90^\circ$ and compare it to the "roughly 1 in 20,000" that Geiger and Marsden observed.

### 🎯 The Big Picture: Our Strategy

1.  **Find the "Target Size":** The formula for $\sigma$ (the "cross-section") gives us the "effective target area" of a _single_ gold nucleus. If an alpha particle's path is aimed within this tiny area, it will scatter by more than $90^\circ$.
    
2.  **Count the Targets:** We need to figure out how many gold nuclei are "in the way" of the alpha particle as it passes through the $0.4 \text{ } \mu\text{m}$ thick foil. We'll find this by calculating the number of gold atoms per unit area ($N_{\text{targets}}$).
    
3.  **Calculate the Probability:** The total probability ($P$) of a scatter is simply the "target area" ($\sigma$) multiplied by the number of targets ($N_{\text{targets}}$). This gives us a single number, $P$.
    
4.  **Compare:** We'll see how our calculated $P$ compares to the experimental $1/20000$.
    

Let's begin the calculation.

---

### 1. Calculate the Impact Parameter ($b$)

The formula for the cross-section $\sigma$ depends on $b$. The formula for $b$ is given, and it sets the condition for our specific angle $\vartheta$. We are interested in all angles _larger than_ $90^\circ$, so we set our boundary angle $\vartheta = 90^\circ$.

$$b = \frac{1}{4\pi\epsilon_0} \frac{zZe^2}{2E_{\text{kin}}} \frac{1}{\tan(\vartheta/2)}$$

Now, we can use a clever shortcut from our previous problem! In part (b), we found the distance of closest approach ($d_{\text{min}}$) for a $180^\circ$ head-on collision:

$$d_{\text{min}} = \frac{1}{4\pi\epsilon_0} \frac{zZe^2}{E_{\text{kin}}}$$

If you look closely, this term is right inside our formula for $b$! We can substitute it in:

$$b = \frac{d_{\text{min}}}{2} \frac{1}{\tan(\vartheta/2)}$$

Let's plug in our known values:

-   $d_{\text{min}} = 45.5 \text{ fm}$ (from our calculation in part b)
    
-   $\vartheta = 90^\circ$, which means $\vartheta/2 = 45^\circ$
    
-   $\tan(45^\circ) = 1$
    

$$b = \frac{45.5 \text{ fm}}{2} \cdot \frac{1}{1}$$

$b = 22.75 \text{ fm}$

This impact parameter $b$ defines the radius of our "effective target."

### 2. Calculate the Cross-Section ($\sigma$)

Now we find the area of that circular target. This is the cross-section $\sigma$.

$$\sigma = \pi b^2$$

$$\sigma = \pi \cdot (22.75 \text{ fm})^2$$

$$\sigma = \pi \cdot 517.56 \text{ fm}^2$$

$\sigma \approx 1626 \text{ fm}^2$

For our next steps, we need this in standard units ($\text{m}^2$).

-   $1 \text{ fm} = 10^{-15} \text{ m}$
    
-   $1 \text{ fm}^2 = (10^{-15} \text{ m})^2 = 10^{-30} \text{ m}^2$
    

**$\sigma \approx 1.626 \times 10^{-27} \text{ m}^2$**

### 3. Calculate the Number Density of Gold ($n$)

Next, we need to find out how many gold atoms are packed into a cubic meter. We'll use the data from the problem text.

-   Density ($\rho_{\text{Au}}$): $19.29 \text{ kg/dm}^3$
    
-   Molar Mass ($M_{\text{Au}}$): $197 \text{ g/mol}$ (from $^{197}\text{Au}$)
    
-   Avogadro's Number ($N_A$): $6.022 \times 10^{23} \text{ atoms/mol}$
    

First, let's fix the density unit:

-   $1 \text{ dm}^3 = (0.1 \text{ m})^3 = 0.001 \text{ m}^3$
    
-   $\rho_{\text{Au}} = 19.29 \text{ kg} / 0.001 \text{ m}^3 = 19290 \text{ kg/m}^3$
    

And the molar mass unit:

-   $M_{\text{Au}} = 197 \text{ g/mol} = 0.197 \text{ kg/mol}$
    

Now, let's find the number of atoms per cubic meter ($n$):

$$n = \frac{\text{Density}}{\text{Molar Mass}} \times \text{Avogadro's Number}$$

$$n = \left( \frac{19290 \text{ kg/m}^3}{0.197 \text{ kg/mol}} \right) \cdot (6.022 \times 10^{23} \text{ atoms/mol})$$

$$n = (97919 \text{ mol/m}^3) \cdot (6.022 \times 10^{23} \text{ atoms/mol})$$

$n \approx 5.896 \times 10^{28} \text{ atoms/m}^3$

### 4. Calculate the Target Areal Density ($N_{\text{targets}}$)

We don't need the full volume, just the number of atoms in the thin $0.4 \text{ } \mu\text{m}$ foil. We multiply the number density ($n$) by the foil thickness ($d$).

-   $n = 5.896 \times 10^{28} \text{ atoms/m}^3$
    
-   $d = 0.4 \text{ } \mu\text{m} = 0.4 \times 10^{-6} \text{ m}$
    

$$N_{\text{targets}} = n \cdot d$$

$$N_{\text{targets}} = (5.896 \times 10^{28} \text{ atoms/m}^3) \cdot (0.4 \times 10^{-6} \text{ m})$$

$N_{\text{targets}} \approx 2.358 \times 10^{22} \text{ atoms/m}^2$

This is the number of gold nuclei per square meter of foil area.

### 5. Calculate the Final Probability (Rate)

We're at the final step! The probability ($P$) is the effective area of one atom ($\sigma$) times the number of atoms per unit area ($N_{\text{targets}}$).

$$P = \sigma \cdot N_{\text{targets}}$$

$$P = (1.626 \times 10^{-27} \text{ m}^2) \cdot (2.358 \times 10^{22} \text{ atoms/m}^2)$$

$P \approx 3.83 \times 10^{-5}$

This is the "exact rate" or probability the question asks for.

---

## 📈 The Conclusion: Comparing Theory and Experiment

Let's see how our calculated result compares to the observation.

-   **Geiger-Marsden Observation:** "roughly one in 20000"
    
    -   $P_{\text{observed}} = 1 / 20000 = 0.00005 = \mathbf{5.0 \times 10^{-5}}$
        
-   **Our Theoretical Calculation:**
    
    -   $P_{\text{calculated}} = \mathbf{3.83 \times 10^{-5}}$
        

These two numbers are incredibly close!

To make the comparison even clearer, let's see what "1 in X" value our calculation gives:

$$\text{Rate} = 1 / P_{\text{calculated}} = 1 / (3.83 \times 10^{-5})$$

$$\text{Rate} \approx \mathbf{26100}$$

So, the Rutherford scattering formula predicts that **1 in 26,100** particles should scatter by more than $90^\circ$.

The experimental observation was "roughly **1 in 20,000**." The fact that our calculation is so close to the real-world experiment is what gave Rutherford and his team so much confidence in their new atomic model. It's a stunning success for physics!

I hope this detailed walkthrough was helpful! Do you have any questions about why the numbers aren't _exactly_ the same, or what this implies?