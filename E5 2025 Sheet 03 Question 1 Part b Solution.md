

Ah, excellent! You've correctly anticipated that we would finally get to use that "extra" information. This question builds directly on our last one and requires us to connect the _activity_ of the sample to its _mass_.

This problem is a fantastic bridge between nuclear physics (decay rates) and chemistry (moles and mass). Let's lay out the full solution.

---

### The Goal: From Activity to Mass

Our main goal is to find the **initial mass ($m_0$)** of the plutonium.

Here's our chain of logic:

1.  Mass ($m_0$) is related to the **number of moles**.
    
2.  The number of moles is related to the **number of atoms ($N_0$)**.
    
3.  The initial number of atoms ($N_0$) is related to the **initial activity ($A_0$)**.
    
4.  We don't have the initial activity ($A_0$), but we _do_ have the activity when it reached Saturn ($A_S$) from part (a)! We can use the **Radioactive Decay Law** to work backward in time.
    

---

### 1. Step 1: Find the Initial Activity ($A_0$)

This is where we use the half-life and travel time. The law for radioactive decay is:

$A(t) = A_0 e^{-\lambda t}$

Where:

-   $A(t)$ is the activity at time $t$. We'll call this $A_S$ (Activity at Saturn).
    
-   $A_0$ is the initial activity at $t=0$ (at the start).
    
-   $t$ is the time elapsed. We'll call this $t_S$ (time to Saturn).
    
-   $\lambda$ (lambda) is the **decay constant**.
    

From part (a), we know the activity at Saturn was:

-   **$A_S = 9.096 \times 10^{15} \text{ decays/s}$**
    

The problem gives us the travel time and half-life:

-   **$t_S = 1467 \text{ days}$**
    
-   **$t_{1/2} = 88 \text{ years}$**
    

First, we must get all our time units to be consistent. It's easiest to convert everything to **seconds (s)**, since our activity is in decays per _second_.

#### A) Convert the Decay Constant ($\lambda$)

The decay constant $\lambda$ is related to the half-life $t_{1/2}$ by the formula:

$\lambda = \frac{\ln(2)}{t_{1/2}}$

Let's find the half-life in seconds:

-   $t_{1/2} \text{ (in s)} = 88 \text{ years} \times \frac{365.25 \text{ days}}{1 \text{ year}} \times \frac{24 \text{ h}}{1 \text{ day}} \times \frac{3600 \text{ s}}{1 \text{ h}}$
    
-   $t_{1/2} \approx 2.778 \times 10^9 \text{ s}$
    

Now, calculate $\lambda$:

-   $\lambda = \frac{\ln(2)}{2.778 \times 10^9 \text{ s}} \approx \frac{0.6931}{2.778 \times 10^9 \text{ s}}$
    
-   **$\lambda \approx 2.495 \times 10^{-10} \text{ s}^{-1}$**
    

#### B) Convert the Travel Time ($t_S$)

-   $t_S \text{ (in s)} = 1467 \text{ days} \times \frac{24 \text{ h}}{1 \text{ day}} \times \frac{3600 \text{ s}}{1 \text{ h}}$
    
-   **$t_S = 1.267 \times 10^8 \text{ s}$**
    

#### C) Solve for $A_0$

We rearrange our decay formula:

$A_S = A_0 e^{-\lambda t_S} \implies A_0 = \frac{A_S}{e^{-\lambda t_S}} = A_S e^{\lambda t_S}$

Now, plug in all our numbers:

-   $A_0 = (9.096 \times 10^{15} \text{ s}^{-1}) \times e^{(2.495 \times 10^{-10} \text{ s}^{-1} \times 1.267 \times 10^8 \text{ s})}$
    
-   Let's calculate the exponent first: $(2.495 \times 10^{-10}) \times (1.267 \times 10^8) \approx 0.03161$
    
-   $A_0 = (9.096 \times 10^{15}) \times e^{0.03161}$
    
-   $A_0 = (9.096 \times 10^{15}) \times (1.0321)$
    
-   **$A_0 \approx 9.388 \times 10^{15} \text{ decays/s}$**
    

This makes sense! The activity at the start ($A_0$) was slightly _higher_ than the activity when it reached Saturn ($A_S$), as the fuel has decayed along the way.

---

### 2. Step 2: Find the Initial Number of Atoms ($N_0$)

The _definition_ of activity ($A$) is that it's proportional to the number of atoms ($N$) present:

$A = \lambda N$

We can use this for our initial ($t=0$) values:

$A_0 = \lambda N_0$

Rearranging to find the initial number of atoms, $N_0$:

-   $N_0 = \frac{A_0}{\lambda}$
    
-   $N_0 = \frac{9.388 \times 10^{15} \text{ s}^{-1}}{2.495 \times 10^{-10} \text{ s}^{-1}}$
    
-   **$N_0 \approx 3.763 \times 10^{25} \text{ atoms}$**
    

This is the total number of ${}^{238}\text{Pu}$ atoms the probe must have had at launch.

---

### 3. Step 3: Find the Initial Mass ($m_0$)

Now we just need to "weigh" these atoms. We use two key constants:

1.  **Molar Mass ($M$):** $238 \text{ g/mol}$ (given in the problem)
    
2.  **Avogadro's Number ($N_A$):** $6.022 \times 10^{23} \text{ atoms/mol}$
    

First, let's find the mass of a _single_ ${}^{238}\text{Pu}$ atom ($m_{\text{atom}}$):

-   $m_{\text{atom}} = \frac{\text{Molar Mass}}{\text{Avogadro's Number}}$
    
-   $m_{\text{atom}} = \frac{238 \text{ g/mol}}{6.022 \times 10^{23} \text{ atoms/mol}}$
    
-   **$m_{\text{atom}} \approx 3.952 \times 10^{-22} \text{ g/atom}$**
    

Finally, find the total initial mass ($m_0$) by multiplying the number of atoms by the mass of one atom:

-   $m_0 = N_0 \times m_{\text{atom}}$
    
-   $m_0 = (3.763 \times 10^{25} \text{ atoms}) \times (3.952 \times 10^{-22} \text{ g/atom})$
    
-   **$m_0 \approx 14870 \text{ g}$**
    

The question asks for kilograms, so we just convert:

-   **$m_0 \approx 14.87 \text{ kg}$**
    

---

### Final Answer

The probe required **14.87 kg** of ${}^{238}\text{Pu}$ at the start of its mission to be able to provide 400 W of electric power by the time it reached Saturn.

That's a significant amount of material, but it's been powering the Voyager 2 probe for (as of 2024) over 47 years!

Are you ready for the final part of this problem?