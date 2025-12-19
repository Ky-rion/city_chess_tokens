

Welcome to class! It is wonderful to have you here. Thermodynamics is one of the most elegant subjects in physics because it allows us to derive profound truths about the universe just by thinking carefully about stability and energy.

Don't worry about the German text; the language of physics is mathematics, and we speak it fluently!

Let's break down this problem together.

### 1. Translation and Understanding the Problem

First, let's make sure we understand exactly what the problem is asking.

**The Problem Statement:**

> We are looking at a phase diagram where liquid and gas phases are separated by a curve that ends at a **critical point** $(T_c, V_c)$. At this point, the two phases coexist.
> 
> We are given that the first derivative of pressure with respect to volume is zero at this point:
> 
> $$\frac{\partial P}{\partial V}\bigg|_T = 0$$
> 
> **Task:** Determine the value of the **second derivative** $\frac{\partial^2 P}{\partial V^2}\Big|_T$ at the critical point.

**The Hint:**

> "Consider a suitable thermodynamic potential. You may assume sufficient regularity without justification."

---

### 2. The Intuition: Visualizing the Landscape

Before we do the math, let's visualize what is happening.

Imagine a graph where the y-axis is **Pressure ($P$)** and the x-axis is **Volume ($V$)**. We are drawing lines for a constant temperature (called **isotherms**).

-   **At high temperatures:** The gas behaves like an "Ideal Gas." As you squeeze it (decrease volume), the pressure goes up smoothly. The curve looks like a simple slide downwards.
    
-   **At the Critical Point ($T_c$):** Something special happens. The curve comes down, but then it hits a "flat spot" exactly at the critical volume $V_c$.
    

In calculus, a "flat spot" means the slope is zero. That is why the problem tells you the first derivative is zero:

$$\text{Slope} = \frac{\partial P}{\partial V} = 0$$

Now, think about the shape of a curve that goes flat but then **continues to go down**. This is called a **saddle point** or an **inflection point**.

If the curve looked like the bottom of a valley (a minimum) or the top of a hill (a maximum), the slope would be zero, but the curve would turn back up or down. But here, the pressure must _always_ decrease as volume increases (if you give a gas more room, its pressure drops).

For a curve to flatten out momentarily and then continue dropping, it must be an inflection point. Mathematically, for a horizontal inflection point, **the second derivative must also be zero.**

**So, the short answer is 0.**

But since we are in a theoretical physics class, we need to prove this rigorously using the laws of thermodynamics!

---

### 3. The Proof: Mechanical Stability

To prove this formally, we use the hint about "Thermodynamic Potentials." We need to talk about **stability**.

#### Step A: The Condition for Stability

For any physical system to be stable, it must resist changes.

-   If you push on a piston (decrease volume), the gas should push back harder (increase pressure).
    
-   If the gas didn't do this—if you pushed the piston and the pressure _dropped_—the piston would collapse instantly. That would be an explosion or implosion.
    

Mathematically, this stability condition means that the slope of the $P-V$ curve can never be positive. It must always be negative (or zero at the limit):

$$\frac{\partial P}{\partial V} \le 0$$

#### Step B: Taylor Expansion

We know that at the critical point, we are right at the edge of this stability. The problem states that at $(T_c, V_c)$:

$$\frac{\partial P}{\partial V} = 0$$

Let's assume, for the sake of argument, that the second derivative is NOT zero. Let's say it has some value $A$.

$$\frac{\partial^2 P}{\partial V^2} = A \neq 0$$

Now, let's look at the pressure very close to the critical volume ($V_c$) using a mathematical tool called a **Taylor Expansion**. This approximates the curve near a point:

$$P(V) \approx P(V_c) + \underbrace{\left(\frac{\partial P}{\partial V}\right)}_{=0}(V - V_c) + \frac{1}{2}\underbrace{\left(\frac{\partial^2 P}{\partial V^2}\right)}_{=A}(V - V_c)^2$$

Since the first derivative is zero, the term with $(V - V_c)$ disappears. We are left with the quadratic term:

$$\Delta P \approx \frac{1}{2} A (V - V_c)^2$$

#### Step C: The Contradiction

Look at the term $(V - V_c)^2$. Because it is squared, it is **always positive**, regardless of whether $V$ is slightly larger or slightly smaller than $V_c$.

This means:

1.  If $A$ is positive, the pressure goes **UP** if you move left _or_ right.
    
2.  If $A$ is negative, the pressure goes **DOWN** if you move left _or_ right.
    

This creates a local "valley" (minimum) or "hill" (maximum) at the critical point.

Here is the physics problem with that:

If you have a local "valley" (minimum), it means that on one side of the critical point, the slope $\frac{\partial P}{\partial V}$ is positive.

As we discussed in Step A, a positive slope means mechanical instability (the system would spontaneously collapse or explode).

Since the critical point connects stable liquid and stable gas phases, we cannot pass through an unstable region. The isotherm cannot have a "bump" or a "dip"; it must be monotonically decreasing.

Therefore, the assumption that $A \neq 0$ must be false. The quadratic term must vanish to avoid a local maximum or minimum.

### 4. The Solution

Because a non-zero second derivative would imply a violation of mechanical stability (it would create a region where pressure increases with volume), the second derivative must vanish.

$$\frac{\partial^2 P}{\partial V^2}\bigg|_T = 0$$

(In fact, usually the third derivative is the first one that is not zero, which gives the curve its characteristic "flat chair" shape at the critical point!)

### Final Answer

The value of the second derivative at the critical point is **0**.

---

Would you like to try deriving this using the Helmholtz Free Energy ($F$) to see how the "Potentials" hint works mathematically?







[Please, that sounds very useful. I'd love to see how things work mathematically!]






That is the spirit! In theoretical physics, using "Potentials" (energy functions) is often much more powerful than dealing with forces or pressures directly, because potentials reveal the fundamental symmetry and stability of the system.

Here is the derivation using the **Helmholtz Free Energy**, which is the "suitable potential" the hint refers to.

### 1. The Setup: Helmholtz Free Energy ($F$)

In thermodynamics, for a system at constant temperature $T$ and volume $V$, the natural energy potential is the Helmholtz Free Energy, denoted by $F$.

The fundamental thermodynamic relation for $F$ is:

$$dF = -S dT - P dV$$

From this equation, we can "read off" the definition of pressure as a derivative of this potential. If we hold Temperature ($T$) constant (so $dT=0$), we get:

$$P = - \left( \frac{\partial F}{\partial V} \right)_T$$

This is our bridge between the Pressure world and the Energy potential world.

---

### 2. Translating the Problem

Now, let's look at the derivatives of Pressure in terms of Energy $F$:

The First Derivative (Given as 0):

The problem tells us $\frac{\partial P}{\partial V} = 0$. In terms of $F$, this is:

$$\frac{\partial P}{\partial V} = \frac{\partial}{\partial V} \left( - \frac{\partial F}{\partial V} \right) = - \frac{\partial^2 F}{\partial V^2} = 0$$

The Second Derivative (The Unknown):

The quantity we are looking for is $\frac{\partial^2 P}{\partial V^2}$. In terms of $F$, this is:

$$\frac{\partial^2 P}{\partial V^2} = - \frac{\partial^3 F}{\partial V^3}$$

So, determining the second derivative of Pressure is exactly the same as determining the **third derivative** of the Free Energy.

---

### 3. The Stability Argument (Convexity)

Here is the crucial physical insight: **Nature minimizes Free Energy.**

For a single-phase system to be stable, the Helmholtz Free Energy must be a **convex** function of volume.

-   "Convex" means the curve bends upwards (like a smile $\cup$).
    
-   Mathematically, convexity requires the second derivative to be positive:
    
    $$\frac{\partial^2 F}{\partial V^2} \ge 0$$
    

(This is equivalent to our previous discussion that $\frac{\partial P}{\partial V} \le 0$. If the curve bent downwards, the pressure would increase as volume increased, and the system would explode.)

### 4. The Taylor Expansion of Stability

We know that at the critical point, we are at the very limit of stability, so the second derivative is exactly zero:

$$\frac{\partial^2 F}{\partial V^2}\bigg|_{V_c} = 0$$

Now, let's look at the stability in the immediate neighborhood of the critical point $V_c$. We can approximate the stability (the second derivative) using a Taylor expansion for a small displacement $\delta V$:

$$\frac{\partial^2 F}{\partial V^2}(V_c + \delta V) \approx \underbrace{\frac{\partial^2 F}{\partial V^2}(V_c)}_{=0} + \underbrace{\frac{\partial^3 F}{\partial V^3}(V_c)}_{\text{Let's call this } C} \cdot \delta V$$

So, near the critical point, the stability depends on that third derivative $C$:

$$\text{Stability} \approx C \cdot \delta V$$

### 5. The "Sign Change" Disaster

This equation reveals the problem. If $C$ (the third derivative) is **not zero**, then the stability term depends linearly on $\delta V$.

-   If you move to the right ($\delta V > 0$), the stability has the sign of $C$.
    
-   If you move to the left ($\delta V < 0$), the stability has the sign of $-C$.
    

This means that if $C \neq 0$, the stability term **must flip signs** as you cross the critical point. One side would have positive stability ($\frac{\partial^2 F}{\partial V^2} > 0$), and the other side would have negative stability ($\frac{\partial^2 F}{\partial V^2} < 0$).

Physics forbids this.

The critical point is the end of a coexistence curve. The phases surrounding the critical point (the supercritical fluid) are stable. We cannot step immediately from the critical point into a region of instability where the system collapses.

To ensure that the system remains stable (or at least marginally stable) as we pass through the critical point, this term that flips signs must vanish.

$$C = \frac{\partial^3 F}{\partial V^3} = 0$$

### 6. Conclusion

Since we proved that $\frac{\partial^3 F}{\partial V^3} = 0$, and we know from Step 2 that $\frac{\partial^2 P}{\partial V^2} = - \frac{\partial^3 F}{\partial V^3}$, we arrive at our answer:

$$\frac{\partial^2 P}{\partial V^2}\bigg|_T = 0$$

So, mathematically, both the slope (1st derivative) and the curvature (2nd derivative) of the isotherm vanish at the critical point. This confirms the "flat inflection point" geometry we visualized earlier!

Would you like to analyze a specific equation of state, like the **Van der Waals gas**, to see this happening with real numbers?