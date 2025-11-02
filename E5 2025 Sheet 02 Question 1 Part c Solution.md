

This is a great question that builds perfectly on our last one! We're going to build another 4-vector, the **4-momentum**, and see that it beautifully packages the concepts of energy and momentum together, just like the position 4-vector packaged space and time.

Let's follow the logic.

### 1. The Analogy to Classical Mechanics

In classical physics, momentum is a 3-vector, $\vec{p}$, defined as:

$\vec{p} = m \vec{v}$

where $m$ is the mass and $\vec{v}$ is the 3-velocity, $\vec{v} = \frac{d\vec{x}}{dt}$.

We want to create a 4-momentum ($p^\mu$) in relativity. The simplest analogy would be:

$p^\mu = (\text{mass}) \times (\text{4-velocity})$

But we have to be _very_ careful. As we learned in the last question, quantities in relativity can be tricky.

-   **Mass ($m$):** We must use a quantity that all observers agree on. This is the **rest mass** (or invariant mass) of the particle, $m$.
    
-   **4-Velocity ($u^\mu$):** We can't just use the 3-velocity. We need to define a 4-velocity, $u^\mu$.
    

So, our definition is:

$p^\mu = m u^\mu$

---

### 2. Answering the Hint: Defining the 4-Velocity ($u^\mu$)

This is the most important step. How do we define 4-velocity?

-   Our position 4-vector is $x^\mu = (ct, x, y, z)$.
    
-   A velocity is a derivative of position with respect to time (e.g., $\frac{dx}{d(\text{time})}$).
    

**The Hint: "Which time do we have to use?"**

We have two "times":

1.  **Lab Time ($t$):** This is the time measured by our clock in the lab. We proved in (b) that this is **relative**. Different observers measure different $t$'s. We cannot build a fundamental 4-vector from a relative quantity.
    
2.  **Proper Time ($\tau$):** This is the time measured by the particle in its _own_ rest frame (as in, the muon's watch). As we discussed in (a), this is an **invariant**. All observers, no matter how fast they are moving, can look at the particle's clock and agree on the time it reads.
    

To build a valid 4-vector, we **must** differentiate with respect to an invariant scalar. Therefore, we must use the **proper time, $\tau$**.

The 4-velocity is defined as:

$u^\mu = \frac{dx^\mu}{d\tau} = \frac{d}{d\tau}(ct, x, y, z) = (c\frac{dt}{d\tau}, \frac{dx}{d\tau}, \frac{dy}{d\tau}, \frac{dz}{d\tau})$

---

### 3. Calculating the Components of 4-Velocity

Now we just need to figure out what those derivatives are. We use two tools:

1.  The time dilation formula from (a): $dt = \gamma d\tau$, which rearranges to **$\frac{dt}{d\tau} = \gamma$**.
    
2.  The chain rule from calculus: e.g., $\frac{dx}{d\tau} = \frac{dx}{dt} \frac{dt}{d\tau}$.
    

Let's find each component of $u^\mu$:

-   0-component ($u^0$):
    
    $u^0 = c \frac{dt}{d\tau} = c\gamma$
    
-   1-component ($u^1$):
    
    $u^1 = \frac{dx}{d\tau} = (\frac{dx}{dt}) (\frac{dt}{d\tau})$
    
    We know $\frac{dx}{dt}$ is just the ordinary velocity in the x-direction, $v_x$.
    
    So, $u^1 = (v_x) (\gamma) = \gamma v_x$
    
-   2 & 3-components ($u^2, u^3$):
    
    Similarly, $u^2 = \gamma v_y$ and $u^3 = \gamma v_z$.
    

We can group the three spatial components into the ordinary 3-velocity vector $\vec{v} = (v_x, v_y, v_z)$.

So, the 4-velocity $u^\mu$ is:

$u^\mu = (\gamma c, \gamma\vec{v})$

---

### 4. Writing the 4-Momentum ($p^\mu$)

Now we go back to our definition $p^\mu = m u^\mu$ and plug this in:

$p^\mu = m (\gamma c, \gamma\vec{v})$

$p^\mu = (\gamma mc, \gamma m\vec{v})$

This is the 4-momentum.

---

### 5. Final Answer: In Terms of $E$ and $\vec{p}$

The question asks for the final answer in terms of the relativistic energy ($E$) and momentum ($\vec{p}$). Your problem gives us these definitions:

-   Relativistic Energy: **$E = \gamma mc^2$**
    
-   Relativistic 3-Momentum: **$\vec{p} = \vec{\beta}\gamma mc = (\frac{\vec{v}}{c})\gamma mc = \gamma m\vec{v}$**
    

Let's look at the components of our 4-momentum $p^\mu = (\gamma mc, \gamma m\vec{v})$ and substitute these definitions.

-   Look at the 0-component ($p^0$):
    
    $p^0 = \gamma mc$
    
    How does this relate to $E = \gamma mc^2$?
    
    If you divide $E$ by $c$, you get: $E/c = (\gamma mc^2) / c = \gamma mc$.
    
    This is a perfect match! So, $p^0 = E/c$.
    
-   Look at the spatial components ($p^1, p^2, p^3$):
    
    $(p^1, p^2, p^3) = \gamma m\vec{v}$
    
    This is exactly the definition of the relativistic 3-momentum, $\vec{p}$.
    

By substituting these in, we get the final, elegant answer:

$p^\mu = (p^0, p^1, p^2, p^3) = (E/c, p_x, p_y, p_z)$

Or, more compactly:

> **$p^\mu = (E/c, \vec{p})$**

Just as a Lorentz boost mixes space and time, it also mixes energy and momentum. They are two sides of the same coin: the 4-momentum.

Are you ready for the next part?