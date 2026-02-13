

![[Pasted image 20260206195039.png]]

Welcome back! You are making excellent progress. We have identified the four members of the $\Delta$ family and their charges.

Now, for **Part (c)**, we are going to look at the "end of life" for these particles. Since $\Delta$ baryons are very heavy and unstable, they decay (break apart) almost instantly.

The question is: **What do they turn into?**

To answer this, we need to balance two "budgets":

1. **The Energy Budget** (Mass)
    
2. **The Quantum Identity Budget** (Isospin $I_3$)
    

---

### 1. The Energy Budget: Why Nucleons and Pions?

First, look at the mass provided in the solution:

- Mass of $\Delta \approx 1232 \text{ MeV}/c^2$.
    

Nature loves to move from high energy to low energy. The $\Delta$ wants to break into lighter particles. The closest lighter relatives are:

- **Nucleons** (Protons and Neutrons): Mass $\approx 938 \text{ MeV}/c^2$.
    
- **Pions** ($\pi$ mesons): Mass $\approx 140 \text{ MeV}/c^2$.
    

If you add a Nucleon and a Pion together ($938 + 140 \approx 1078 \text{ MeV}/c^2$), the total is _less_ than the $\Delta$ mass ($1232 \text{ MeV}/c^2$). This means the decay is energetically allowed!

So, the general rule is:

$$\Delta \to \text{Nucleon} + \text{Pion}$$

---

### 2. The Identity Budget: Conservation of $I_3$

Since this decay happens via the **Strong Interaction** (it happens very fast), we must obey a strict rule: **Isospin ($I_3$) must be conserved.**

The total $I_3$ value _before_ the decay must equal the total $I_3$ value _after_ the decay.

To verify this, we first need to know the "ID numbers" ($I_3$) for the potential children: the Nucleons and the Pions. Your solution calculates these using the relation $I_3 = Q - Y/2$.

#### The Children:

- **Proton ($p$):** Charge $Q=1$, Hypercharge $Y=1$.
    
    $$I_3 = 1 - 1/2 = \mathbf{+1/2}$$
    
- **Neutron ($n$):** Charge $Q=0$, Hypercharge $Y=1$.
    
    $$I_3 = 0 - 1/2 = \mathbf{-1/2}$$
    
- **Pion Plus ($\pi^+$):** Charge $Q=1$, Hypercharge $Y=0$ (since it's a meson with no strangeness).
    
    $$I_3 = 1 - 0 = \mathbf{+1}$$
    
- **Pion Neutral ($\pi^0$):** Charge $Q=0$.
    
    $$I_3 = 0 - 0 = \mathbf{0}$$
    
- **Pion Minus ($\pi^-$):** Charge $Q=-1$.
    
    $$I_3 = -1 - 0 = \mathbf{-1}$$
    

---

### 3. Matching Parents to Children

Now, let's look at each $\Delta$ parent and see which combination of children adds up to the correct $I_3$.

#### Case 1: The $\Delta^{++}$ ($I_3 = +3/2$)

We need children that add up to $+1.5$.

- Try Proton ($+0.5$) + $\pi^+$ ($+1$).
    
- Sum: $0.5 + 1 = 1.5$. **Match!**
    
    $$\Delta^{++} \to p + \pi^+$$
    

#### Case 2: The $\Delta^{+}$ ($I_3 = +1/2$)

We need children that add up to $+0.5$. We have two options here:

- **Option A:** Proton ($+0.5$) + $\pi^0$ ($0$). Sum $= +0.5$.
    
- **Option B:** Neutron ($-0.5$) + $\pi^+$ ($+1$). Sum $= +0.5$.
    
    $$\Delta^{+} \to p + \pi^0 \quad \text{OR} \quad \Delta^{+} \to n + \pi^+$$
    
    _Both decays occur in nature!_
    

#### Case 3: The $\Delta^{0}$ ($I_3 = -1/2$)

We need children that add up to $-0.5$. Again, two options:

- **Option A:** Neutron ($-0.5$) + $\pi^0$ ($0$). Sum $= -0.5$.
    
- **Option B:** Proton ($+0.5$) + $\pi^-$ ($-1$). Sum $= -0.5$.
    
    $$\Delta^{0} \to n + \pi^0 \quad \text{OR} \quad \Delta^{0} \to p + \pi^-$$
    

#### Case 4: The $\Delta^{-}$ ($I_3 = -3/2$)

We need children that add up to $-1.5$.

- Try Neutron ($-0.5$) + $\pi^-$ ($-1$).
    
- Sum: $-0.5 - 1 = -1.5$. **Match!**
    
    $$\Delta^{-} \to n + \pi^-$$
    

---

### Summary Table

Here is the complete list of decays derived from Isospin conservation:

|**Parent**|**I3​ (Parent)**|**Decay Products**|**I3​ (Products)**|
|---|---|---|---|
|$\Delta^{++}$|$+3/2$|$p + \pi^+$|$+1/2 + 1 = +3/2$|
|$\Delta^{+}$|$+1/2$|$p + \pi^0$|$+1/2 + 0 = +1/2$|
|||$n + \pi^+$|$-1/2 + 1 = +1/2$|
|$\Delta^{0}$|$-1/2$|$n + \pi^0$|$-1/2 + 0 = -1/2$|
|||$p + \pi^-$|$+1/2 - 1 = -1/2$|
|$\Delta^{-}$|$-3/2$|$n + \pi^-$|$-1/2 - 1 = -3/2$|

You might notice that for $\Delta^+$ and $\Delta^0$, there are two possibilities. In a real experiment, these don't happen 50/50!

Would you like me to show you how to calculate the **Branching Ratios** (the probability of one decay vs. the other) using something called **Clebsch-Gordan coefficients**? That is usually the "bonus points" part of this question!