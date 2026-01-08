

Hello there! Welcome to my office hours. I am delighted to help you tackle this problem. Thermodynamics is a beautiful subject because it takes these messy, chaotic collections of particles and gives us elegant, predictable rules.

Today, we are looking at a "real gas." You might remember the **Ideal Gas Law** ($PV=N k_B T$), which assumes gas particles don't interact and take up no space. It's a great lie, but often too simple. The **Van der Waals** gas is the famous correction, but in this problem ("Aufgabe 2"), we are exploring a _different_ realistic approximation.

Let's walk through the solution provided by your other professor together.

### 1. The Setup: What is a Critical Point?

First, look at the equation of state given in the problem:

$$P = \frac{N k_B T}{V - Nb} e^{-\frac{a N}{V k_B T}}$$

We are asked to find the **critical values** $V_c$, $T_c$, and $P_c$.

**Concept Check:** Imagine compressing a gas at a constant temperature.

-   At high temperatures, the pressure just goes up smoothly as volume goes down.
    
-   At low temperatures, the gas suddenly condenses into a liquid, creating a flat line on the $P-V$ diagram (a phase transition).
    
-   The **Critical Point** is the specific boundary case between these two behaviors. Mathematically, it is an **inflection point** on the isotherm (the $P-V$ curve at constant $T$).
    

Because it's a flat inflection point, two conditions must be met simultaneously:

1.  The slope is zero: $\frac{\partial P}{\partial V} \big|_{T_c} = 0$
    
2.  The curvature is zero: $\frac{\partial^2 P}{\partial V^2} \big|_{T_c} = 0$
    

Our strategy is simply to calculate these two derivatives, set them to zero, and solve the algebra!

### 2. The First Derivative

Let's take the derivative of our pressure equation with respect to volume $V$. This requires the **product rule** because $V$ appears in the fraction term and in the exponential term.

$$P = \underbrace{\left(\frac{N k_B T}{V - Nb}\right)}_{Term 1} \cdot \underbrace{\left(e^{-\frac{a N}{V k_B T}}\right)}_{Term 2}$$

Differentiating yields:

$$\frac{\partial P}{\partial V} = P \cdot \left[ \frac{aN}{V^2 k_B T} - \frac{1}{V-Nb} \right] = 0$$

Wait, how did we get there so fast?

-   Differentiating _Term 1_ gives a factor of $-\frac{1}{(V-Nb)^2}$.
    
-   Differentiating _Term 2_ brings down a factor of $+\frac{aN}{V^2 k_B T}$ from the exponent.
    
-   When you factor out the original $P$, you are left with the bracketed term above.
    

Since $P$ is not zero, the term in the brackets _must_ be zero. This gives us our first major clue:

$$\frac{aN}{V_c^2 k_B T_c} = \frac{1}{V_c - Nb}$$

If we rearrange this to solve for temperature, we get:

$$T_c = \frac{aN}{k_B} \frac{V_c - Nb}{V_c^2}$$

### 3. The Second Derivative (and a Professor's Trick)

Now we need the second derivative $\frac{\partial^2 P}{\partial V^2} = 0$.

Taking the derivative of the result we just found looks messy, but here is a standard physicist's trick used in the solution. We are differentiating the expression $\frac{\partial P}{\partial V}$. We know that $\frac{\partial P}{\partial V}$ is a product of $P$ and the bracket term $[\dots]$.

$$\frac{\partial^2 P}{\partial V^2} = \frac{\partial P}{\partial V} \cdot [\dots] + P \cdot \frac{\partial}{\partial V}[\dots]$$

**The Trick:** We already know that at the critical point, $\frac{\partial P}{\partial V} = 0$. So the first part of this product rule vanishes!. We only need to differentiate the bracket term itself and set it to zero.

So, we differentiate the bracket $\left[ \frac{aN}{V^2 k_B T} - \frac{1}{V-Nb} \right]$ with respect to $V$:

$$-\frac{2aN}{V^3 k_B T} + \frac{1}{(V-Nb)^2} = 0$$

This simplifies to our second major clue:

$$\frac{2aN}{V_c^3 k_B T_c} = \frac{1}{(V_c - Nb)^2}$$

### 4. Solving the System (The Finale)

Now we have a system of two equations.

1.  **From 1st derivative:** $\frac{aN}{V_c^2 k_B T_c} = \frac{1}{V_c - Nb}$
    
2.  **From 2nd derivative:** $\frac{2aN}{V_c^3 k_B T_c} = \frac{1}{(V_c - Nb)^2}$
    

Divide the second equation by the first (or substitute). The solution source does a nice substitution:

It sees that $\frac{aN}{V_c^2 k_B T_c}$ is exactly equal to $\frac{1}{V_c - Nb}$.

So, look at the Left Hand Side of equation 2. It can be written as $\frac{2}{V_c} \cdot \left( \frac{aN}{V_c^2 k_B T_c} \right)$.

Substituting Eq 1 into Eq 2 gives:

$$\frac{2}{V_c} \cdot \frac{1}{V_c - Nb} = \frac{1}{(V_c - Nb)^2}$$

Cancel one $\frac{1}{V_c - Nb}$ from both sides:

$$\frac{2}{V_c} = \frac{1}{V_c - Nb}$$

Cross-multiply:

$$2(V_c - Nb) = V_c$$

$$2V_c - 2Nb = V_c$$

$$V_c = 2Nb$$

We have found the **Critical Volume**!

Finding Critical Temperature ($T_c$):

Plug $V_c = 2Nb$ back into our equation for $T_c$ (from Step 2):

$$T_c = \frac{aN}{k_B} \frac{(2Nb - Nb)}{(2Nb)^2} = \frac{aN}{k_B} \frac{Nb}{4N^2 b^2}$$

$$T_c = \frac{a}{4b k_B}$$

Finding Critical Pressure ($P_c$):

Finally, substitute $V_c$ and $T_c$ back into the very first pressure equation given in the problem statement.

$$P_c = \frac{N k_B ( \frac{a}{4b k_B} )}{2Nb - Nb} \exp\left(-\frac{a N}{2Nb \cdot k_B \cdot \frac{a}{4b k_B}}\right)$$

Let's clean up the fraction:

Numerator: $\frac{Na}{4b}$

Denominator: $Nb$

Result: $\frac{a}{4b^2}$

Now the exponent:

$-\frac{aN}{ \frac{2Nb k_B a}{4b k_B} } = -\frac{aN}{ \frac{aN}{2} } = -2$

So, the final pressure is:

$$P_c = \frac{a}{4b^2} e^{-2}$$

### Summary of Results

Here are the critical values for this specific real gas:

-   **Critical Volume:** $V_c = 2Nb$
    
-   **Critical Temperature:** $T_c = \frac{a}{4b k_B}$
    
-   **Critical Pressure:** $P_c = \frac{a}{4b^2} e^{-2}$
    

And there you have it! You have successfully characterized the phase transition point for this gas.

**Would you like to move on to "Aufgabe 3" and discuss how these principles apply to Superconductors?**