

![[Pasted image 20260128115942.png]]

Hello! Welcome to our first session on particle physics. I am delighted to be your guide. Don't worry if this looks intimidating at first glance—particle physics is essentially just counting energy and momentum, but with some very fast-moving objects!

We are looking at a classic experiment performed at **HERA** (the Hadron-Electron Ring Accelerator) in Germany. This was a unique machine because it collided **electrons** (light particles) with **protons** (heavy particles).

Let's break down the solution for **Part (a)** step-by-step.

---

### 1. The Concept of Center-of-Mass Energy ($\sqrt{s}$)

In particle physics, the most important number we care about is the **Center-of-Mass (CoM) energy**. We usually denote the square of this energy by the Mandelstam variable $s$. So, the energy itself is $\sqrt{s}$.

Think of $\sqrt{s}$ as the "useful" energy available in a collision to create new particles or probe the inside of the proton.

The general formula for $s$ when two particles collide is based on their **four-momenta** (a way of combining energy and momentum into one vector). The exact formula shown in the solution is:

$$s = (p_1 + p_2)^2 = m_1^2 + m_2^2 + 2(E_1 E_2 - \vec{p}_1 \cdot \vec{p}_2)$$

Where:

-   $m$ is mass.
    
-   $E$ is energy.
    
-   $\vec{p}$ is the momentum vector.
    

### 2. The Collider Scenario (Head-on)

In the HERA collider, the electron and proton fly toward each other. This is a **head-on collision**.

**Step A: Can we neglect masses?**

The problem asks if we can neglect masses. Let's look at the numbers:

-   Electron Energy: $E_e = 27.6 \text{ GeV}$ vs. Electron Mass: $m_e \approx 0.0005 \text{ GeV}$
    
-   Proton Energy: $E_p = 920 \text{ GeV}$ vs. Proton Mass: $m_p \approx 0.938 \text{ GeV}$
    

Because the energies are **massive** compared to the rest masses ($E \gg m$), the particles are moving at essentially the speed of light ($c$). In this "ultra-relativistic" limit, momentum is roughly equal to energy ($|\vec{p}| \approx E/c$).

-   **Verdict:** Yes, we can safely ignore the masses to make the math easier. They are tiny crumbs compared to the whole cake.
    

**Step B: The Approximation**

Since it is a head-on collision, the momentum vectors point in opposite directions. When you subtract a negative vector (in the dot product $\vec{p}_1 \cdot \vec{p}_2$), it adds up.

If we drop the mass terms ($m \approx 0$) and assume head-on collision, the big formula simplifies beautifully to the one in your solution:

$$s \approx 4 E_e E_p$$

**Step C: The Calculation**

Now we just plug in the numbers provided in the problem:

$$s \approx 4 \cdot (27.6 \text{ GeV}) \cdot (920 \text{ GeV})$$

$$s \approx 101,568 \text{ GeV}^2$$

To get the Center-of-Mass energy, we take the square root:

$$\sqrt{s} = \sqrt{101,568} \approx \mathbf{319 \text{ GeV}}$$

This matches the solution! This means there is 319 GeV of pure energy available in the collision to do physics.

---

### 3. The "Fixed Target" Scenario

The second part of the question is very clever. It asks: **"What if the proton wasn't moving?"**

Imagine we kept the proton stationary (like a block of ice) and fired the electron beam at it. How much energy would the electron beam need to create that same $319 \text{ GeV}$ collision?

**Step A: The Physics Change**

When you hit a stationary target, a lot of the incoming energy is "wasted" just pushing the wreckage forward (conserving momentum) rather than breaking the particles apart. This makes fixed-target experiments much less efficient energetically.

**Step B: The Formula**

We go back to our master equation:

$$s = m_e^2 + m_p^2 + 2(E_e E_p - \vec{p}_e \cdot \vec{p}_p)$$

Since the proton is stationary:

1.  Its momentum is zero: $\vec{p}_p = 0$.
    
2.  Its energy is just its rest mass: $E_p = m_p$.
    

We still ignore the electron's tiny mass ($m_e \approx 0$). The formula simplifies to:

$$s \approx 2 E_{\text{beam}} m_p$$

**Step C: Solving for the Beam Energy**

We want $s$ to be the same as before ($s \approx 101,568 \text{ GeV}^2$). We know the proton mass is roughly $0.938 \text{ GeV}$. We rearrange to solve for the required electron beam energy ($E_e$):

$$E_e \approx \frac{s}{2 m_p}$$

$$E_e \approx \frac{101,568}{2 \cdot 0.938}$$

$$E_e \approx \mathbf{54,140 \text{ GeV}} \approx \mathbf{54 \text{ TeV}}$$

### Summary and Professor's Insight

Look at the difference!

-   **Collider:** You only need an electron beam of **27.6 GeV**.
    
-   **Fixed Target:** You would need an electron beam of **54,000 GeV**.
    

This explains **why** we build colliders (like the Large Hadron Collider or HERA). Colliding two beams head-on is vastly more efficient at generating high collision energies than shooting a beam at a stationary rock. To get the same result with a stationary proton, you'd need an accelerator thousands of times more powerful than what exists today!

---

**Would you like me to move on to part (b) of the question, or would you like to clarify anything about the "Fixed Target" vs. "Collider" concept first?**