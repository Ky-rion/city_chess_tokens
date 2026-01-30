

![[Pasted image 20260128115747.png]]

Welcome back! You have successfully moved from playing billiards (elastic scattering) to smashing atoms (inelastic scattering).

In **Part (d)**, we are given a specific scenario to test our new formulas.

The problem states: **"Let the scattered electron energy be $E' = 10 \text{ GeV}$."**

Wait, recall Part (b). When the collision was elastic (the proton stayed whole), the electron _had_ to come out with **17.8 GeV**. Now, it's coming out with only **10 GeV**.

-   **Where did that extra energy go?** It didn't disappear. It was used to blow the proton apart!
    
-   Because $E' (10) < E'_{elastic} (17.8)$, we know for a fact this is **Inelastic Scattering**.
    

Let's walk through the calculations in the solution.

---

### 1. Calculate the New Momentum Transfer ($Q^2$)

Even though the proton broke, the electron interaction is still the same: it came in, emitted a virtual photon, and left. So, we use the exact same formula for $Q^2$ as we did in Part (b), just with our new energy $E'$.

**The Formula:**

$$Q^2 = \frac{2 E E'}{c^2} (1 - \cos\theta)$$

**The Calculation:**

-   $E = 25 \text{ GeV}$
    
-   $E' = 10 \text{ GeV}$ (New value!)
    
-   $1 - \cos(10^\circ) \approx 0.0152$
    

$$Q^2 = 2 \times 25 \times 10 \times 0.0152$$

$$Q^2 = 500 \times 0.0152 \approx 7.60 \text{ GeV}^2/c^2$$

**Physics Note:** Notice that $Q^2$ is smaller here ($7.6$) than in the elastic case ($13.5$). This is because the outgoing electron is slower (has less momentum), so the difference between "in" and "out" is smaller.

---

### 2. Derive and Calculate the Invariant Mass ($W$)

This is the most important derivation in this section. We need to find the mass of the "hadronic system" (the debris cloud).

**The Derivation:**

Start with conservation of four-momentum:

$$P' = P + q$$

_(Debris momentum = Proton momentum + Photon kick)_

Square both sides (remember, squaring a four-vector gives its mass squared):

$$P'^2 = (P + q)^2$$

$$W^2 c^2 = P^2 + 2(P \cdot q) + q^2$$

Now, let's identify what each term means:

1.  **$P^2$**: The squared mass of the original target proton.
    
    $$P^2 = m_p^2 c^2$$
    
2.  **$q^2$**: The squared mass of the virtual photon. By definition, $Q^2 = -q^2$.
    
    $$q^2 = -Q^2$$
    
3.  **$2(P \cdot q)$**: The interaction term.
    
    -   $P = (m_p c, 0, 0, 0)$
        
    -   $q = ( (E-E')/c, \dots )$
        
    -   Dot product: $P \cdot q = m_p c \cdot \frac{E - E'}{c} = m_p (E - E')$
        

Substitute these back into the main equation:

$$W^2 c^2 = m_p^2 c^2 + 2 m_p (E - E') - Q^2$$

**The Calculation:**

Let's plug in the numbers. Be careful with units (we will work in GeV):

-   $m_p = 0.938 \text{ GeV}$
    
-   $m_p^2 = (0.938)^2 \approx 0.88 \text{ GeV}^2$
    
-   $E - E' = 25 - 10 = 15 \text{ GeV}$ (Energy lost by electron)
    
-   $Q^2 = 7.60 \text{ GeV}^2$
    

$$W^2 = 0.88 + 2(0.938)(15) - 7.60$$

$$W^2 = 0.88 + 28.14 - 7.60$$

$$W^2 = 21.42 \text{ GeV}^2$$

Now, take the square root to find the mass:

$$W = \sqrt{21.42} \approx 4.63 \text{ GeV}/c^2$$

**Result:** The "blob" of particles created by the collision has a mass of **4.63 GeV**. This is much heavier than the original proton (0.938 GeV), proving that we created new matter!

---

### 3. Calculate the Bjorken Variable ($x$)

Finally, we calculate $x$ to confirm how "inelastic" this collision was.

**The Formula:**

$$x = \frac{Q^2}{2 P \cdot q} = \frac{Q^2}{2 m_p (E - E')}$$

**The Calculation:**

-   Numerator: $7.60$
    
-   Denominator: $2 \times 0.938 \times 15 = 28.14$
    

$$x = \frac{7.60}{28.14} \approx 0.270$$

**The Meaning:**

-   Since $x = 0.270$ (which is much less than 1), this confirms the scattering is **Deeply Inelastic**.
    
-   Physical interpretation: The electron didn't hit the _whole_ proton. It hit a constituent part (a quark) that carried roughly **27%** of the proton's total momentum.
    

You have now completed the full analysis of an electron scattering event! You've calculated the kinematics for when the proton stays whole (elastic) and for when it shatters (inelastic).

**Would you like me to summarize the differences between Elastic and Inelastic scattering in a comparison table for your revision notes?**