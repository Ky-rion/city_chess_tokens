

Hello there! Welcome to the class. It is always a pleasure to walk a curious student through the beautiful landscape of statistical thermodynamics.

The problem you are looking at is a classic "thermodynamic relation" problem. We are essentially trying to find the "cost" difference between heating a magnet when you hold the **external field** constant versus when you hold the **magnetization** constant.

Let's break down the solution provided by the other professor step-by-step. He uses a very standard, rigorous recipe that we use for almost all problems of this type.

### 1. The Setup: Defining the Heat Capacities

First, recall that heat capacity is basically "how much heat ($\delta Q$) do I need to add to change the temperature by a small amount ($dT$)?" Since reversible heat is $\delta Q = TdS$, we have $C = T \frac{\partial S}{\partial T}$.

We are given two different specific scenarios:

-   **$C_H$**: Heat capacity at constant magnetic field $H$.
    
-   **$C_M$**: Heat capacity at constant magnetization $M$.
    

The professor's note starts by stating the strategy: "we follow the same derivation as the one presented in lecture when deriving the connections between $C_V - C_p$". This is a great hint—if you remember how we connected specific heat at constant volume vs. pressure for a gas, this is the exact same math, just with magnetic variables!

---

### 2. Thinking in Total Differentials

To connect $C_M$ and $C_H$, we need to look at the entropy $S$.

Step A: Expand Entropy with respect to T and H

The professor starts by considering entropy as a function of temperature and field: $S(T, H)$.

We write the total differential for $S$:

$$dS = \left( \frac{\partial S}{\partial T} \right)_H dT + \left( \frac{\partial S}{\partial H} \right)_T dH$$

This equation tells us: "The total change in entropy is the change due to temperature (holding field fixed) plus the change due to field (holding temperature fixed)."

Step B: Expand the Field H

But we have a problem. We want to find a derivative where $M$ (Magnetization) is fixed, not $H$. So, we need to bring $M$ into the equation. We do this by expanding the differential for $H$, assuming $H$ is a function of $M$ and $T$: $H(M, T)$.

$$dH = \left( \frac{\partial H}{\partial M} \right)_T dM + \left( \frac{\partial H}{\partial T} \right)_M dT$$

---

### 3. Substitution and Comparison

Now, the clever part. We plug the expression for **$dH$** (from Step B) into the expression for **$dS$** (from Step A).

$$dS = \left( \frac{\partial S}{\partial T} \right)_H dT + \left( \frac{\partial S}{\partial H} \right)_T \left[ \left( \frac{\partial H}{\partial M} \right)_T dM + \left( \frac{\partial H}{\partial T} \right)_M dT \right]$$

The professor groups the terms that are multiplied by $dT$ together:

$$dS = \left( \frac{\partial S}{\partial H} \right)_T \left( \frac{\partial H}{\partial M} \right)_T dM + \left[ \left( \frac{\partial S}{\partial T} \right)_H + \left( \frac{\partial S}{\partial H} \right)_T \left( \frac{\partial H}{\partial T} \right)_M \right] dT$$

Why did we do this?

We are looking for $\left( \frac{\partial S}{\partial T} \right)_M$. This derivative literally means "change in $S$ over change in $T$ when $dM = 0$."

If we set $dM = 0$ in the massive equation above, the term with $dM$ vanishes, and we are left with exactly the expression inside the square brackets!

So, the professor writes:

$$\left( \frac{\partial S}{\partial T} \right)_M = \left( \frac{\partial S}{\partial T} \right)_H + \left( \frac{\partial S}{\partial H} \right)_T \left( \frac{\partial H}{\partial T} \right)_M$$

---

### 4. The Maxwell Relation

Now we have a mathematical identity, but we need to convert it into physical quantities we can measure (like susceptibility $\chi$).

The professor uses a **Maxwell Relation**. These are powerful shortcuts derived from the fact that thermodynamic potentials (like Gibbs Free Energy $G$) have continuous second derivatives.

From the potential $dG = -SdT - MdH$ (or similar depending on convention), we get the relation:

$$\left( \frac{\partial S}{\partial H} \right)_T = \left( \frac{\partial M}{\partial T} \right)_H$$

Substituting this back into our main equation gives us:

$$\left( \frac{\partial S}{\partial T} \right)_M = \left( \frac{\partial S}{\partial T} \right)_H + \left( \frac{\partial M}{\partial T} \right)_H \left( \frac{\partial H}{\partial T} \right)_M$$

---

### 5. The Cyclic Property (Triple Product Rule)

We are almost there, but we have an annoying term: $\left( \frac{\partial H}{\partial T} \right)_M$. This is the "change in field required to maintain constant magnetization as temperature changes." That's hard to measure directly.

To fix this, the professor uses the **cyclic property** of calculus. For any three variables $x, y, z$ related by a function, the product of their partial derivatives in a cycle is $-1$.

$$\left( \frac{\partial T}{\partial M} \right)_H \left( \frac{\partial M}{\partial H} \right)_T \left( \frac{\partial H}{\partial T} \right)_M = -1$$

We can rearrange this to solve for the annoying term:

$$\left( \frac{\partial H}{\partial T} \right)_M = - \frac{1}{\left( \frac{\partial T}{\partial M} \right)_H \left( \frac{\partial M}{\partial H} \right)_T} = - \frac{\left( \frac{\partial M}{\partial T} \right)_H}{\left( \frac{\partial M}{\partial H} \right)_T}$$

(Note: Recall that $\frac{1}{(\partial x / \partial y)} = (\partial y / \partial x)$).

---

### 6. The Final Assembly

Now, let's plug everything back into our entropy equation.

$$\left( \frac{\partial S}{\partial T} \right)_M = \left( \frac{\partial S}{\partial T} \right)_H - \frac{\left( \frac{\partial M}{\partial T} \right)_H^2}{\left( \frac{\partial M}{\partial H} \right)_T}$$

To turn these entropy derivatives into Heat Capacities ($C$), we multiply the whole equation by $T$ (since $C = T \frac{\partial S}{\partial T}$).

$$C_M = C_H - \frac{T \left( \frac{\partial M}{\partial T} \right)_H^2}{\left( \frac{\partial M}{\partial H} \right)_T}$$

The professor rearranges this to solve for $C_H$:

$$C_H = C_M + \frac{T \left( \frac{\partial M}{\partial T} \right)_H^2}{\left( \frac{\partial M}{\partial H} \right)_T}$$

The Final Polish:

We are given the definition of isothermal susceptibility: $\chi_T = \frac{1}{V} \left( \frac{\partial M}{\partial H} \right)_T$.

This implies $\left( \frac{\partial M}{\partial H} \right)_T = V \chi_T$.

Substituting this into the denominator, we get the final result:

$$C_H = C_M + \frac{T}{V \chi_T} \left( \frac{\partial M}{\partial T} \right)_H^2$$

And that matches the equation (2) you were asked to derive!

Physical Intuition:

This equation tells us that $C_H$ is generally larger than $C_M$ (since $T, V, \chi_T$, and the square term are usually positive). This makes sense: when you heat a material at constant field ($C_H$), the magnetization drops. The external field then has to do "work" to try to maintain the alignment, or rather, energy goes into the changing magnetic configuration. This requires more heat input than if you simply locked the spins in place ($C_M$).