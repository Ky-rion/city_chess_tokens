

This is the grand finale! This question ties everything we've done together. It uses the "invariance" from (b) and the 4-momentum from (c) to derive one of the most famous and useful equations in all of physics.

Let's do this one just as carefully as the others.

### 1. The Core Principle (from part b)

In part (b), we discovered something amazing: when you "square" a 4-vector, the result is a **Lorentz Invariant**. This means the resulting number is **the same in all reference frames**.

-   For the position 4-vector $x^\mu$, we found $s^2 = (ct)^2 - x^2 - y^2 - z^2$. This "spacetime interval" is the same for all observers.
    
-   In part (c), we defined the 4-momentum $p^\mu = (E/c, \vec{p})$. This is also a 4-vector.
    

Therefore, the exact same logic must apply: the "square" of the 4-momentum, $p \cdot p$, must also be a **Lorentz Invariant**. Its value must be identical in the lab frame and in the particle's rest frame.

This gives us our strategy:

1.  Calculate $p \cdot p$ in the **lab frame**.
    
2.  Calculate $p \cdot p$ in the **rest frame**.
    
3.  Set them equal to each other and see what it means.
    

---

### 2. Calculating $p \cdot p$ in the Lab Frame

The "square" of a 4-vector $A^\mu = (A^0, \vec{A})$ is $(A^0)^2 - |\vec{A}|^2$.

Our 4-momentum is $p^\mu = (E/c, \vec{p})$.

-   The time-component ($p^0$) is $E/c$.
    
-   The space-components ($\vec{p}$) are just $\vec{p}$, with a magnitude $|\vec{p}| = p$.
    

So, the square of the 4-momentum in the lab frame is:

$(p \cdot p)_{\text{lab}} = (p^0)^2 - |\vec{p}|^2$

$(p \cdot p)_{\text{lab}} = (E/c)^2 - p^2$

This is our expression in the lab frame, where the particle has energy $E$ and momentum $p$.

---

### 3. Calculating $p \cdot p$ in the Rest Frame

Now, let's consider the particle in its **own rest frame**. This is the frame where the particle is not moving.

-   **Velocity:** $\vec{v} = 0$.
    
-   **Momentum ($\vec{p}_{\text{rest}}$):** Since $\vec{p} = \gamma m\vec{v}$, if $\vec{v}=0$, then **$\vec{p}_{\text{rest}} = 0$**.
    
-   **Energy ($E_{\text{rest}}$):** We need to find the energy. Let's look at the definitions:
    
    -   $\beta = v/c = 0$
        
    -   $\gamma = 1/\sqrt{1 - \beta^2} = 1/\sqrt{1 - 0} = 1$
        
    -   $E = \gamma mc^2 = (1)mc^2 =$ **$mc^2$**
        

So, in its _own rest frame_, the particle has $E_{\text{rest}} = mc^2$ (its rest energy) and $\vec{p}_{\text{rest}} = 0$.

Now, let's write the 4-momentum in the rest frame:

$p^\mu_{\text{rest}} = (E_{\text{rest}}/c, \vec{p}_{\text{rest}}) = (mc^2/c, \vec{0}) = (mc, 0, 0, 0)$

Let's "square" this 4-momentum:

$(p \cdot p)_{\text{rest}} = (p^0_{\text{rest}})^2 - |\vec{p}_{\text{rest}}|^2$

$(p \cdot p)_{\text{rest}} = (mc)^2 - 0^2$

$(p \cdot p)_{\text{rest}} = m^2 c^2$

---

### 4. Comparing the Results (The Expression for $E$)

The invariance principle tells us that these two quantities must be equal:

$(p \cdot p)_{\text{lab}} = (p \cdot p)_{\text{rest}}$

Substitute what we found in steps 2 and 3:

$(E/c)^2 - p^2 = m^2 c^2$

This is the comparison. Now, let's follow the hint and find an expression for $E$. We just need to rearrange this equation:

1.  Add $p^2$ to both sides:
    
    $(E/c)^2 = m^2 c^2 + p^2$
    
2.  Multiply the whole equation by $c^2$:
    
    $E^2 = (m^2 c^2)c^2 + (p^2)c^2$
    
    $E^2 = m^2 c^4 + p^2 c^2$
    

This is the famous **Energy-Momentum Relation**. It's often written as $E^2 = (mc^2)^2 + (pc)^2$ to make the units more obvious.

---

### 5. What is the Significance of Your Result?

This result is profoundly important for several reasons:

1.  **It unifies Energy, Mass, and Momentum:** This equation is the complete relationship connecting a particle's total energy ($E$), its momentum ($p$), and its fundamental, invariant mass ($m$).
    
2.  **It contains $E=mc^2$ as a special case:** What if the particle is at rest (as in, we are in its rest frame)?
    
    -   If the particle is at rest, its momentum $p=0$.
        
    -   The equation becomes: $E^2 = (mc^2)^2 + 0$
        
    -   $E^2 = (mc^2)^2 \implies E = mc^2$
        
    -   This shows that the famous $E=mc^2$ equation describes the **rest energy** of a particle—the energy it has just by existing.
        
3.  **It works for massless particles:** What about a particle of light (a photon), which has $m=0$?
    
    -   The equation becomes: $E^2 = 0 + (pc)^2$
        
    -   $E^2 = (pc)^2 \implies E = pc$
        
    -   This is the correct relationship for light!
        
4.  **It defines Invariant Mass:** The deepest significance is that the quantity $(E/c)^2 - p^2 = m^2 c^2$ is an **invariant**. Since $c$ is a constant, this means **$m^2$** (and thus $m$, the rest mass) is a fundamental property of the particle that **all observers agree on**. This is why $m$ is called the **invariant mass**. Observers will disagree on $E$ (total energy) and $\vec{p}$ (momentum), but they will _all_ calculate the same value for $m$ using their measured $E$ and $\vec{p}$.
    

In short, "squaring" the 4-momentum reveals the particle's invariant mass.

You've just walked through the logical core of special relativity. Well done! Do you have any more questions about this, or are you ready to move on?