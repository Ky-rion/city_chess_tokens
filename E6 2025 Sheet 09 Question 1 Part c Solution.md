

![[Pasted image 20260126135219.png]]

Welcome back to class! We are moving perfectly through the logical steps of the **Drude-Sommerfeld model**.

In part **a)** we looked at the "Push" (the Field).

In part **b)** we conceptually discussed the "Friction" (Scattering).

Now in part **c)**, we are going to model that friction mathematically by seeing what happens when we **stop pushing**.

This is often called the **Relaxation Time Approximation**, and it is one of the most useful tools in all of physics.

---

### 1. The Scenario (The Question)

**The Question (Image 1):**

> "Now the electric field is switched off. The Fermi sphere shifts back to the initial state with [a decay of] $\delta\vec{k} \propto e^{-t/\tau}$. Find an expression for the time rate of change of the mean reciprocal vector $\frac{\partial \langle \vec{k} \rangle}{\partial t} |_{relax}$ here as well."

**The Setup:**

Imagine you are stretching a rubber band.

-   **Part A** was you pulling it (applying force).
    
-   **Part C** is you letting go. The rubber band snaps back to its original shape.
    

We are told the return journey follows an **exponential decay**:

$$\delta\vec{k}(t) = \vec{\delta}_0 \cdot e^{-t/\tau}$$

-   $\delta\vec{k}$: The displacement (how far "off-center" the Fermi sphere is).
    
-   $\vec{\delta}_0$: The starting displacement at the moment you switched off the field.
    
-   $\tau$ (Tau): The **Relaxation Time**. This represents the average time an electron travels before it hits something (scatters).
    

---

### 2. The Derivation (The Math)

Let's walk through the solution in Image 2 line-by-line. It uses a clever calculus trick.

**Step 1: Define the Total State**

The current average wavevector $\langle \vec{k} \rangle(t)$ is made of two parts:

1.  The equilibrium position $\langle \vec{k} \rangle^0$ (usually zero).
    
2.  The extra displacement $\delta\vec{k}(t)$.
    

$$\langle \vec{k} \rangle(t) = \langle \vec{k} \rangle^0 + \delta\vec{k}(t)$$

**Step 2: Take the Derivative**

We want to know how fast the state changes ($\frac{\partial}{\partial t}$). So we differentiate the equation above:

$$\frac{\partial \langle \vec{k} \rangle}{\partial t} = \frac{\partial \langle \vec{k} \rangle^0}{\partial t} + \frac{\partial \delta\vec{k}}{\partial t}$$

-   **First term:** $\frac{\partial \langle \vec{k} \rangle^0}{\partial t} = 0$. Why? Because the equilibrium state (the metal sitting on a table with no power) never changes. It's constant.
    
-   **Second term:** This is the one we need to calculate.
    

**Step 3: Differentiate the Exponential**

We know $\delta\vec{k}(t) = \vec{\delta}_0 \cdot e^{-t/\tau}$. Let's take the time derivative:

$$\frac{\partial}{\partial t} (\vec{\delta}_0 \cdot e^{-t/\tau})$$

Using the chain rule (derivative of $e^{at}$ is $a \cdot e^{at}$):

$$= \vec{\delta}_0 \cdot \left( -\frac{1}{\tau} \right) \cdot e^{-t/\tau}$$

**Step 4: The Substitution Trick**

Rearrange that result slightly:

$$= -\frac{1}{\tau} \cdot \underbrace{(\vec{\delta}_0 \cdot e^{-t/\tau})}_{\text{Hey, this is just } \delta\vec{k}!}$$

So, we can replace the exponential part back with $\delta\vec{k}$:

$$\frac{\partial \delta\vec{k}}{\partial t} = -\frac{\delta\vec{k}}{\tau}$$

**The Final Result:**

$$\frac{\partial \langle \vec{k} \rangle}{\partial t}|_{relax} = -\frac{\delta\vec{k}}{\tau}$$

---

### 3. Professor's Insight: What does this mean?

This simple equation:

$$\text{Change in k} = -\frac{\text{Current Displacement}}{\tau}$$

tells us something profound about nature. It says: **"The further you are from home, the faster you rush back."**

-   If the Fermi sphere is shifted way off to the right (large $\delta\vec{k}$), the scattering is intense, and it moves back quickly.
    
-   As it gets closer to the center (small $\delta\vec{k}$), the change slows down.
    
-   Eventually, it gently settles into equilibrium.
    

**Why is this important?**

Because now we have the two halves of the puzzle!

1.  **Part A** gave us the rate of change due to the **Field** ($\sim \vec{E}$).
    
2.  **Part C** gave us the rate of change due to **Collisions** ($\sim -\delta\vec{k}/\tau$).
    

In the next step (which usually follows in these problem sets), we will combine these to find the **Steady State**, where the "Push" equals the "Relaxation."

Would you like to put these pieces together now to derive the famous formula for conductivity?