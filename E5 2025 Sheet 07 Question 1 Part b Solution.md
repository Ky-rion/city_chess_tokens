

![[Pasted image 20260206194809.png]]

Welcome back to class! Excellent job following along with the spin conservation. Now we are moving on to one of the most elegant concepts in physics: **Parity ($P$)**.

In Part (A), we narrowed down the orbital angular momentum ($l$) to either 1 or 2. In Part (B), the problem gives us a hint ("from the angular distribution... $l=1$") that locks in the value. Now we use that to find the **Intrinsic Parity** of the parent particle.

### The Concept: What is Parity?

In quantum mechanics, Parity is essentially a "mirror test." If you flip the coordinates of the universe (turn left into right, up into down), does the particle's wave function stay the same ($+1$) or does it flip its sign ($-1$)?

- **Parity $+1$ (Even):** The object looks the same in a mirror.
    
- **Parity $-1$ (Odd):** The object looks "negative" or inverted in a mirror.
    

### The Golden Rule: Parity Conservation

Just like we conserved angular momentum in Part (A), we must conserve Parity here.

> **Crucial Rule:** The Strong Force (which causes this decay) **always conserves parity**.
> 
> Therefore:
> 
> $$\text{Total Parity}_{\text{ (Parent)}} = \text{Total Parity}_{\text{ (Daughters)}}$$

---

### Step 1: Breakdown of the "After" State (The Daughters)

The total parity of the final state is the product of three things:

1. The intrinsic parity of the **Neutron**.
    
2. The intrinsic parity of the **Pion**.
    
3. The **Orbital Parity** (coming from their motion relative to each other).
    

Unlike energy or momentum which you _add_, Parity is a **multiplicative** quantum number.

$$P_{\text{total}} = P_{\text{neutron}} \times P_{\text{pion}} \times P_{\text{orbital}}$$

Let's find the value for each:

#### 1. The Neutron ($n$)

The neutron is a **Fermion** (a matter particle). By convention in physics, we define the intrinsic parity of regular quarks and fermions (like protons and neutrons) as **positive (+1)**.

- **$P_n = +1$**
    

#### 2. The Pion ($\pi^+$)

The pion is a specific type of meson. It is famous in particle physics for being a "pseudoscalar." That is a fancy way of saying it has spin 0 but **negative** parity. (This is because it is made of a quark and an antiquark in an $L=0$ state; the antiquark contributes a $-1$ parity).

- **$P_{\pi} = -1$**
    

#### 3. The Orbital Parity ($P_{\text{orbital}}$)

This is determined by the motion $l$. The rule for orbital parity is simple but strict:

$$P_{\text{orbital}} = (-1)^l$$

The problem states that $l = 1$.

- **$P_{\text{orbital}} = (-1)^1 = -1$**
    

---

### Step 2: Doing the Math

Now, let's assemble the pieces to find the unknown parity of the parent $\Delta^+$.

$$P(\Delta^+) = P(n) \times P(\pi^+) \times P_{\text{orbital}}$$

Substitute the values we found:

$$P(\Delta^+) = (+1) \times (-1) \times (-1)$$

$$P(\Delta^+) = +1$$

### Conclusion

The intrinsic parity of the $\Delta^+$ particle is **Positive ($+1$)**.

This fits perfectly with the solution provided by the other professor. When they wrote:

$$P|\Delta^+\rangle = (-1)^1 (+1)(-1)|n\pi^+\rangle$$

They were showing exactly this multiplication: $(\text{Orbital}) \times (\text{Neutron}) \times (\text{Pion})$.

**Summary of the physics logic:**

Because the two daughter particles (neutron and pion) have opposite intrinsic parities, and they are rotating around each other with $l=1$ (which adds another factor of -1), the two negatives cancel out, leaving the total system—and thus the parent particle—with positive parity.

**Would you like to move on to the next part where we might look at the quark composition to double-check this result?**