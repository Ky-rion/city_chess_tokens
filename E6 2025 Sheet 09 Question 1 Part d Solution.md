

![[Pasted image 20260126135229.png]]

This is the "Grand Finale" of this problem! We are now going to take the "Push" from part **a)** and the "Friction" from part **c)** and combine them to explain real-world electricity.

Let's break down part **d)**.

### 1. The Goal (The Question)

**The Question (Image 1):**

> "Using the terms from a) and c), set up an equilibrium condition for current flow in a constant electric field."

**The Setup:**

We want to find the mathematical definition of "Steady State." This is the point where the current becomes constant (Ohm's Law applies), and the electrons stop accelerating, settling into a steady drift velocity.

---

### 2. The Physics: The Bathtub Analogy

To understand the equation in the solution, think of a bathtub:

1.  **The Tap (Part A):** You turn on the water. This is the **Electric Field** pumping momentum into the system. It wants to raise the water level (increase the electron speed) forever.
    
2.  **The Drain (Part C):** You open the drain. This is the **Scattering**. The more water there is (the faster the electrons go), the faster it drains out.
    
3.  **Equilibrium (Part D):** Eventually, the water level stops rising. Why? Because **Water In = Water Out**.
    

In physics terms, the **Net Change** in the wavevector $\langle \vec{k} \rangle$ must be **zero**.

---

### 3. The Math (The Solution)

Let's look at the professor's solution (Image 2):

$$\frac{d\langle \vec{k} \rangle}{dt} = \left. \frac{\partial \langle \vec{k} \rangle}{\partial t} \right|_{el} + \left. \frac{\partial \langle \vec{k} \rangle}{\partial t} \right|_{Streu} = 0$$

This equation is just adding up our two competing forces:

-   **Left Side ($\frac{d\langle \vec{k} \rangle}{dt}$):** The _total_ rate of change of the system.
    
-   **Middle Term 1 ($\dots|_{el}$):** The change caused by the **Electric Field** (from part a).
    
-   **Middle Term 2 ($\dots|_{Streu}$):** The change caused by **Scattering** (from part c). _Note: "Streu" is short for "Streuung," which is German for Scattering._
    
-   **Right Side ($= 0$):** This is the definition of **Equilibrium**. The total change must be zero for the current to be constant.
    

---

### 4. Let's Solve It (The "Hidden" Step)

The solution image stops at the equation setup, but to really understand it, we should plug in our answers from **a)** and **c)** to see what happens. This is likely what you would do next in class.

1.  **From Part A:** We found the field adds momentum at a rate of:
    
    $$-\frac{e\vec{E}}{\hbar}$$
    
2.  **From Part C:** We found scattering removes momentum at a rate of:
    
    $$-\frac{\delta\vec{k}}{\tau}$$
    
3.  **Combine them using the Equilibrium Equation:**
    
    $$\left( -\frac{e\vec{E}}{\hbar} \right) + \left( -\frac{\delta\vec{k}}{\tau} \right) = 0$$
    
4.  **Rearrange to solve for the shift $\delta\vec{k}$:**
    
    Move one term to the other side:
    
    $$-\frac{\delta\vec{k}}{\tau} = \frac{e\vec{E}}{\hbar}$$
    
    Multiply by $-\tau$:
    
    $$\delta\vec{k} = -\frac{e\tau}{\hbar}\vec{E}$$
    

### 5. Professor's Insight: Why is this result famous?

Look at that final derived equation: $\delta\vec{k} \propto \vec{E}$.

This proves **Ohm's Law**!

It tells us that the shift in electron velocity ($\delta\vec{k}$) is directly proportional to the Electric Field applied ($\vec{E}$).

-   Double the field $\rightarrow$ Double the electron speed $\rightarrow$ Double the current.
    

This is the microscopic proof of $V = IR$ (or more accurately $J = \sigma E$).

**Would you like me to help you derive the final expression for Conductivity ($\sigma$) from this, or move on to a new problem?**