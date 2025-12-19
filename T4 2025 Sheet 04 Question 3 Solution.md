

Welcome to the office hour! It is wonderful to see your enthusiasm. This is actually a very beautiful and classic problem in thermodynamics and fluid mechanics. What we are looking at here is the derivation of the **Young-Laplace Equation**.

Don't let the German text scare you; the physics is universal. The problem asks us to look at a spherical water droplet and prove a specific relationship between the pressure inside the drop, the pressure outside, and the surface tension.

Let's walk through this derivation together, step-by-step.

---

### 1. The Setup: What are we looking at?

Imagine a perfect sphere of water floating in the air.

-   **$R$:** The radius of the droplet.
    
-   **$P_{\text{in}}$:** The pressure _inside_ the water droplet.
    
-   **$P_{\text{um}}$:** The ambient pressure _outside_ (the surroundings).
    
-   **$\mathcal{S}$:** The **surface tension** (often denoted as $\gamma$ or $\sigma$ in other textbooks, but here it is $\mathcal{S}$).
    

The Core Concept:

Nature hates creating new surfaces. Molecules inside the water are happy because they are surrounded by friends (other water molecules). Molecules on the surface are unhappy because they are exposed to the air. To create more surface area, you have to do work against this attractive force. This "cost" is what we call surface tension.

The problem states:

$$dW = \mathcal{S} \, dA$$

This means: The work ($dW$) needed to increase the surface area by a tiny amount ($dA$) is equal to the surface tension times that area change.

---

### 2. The "Thought Experiment" (Virtual Displacement)

The problem asks us to consider a "quasistatic, adiabatic change" where the radius changes from $R \to R + \Delta R$.

Think of this as a **virtual displacement**. Imagine we grab the droplet and mechanically stretch it just a tiny bit so it gets slightly bigger.

-   If the system is in **equilibrium** (stable), the total mechanical work done by the forces acting on the system must balance out to zero.
    

We have two competing players here:

1.  **Pressure Forces:** The air inside pushes out, and the air outside pushes in. Since the drop is stable, $P_{\text{in}}$ must be usually higher than $P_{\text{um}}$ to hold the skin of the water up. This pressure difference tries to **expand** the drop.
    
2.  **Surface Tension:** The "skin" of the water wants to shrink to minimize its area. It tries to **compress** the drop.
    

For the drop to be stable, the work done by the pressure pushing out must exactly equal the energy cost of creating the new surface area.

---

### 3. The Math

Let's calculate the changes for a sphere when we increase the radius by a tiny amount $dR$ (or $\Delta R$).

A. Change in Surface Area ($dA$)

The surface area of a sphere is:

$$A = 4\pi R^2$$

If we change $R$ by $dR$, the change in area is the derivative:

$$dA = \frac{d}{dR}(4\pi R^2) \, dR = 8\pi R \, dR$$

B. Change in Volume ($dV$)

The volume of a sphere is:

$$V = \frac{4}{3}\pi R^3$$

If we change $R$ by $dR$, the change in volume is:

$$dV = \frac{d}{dR}\left(\frac{4}{3}\pi R^3\right) \, dR = 4\pi R^2 \, dR$$

---

### 4. Balancing the Work

Now, let's write down the energy balance.

Work done by Pressure ($dW_{\text{pressure}}$):

Work is Force $\times$ Distance, or Pressure $\times$ Volume change.

The pressure inside pushes the surface out ($P_{\text{in}}$ does positive work).

The pressure outside pushes the surface in ($P_{\text{um}}$ does negative work).

The net pressure doing work is $(P_{\text{in}} - P_{\text{um}})$.

$$dW_{\text{pressure}} = (P_{\text{in}} - P_{\text{um}}) \, dV$$

Work cost of Surface Tension ($dW_{\text{surface}}$):

As the prompt told us, the energy cost to stretch the surface is:

$$dW_{\text{surface}} = \mathcal{S} \, dA$$

Equilibrium Condition:

At equilibrium, the work done by the pressure expansion must equal the energy consumed by the surface tension. (Alternatively, the change in total free energy is zero).

$$(P_{\text{in}} - P_{\text{um}}) \, dV = \mathcal{S} \, dA$$

---

### 5. The Final Substitution

Now, substitute the expressions for $dV$ and $dA$ we calculated in Step 3 into our equilibrium equation:

$$(P_{\text{in}} - P_{\text{um}}) \cdot (4\pi R^2 \, dR) = \mathcal{S} \cdot (8\pi R \, dR)$$

Now, we act like true physicists and cancel out the terms that appear on both sides:

1.  Divide both sides by $dR$.
    
2.  Divide both sides by $4\pi R$.
    

On the left side:

$$(P_{\text{in}} - P_{\text{um}}) \cdot R$$

On the right side:

$$\mathcal{S} \cdot 2$$

Now, just isolate the pressure difference:

$$(P_{\text{in}} - P_{\text{um}}) = \frac{2\mathcal{S}}{R}$$

---

### Conclusion

And there you have it! We have derived equation (2) from your homework sheet.

**What does this actually mean physically?**

1.  **Pressure Jump:** There is always a pressure jump across a curved interface. The pressure inside a bubble or drop is always _higher_ than the outside.
    
2.  **The $1/R$ factor:** This is the most crucial part. The smaller the droplet (smaller $R$), the _larger_ the pressure difference.
    
    -   This is why it is very hard to blow up a balloon at the very beginning (small radius = huge pressure needed), but it gets easier as the balloon gets bigger!
        

Does that make sense to you? Would you like to try applying this to a soap bubble next? (Warning: Soap bubbles have _two_ surfaces, so there's a trick to it!)