

This is it! Let's put everything together. We will use all the information from the problem and the equations we've derived to find the final answers.

Here is our plan:

1.  **Find the number of $^{12}$C atoms:** We'll use the total mass of carbon (1.2 g), the molar mass of $^{12}$C (12 g/mol), and Avogadro's number.
    
2.  **Find the _initial_ $^{14}$C atoms ($N_0$):** We'll use our result from Step 1 and the given atmospheric ratio.
    
3.  **Find the _current_ $^{14}$C atoms ($N(t)$):** We'll use the given current activity (845 decays/hour) and our derived relationship $A = \lambda N$. This will require us to be very careful with units!
    
4.  **Find the age ($t$):** We'll use the radioactive decay law, $N(t) = N_0 e^{-\lambda t}$, along with our calculated values for $N_0$ and $N(t)$.
    

---

### 1. ⚛️ Calculation of $^{12}$C Atoms

-   **Assumption:** The problem gives the total mass of carbon as 1.2 g. As we saw from the atmospheric ratio ($^{12}$C is $7.85 \times 10^{11}$ times more common than $^{14}$C), the sample's mass is almost _entirely_ from $^{12}$C. We can safely assume the full 1.2 g is $^{12}$C.
    
-   Step 1.1: Find moles of $^{12}$C.
    
    We use the formula: $\text{moles } (n) = \frac{\text{mass } (m)}{\text{Molar mass } (M)}$
    
    $n = 1.2 \text{ g} / 12 \text{ g/mol} = 0.1 \text{ mol}$
    
-   Step 1.2: Find atoms of $^{12}$C.
    
    We use Avogadro's number, $N_A \approx 6.022 \times 10^{23} \text{ atoms/mol}$.
    
    $\text{Number of atoms} = n \times N_A$
    
    $\text{Number of }^{12}\text{C atoms} = 0.1 \text{ mol} \times (6.022 \times 10^{23} \text{ atoms/mol})$
    

> **Number of $^{12}$C atoms ($N_{12}$) = $6.022 \times 10^{22}$ atoms**

---

### 2. 🕰️ Calculation of _Initial_ $^{14}$C Atoms ($N_0$)

-   **Concept:** At the moment the tree died ($t=0$), the ratio of its carbon isotopes matched the atmosphere. We use assumption (i).
    
-   **Given Ratio:** $\frac{\text{Number of }^{12}\text{C atoms}}{\text{Number of }^{14}\text{C atoms}} = 7.85 \times 10^{11}$
    
-   Calculation: We can write this as $\frac{N_{12}}{N_0} = 7.85 \times 10^{11}$. We just need to rearrange and solve for $N_0$.
    
    $N_0 = \frac{N_{12}}{7.85 \times 10^{11}}$
    
    $N_0 = \frac{6.022 \times 10^{22}}{7.85 \times 10^{11}}$
    
    $N_0 \approx 0.7671 \times 10^{11} \text{ atoms}$
    

> Initial Number of $^{14}$C atoms ($N_0$) $\approx 7.671 \times 10^{10}$ atoms
> 
> (This was the number of $^{14}$C atoms in the splinter when the tree died.)

---

### 3. 📉 Calculation of _Current_ $^{14}$C Atoms ($N(t)$)

-   **Concept:** We are given the _current activity_ $A(t) = 845 \text{ decays/hour}$. We know the activity is related to the number of atoms by $A(t) = \lambda N(t)$. To find $N(t)$, we must first find the decay constant $\lambda$.
    
-   Step 3.1: Find $\lambda$ in the correct units.
    
    The activity is in "per hour," so we must use a value for $\lambda$ in "per hour" (i.e., $\text{h}^{-1}$). We'll convert the half-life from years to hours.
    
    $t_{1/2} = 5730 \text{ years}$
    
    $t_{1/2} \text{ (in hours)} = 5730 \text{ a} \times 365.25 \text{ d/a} \times 24 \text{ h/d} \approx 50,227,380 \text{ hours}$
    
    Now use the formula from part (b):
    
    $\lambda = \frac{\ln(2)}{t_{1/2}}$
    
    $\lambda = 0.69315 / 50,227,380 \text{ h} \approx 1.3799 \times 10^{-8} \text{ h}^{-1}$
    
-   Step 3.2: Find $N(t)$.
    
    We rearrange the activity formula: $N(t) = \frac{A(t)}{\lambda}$
    
    $N(t) = 845 \text{ decays/hour} / (1.3799 \times 10^{-8} \text{ h}^{-1})$
    
    $N(t) \approx 612.36 \times 10^8 \text{ atoms}$
    

> Current Number of $^{14}$C atoms ($N(t)$) $\approx 6.124 \times 10^{10}$ atoms
> 
> (This is the number of $^{14}$C atoms today.)
> 
> _Self-check: $N(t)$ is less than $N_0$, which is exactly what we expect!_

---

### 4. 🌳 Calculation of the Splinter's Age ($t$)

-   **Concept:** We now have the starting amount ($N_0$), the current amount ($N(t)$), and the decay constant ($\lambda$). We can plug these into our main **Radioactive Decay Law** and solve for the one unknown variable: $t$.
    
-   Step 4.1: Set up the equation.
    
    $N(t) = N_0 e^{-\lambda t}$
    
-   Step 4.2: Isolate $t$.
    
    Divide by $N_0$:
    
    $\frac{N(t)}{N_0} = e^{-\lambda t}$
    
    Take the natural logarithm ($\ln$) of both sides to cancel the $e$:
    
    $\ln\left(\frac{N(t)}{N_0}\right) = -\lambda t$
    
    Solve for $t$:
    
    $t = -\frac{1}{\lambda} \ln\left(\frac{N(t)}{N_0}\right)$
    
-   Step 4.3: Substitute $\lambda$.
    
    This next step is a very common and useful trick. Instead of using our rounded number for $\lambda$, let's substitute the formula for $\lambda$ back in: $\lambda = \frac{\ln(2)}{t_{1/2}}$.
    
    $t = -\frac{1}{\frac{\ln(2)}{t_{1/2}}} \ln\left(\frac{N(t)}{N_0}\right)$
    
    $t = -\frac{t_{1/2}}{\ln(2)} \ln\left(\frac{N(t)}{N_0}\right)$
    
    Using the log rule $-\ln(a/b) = \ln(b/a)$, we can flip the fraction to get rid of the minus sign:
    
    $t = \frac{t_{1/2}}{\ln(2)} \ln\left(\frac{N_0}{N(t)}\right)$
    
    This is a beautiful formula. It lets us use the half-life directly (in years!) to get an answer (in years!).
    
-   **Step 4.4: Plug in the numbers and solve.**
    
    -   $t_{1/2} = 5730 \text{ years}$
        
    -   $\ln(2) \approx 0.69315$
        
    -   $N_0 = 7.671 \times 10^{10} \text{ atoms}$
        
    -   $N(t) = 6.124 \times 10^{10} \text{ atoms}$
        
    
    $t = \frac{5730}{0.69315} \ln\left(\frac{7.671 \times 10^{10}}{6.124 \times 10^{10}}\right)$
    
    $t = (8266.6) \times \ln(1.2526)$
    
    $t = (8266.6) \times (0.2252)$
    
    $t \approx 1861.6 \text{ years}$
    

> **The age of the wood splinter is $\approx 1862$ years.**

---

### 📜 Final Summary

-   **Number of $^{12}$C atoms:** $6.022 \times 10^{22}$ atoms
    
-   **$^{14}$C atoms at death ($N_0$):** $7.671 \times 10^{10}$ atoms
    
-   **$^{14}$C atoms today ($N(t)$):** $6.124 \times 10^{10}$ atoms
    
-   **Age of splinter ($t$):** **1862 years**
    

This completes the entire problem! We have successfully gone from the first principles of decay all the way to dating a real-world object.

Do you have any questions about these steps, or would you like to try another physics problem?