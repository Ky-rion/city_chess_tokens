

![[Pasted image 20260125185646.png]]

Hello! Welcome to our solid-state physics lecture. I am delighted to be your guide. Don't worry if you've never seen this before—every physicist starts exactly where you are right now.

Today we are looking at **Phonons**, which is just a fancy word for "sound particles" or quantized vibrations in a solid.

Let’s break down **Task 3 (Aufgabe 3)** and the solution provided.

---

### 1. Translating the Problem (The Setup)

First, let's make sure we understand what the German text is telling us.

-   **System:** We have a "1-D Kette von Atomen" (a 1-dimensional chain of atoms). Imagine a long line of balls connected by springs.
    
-   **$L = 30\,\text{cm}$:** The total length of this chain.
    
-   **$v_S = 796\,\text{m/s}$:** The speed of sound in this material (how fast a vibration travels down the line).
    
-   **$D = 1.2 \times 10^{-4}\,\text{s}$:** This is the **Density of States**. This is the most critical variable here.
    
-   **$\omega_D = 8.38 \times 10^{12}\,\text{rad/s}$:** This is the **Debye Frequency**.
    

**The Goal:** Calculate $N$ (the total number of atoms in the chain).

---

### 2. The Core Concept: What is the "Debye Model"?

Before we look at the math, you need the intuition.

In a solid, atoms vibrate. However, they can't just vibrate at _any_ random frequency. Because the atoms are bound in a finite space (the chain), they can only vibrate at specific, allowed frequencies. These are called **modes**.

**The Golden Rule of Solid State Physics:**

> The total number of allowed vibrational modes is equal to the number of degrees of freedom in the system.

For a 1D chain of $N$ atoms, each atom can move back and forth (1 degree of freedom). Therefore, there are **$N$ total modes** of vibration.

The **Debye Model** is an approximation that assumes sound waves behave simply (like a continuous elastic string) up to a maximum cut-off frequency, called the **Debye Frequency ($\omega_D$)**. No vibrations can exist faster than this frequency.

---

### 3. Explaining the Solution Formula

Now, look at the red text in the second image. The professor solved it using this formula:

$$N = \int_{0}^{\omega_D} D \, d\omega$$

Let's decode this integral. This is the heart of the physics.

-   **$N$**: Total number of atoms (or total modes).
    
-   **$\omega$**: The frequency of vibration.
    
-   **$D$ (Density of States)**: This tells us _how many_ allowed vibrational modes exist at a specific frequency. You can think of $D$ as a "ticket counter." It tells you how many "tickets" (modes) correspond to a certain energy level.
    
-   **$\int_{0}^{\omega_D}$**: This is an integral (a sum). It means: "Sum up all the allowed modes starting from frequency 0 all the way up to the maximum limit, $\omega_D$."
    

**The Analogy:**

Imagine you are counting how many people are in a stadium.

-   $D$ is the number of seats per row.
    
-   $\omega$ is the row number.
    
-   To get the total people ($N$), you sum up the seats in every row until you reach the last row ($\omega_D$).
    

---

### 4. The Calculation Step-by-Step

In the solution image, you see this step:

$$N = D \cdot \omega_D$$

**Wait, what happened to the integral sign?**

This is a subtle but important mathematical point. The problem statement gave you $D$ as a constant number ($1.2 \times 10^{-4}\,\text{s}$). It is not a function of $\omega$ (it's not $D(\omega)$).

When you integrate a constant, you just multiply the constant by the range:

$$\int_{0}^{\omega_D} (\text{Constant}) \, d\omega = \text{Constant} \times (\omega_D - 0)$$

So the professor simply multiplied the Density of States by the Debye Frequency.

**Plugging in the numbers:**

$$N = (1.2 \times 10^{-4}\,\text{s}) \times (8.38 \times 10^{12}\,\text{rad/s})$$

-   _Note on units:_ The "s" in density and the "1/s" in frequency cancel out, leaving a dimensionless number (which counts the atoms).
    
-   $1.2 \times 8.38 \approx 10.05$
    
-   $10^{-4} \times 10^{12} = 10^8$
    
-   $10.05 \times 10^8 \approx 10^9$
    

**Final Answer:**

$$N = 10^9 \text{ atoms}$$

---

### 5. Professor's "Office Hour" Secret (Why did we ignore $L$ and $v_S$?)

You might have noticed the problem gave you the length ($L=30\text{cm}$) and the speed of sound ($v_S = 796 \text{m/s}$), and even a formula involving $\sqrt{K/m}$.

**Why didn't we use them?**

This is a classic physics trick! Sometimes, problems give you more information than you need for a specific method.

However, they are actually connected. In a 1D chain, the Density of States $D$ is theoretically calculated as:

$$D = \frac{L}{\pi v_S}$$

Let's check if the problem is consistent:

$$D = \frac{0.30\,\text{m}}{\pi \times 796\,\text{m/s}} \approx \frac{0.30}{2500} \approx 1.2 \times 10^{-4}\,\text{s}$$

Aha! The value for $D$ given in the text was actually derived from the Length and Speed. The professor gave you the "pre-calculated" value of $D$ to save you time. If they hadn't given you $D$, you would have had to calculate it yourself using $L$ and $v_S$.

**Next Step for you:**

Do you feel comfortable with how the integral turned into a simple multiplication? If so, we can move on to looking at how the energy of these atoms behaves, or we can look at the next part of the problem!