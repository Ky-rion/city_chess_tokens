

This is a wonderful problem! We are moving from the behaviour of individual particles to the collective behavior of the atomic nucleus. This is the realm of **Nuclear Physics**.

We are exploring the **"Valley of Stability."** Imagine a landscape where "Altitude" represents Energy. Nuclei want to be at the lowest possible energy (the bottom of the valley) to be stable. If they are up on the slopes, they will "roll down" via radioactive decay until they hit the bottom.

Here is the solution to your problem set.

---

### (a) How do $Z$, $N$, and $A$ change during $\beta$-decays or Electron Capture?

**The Professor's Insight:**

These decays are how nuclei move _sideways_ along the bottom of the valley to find the optimal balance of protons and neutrons.

- $Z$ = Atomic Number (Protons)
    
- $N$ = Neutron Number
    
- $A$ = Mass Number ($Z + N$)
    

**1. Beta-Minus Decay ($\beta^-$):**

A neutron turns into a proton (emitting an electron).

- **$Z$ (Protons):** Increases by 1 ($Z \rightarrow Z+1$)
    
- **$N$ (Neutrons):** Decreases by 1 ($N \rightarrow N-1$)
    
- **$A$ (Mass):** Stays constant (unchanged)
    

**2. Electron Capture (EC) / Beta-Plus Decay ($\beta^+$):**

A proton turns into a neutron (absorbing an electron).

- **$Z$ (Protons):** Decreases by 1 ($Z \rightarrow Z-1$)
    
- **$N$ (Neutrons):** Increases by 1 ($N \rightarrow N+1$)
    
- **$A$ (Mass):** Stays constant (unchanged)
    

> **Summary:** These processes swap protons for neutrons (or vice versa) while keeping the total number of nucleons ($A$) constant.

---

### (b) Derive the relationship between $Z$ and $A$ for the Valley of Stability using the Weizsäcker Mass Formula.

**The Professor's Insight:**

Nature is lazy. It always seeks the configuration with the **lowest energy** (and therefore the lowest mass, since $E=mc^2$).

To find the "stable" nucleus for a given mass number $A$, we need to find the value of $Z$ that minimizes the nucleus's mass.

**The Derivation:**

We start with the Semi-Empirical Mass Formula (SEMF). The mass of a nucleus $M(A,Z)$ is the sum of the parts minus the Binding Energy ($B$).

$$M(A,Z) = Z m_p + (A-Z) m_n - B(A,Z)$$

_(Note: We divide $B$ by $c^2$ strictly speaking, but in natural units $c=1$.)_

The problem states $m_p = m_n$, so the first part ($Z m_p + N m_n$) becomes just $A \cdot m_{nucleon}$, which is constant for a fixed $A$. To minimize Mass, we must **maximize Binding Energy ($B$)**.

The Binding Energy formula (using the problem's constants):

$$B(A,Z) = a_V A - a_S A^{2/3} - a_C \frac{Z^2}{A^{1/3}} - a_A \frac{(A-2Z)^2}{A} + \delta$$

_(Note: The asymmetry term uses $N-Z = (A-Z)-Z = A-2Z$. Also $a_P=0$ so $\delta=0$.)_

We take the derivative of $B$ with respect to $Z$ and set it to zero to find the maximum:

$$\frac{\partial B}{\partial Z} = \frac{\partial}{\partial Z} \left( - a_C \frac{Z^2}{A^{1/3}} - a_A \frac{(A-2Z)^2}{A} \right) = 0$$

Let's differentiate the terms:

1. **Coulomb Term:** $\frac{d}{dZ} (-a_C A^{-1/3} Z^2) = -2 a_C A^{-1/3} Z$
    
2. **Asymmetry Term:** $\frac{d}{dZ} (-a_A A^{-1} (A-2Z)^2) = -a_A A^{-1} \cdot 2(A-2Z) \cdot (-2) = \frac{4 a_A (A-2Z)}{A}$
    

Set the sum to zero:

$$\frac{4 a_A (A-2Z)}{A} - \frac{2 a_C Z}{A^{1/3}} = 0$$

Now, we solve for $Z$:

$$\frac{2 a_A (A-2Z)}{A} = \frac{a_C Z}{A^{1/3}}$$

$$2 a_A (A-2Z) = a_C Z A^{2/3}$$

$$2 a_A A - 4 a_A Z = a_C Z A^{2/3}$$

$$2 a_A A = Z (4 a_A + a_C A^{2/3})$$

$$Z_{stable} = \frac{2 a_A A}{4 a_A + a_C A^{2/3}}$$

Divide numerator and denominator by $2 a_A$:

$$Z_{stable} = \frac{A}{2 + \frac{a_C}{2a_A} A^{2/3}}$$

**Plugging in the numbers:**

- $a_C = 0.71 \text{ MeV}$
    
- $a_A = 23.29 \text{ MeV}$
    

$$\frac{a_C}{2 a_A} = \frac{0.71}{2 \times 23.29} = \frac{0.71}{46.58} \approx 0.0152$$

**Final Formula:**

$$Z_{stable} \approx \frac{A}{2 + 0.015 A^{2/3}}$$

> **Interpretation:** For small $A$, the denominator is $\approx 2$, so $Z \approx A/2$ (Protons = Neutrons). As $A$ gets huge, the denominator grows, making $Z < A/2$. We need _more_ neutrons than protons in heavy nuclei to glue them together against the electric repulsion!

---

### (c) Sketch the course of the Valley of Stability in the $Z$-$N$-Diagram.

**The Sketch Description:**

You should draw a graph with:

1. **X-axis:** Neutron Number $N$.
    
2. **Y-axis:** Atomic Number $Z$ (Protons).
    
3. **Reference Line:** Draw a straight diagonal line $N = Z$ (45 degrees).
    
4. **The Valley Line:**
    
    - Start at the origin ($0,0$).
        
    - For light elements (up to Calcium, $Z=20$), the line follows the $N=Z$ diagonal perfectly.
        
    - Above $Z=20$, the line begins to **bend downwards/rightwards** (towards the N-axis).
        
    - This means for heavy elements, $N > Z$. (e.g., Lead has 82 protons but 126 neutrons).
        

---

### (d) Which two processes are responsible for the fact that there are no stable nuclei for large values of $A$?

**The Professor's Insight:**

The question asks why the valley eventually _ends_. Why can't we build a nucleus the size of a watermelon?

As nuclei get bigger, the **Coulomb Repulsion** (protons repelling protons) grows with $Z^2$, while the **Strong Nuclear Force** (which holds them together) only grows with $A$ (neighbor-to-neighbor). Eventually, the electric force wins and tears the nucleus apart.

The two dominant "tear-apart" mechanisms for heavy nuclei are:

1. **Alpha Decay ($\alpha$):** The nucleus emits a Helium nucleus to quickly shed positive charge ($Z$) and reduce the Coulomb pressure.
    
2. **Spontaneous Fission:** The nucleus becomes so unstable that it simply splits into two large, roughly equal chunks. This happens when the repelling Coulomb force overcomes the Surface Tension holding the "drop" together.
    

---

### Professor's Check-in

You have successfully derived one of the most fundamental curves in physics!

- You showed mathematically why heavy elements have more neutrons ($Z < A/2$).
    
- You identified the "death" of heavy nuclei via fission and alpha decay.
    

**This completes the theoretical section. Would you like to review any part of the Weizsäcker Mass Formula, or are you ready for the next challenge?**