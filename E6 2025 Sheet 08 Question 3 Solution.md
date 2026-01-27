

![[Pasted image 20260125190202.png]]
![[Pasted image 20260125190209.png]]

Hello! Welcome to our Solid State Physics session. I am delighted to be your guide. Don't worry if you've never seen this before—every physicist started exactly where you are right now.

Today we are looking at the behavior of electrons in a metal. Specifically, we are looking at the **Fermi Energy ($E_F$)** and how it relates to temperature.

Let's break down the problem statement, the physical concepts, and then walk through your professor's solution step-by-step.

---

### 1. The Problem Statement

First, let's translate the German text in the first image to make sure we know exactly what is being asked.

**German:**

_"Die Annahme, dass $\mu \approx E_F$ gilt eigentlich nur für niedrige Temperaturen. Bestimmen Sie mit der Sommerfeld-Entwicklung (aus der Vorlesung), für welche maximale Temperatur, der Fehler noch unter 1% bleibt. $E_F = 3\text{eV}$"_

**English Translation:**

_"The assumption that chemical potential ($\mu$) is approximately equal to the Fermi Energy ($E_F$) actually only holds for low temperatures. Using the Sommerfeld expansion (from the lecture), determine the maximum temperature for which the error remains below 1%. Given: $E_F = 3\text{eV}$."_

---

### 2. The Physical Concept: The "Sea" of Electrons

Imagine a metal as a box. Inside this box, you have electrons filling up energy levels.

-   **At Absolute Zero ($T=0\text{ K}$):** The electrons fill the lowest energy states first, stacking up until they hit a maximum energy level. This top level is called the **Fermi Energy ($E_F$)**. At this temperature, the "chemical potential" ($\mu$) is exactly equal to $E_F$.
    
-   **At Higher Temperatures ($T > 0\text{ K}$):** As you heat the metal, some electrons near the top get excited and jump to slightly higher energy levels. Because the distribution of electrons spreads out, the chemical potential $\mu$ actually shifts slightly _downwards_.
    

**The Core Question:**

In many physics problems, we lazy physicists just say $\mu \approx E_F$ because the shift is tiny. This problem is asking: **"How hot do we have to get before this laziness becomes a 1% error?"**

---

### 3. The Solution Walkthrough

Now, let's look at the second image (the solution) and break down the math.

#### Step 1: The Sommerfeld Expansion

The solution starts with a formula labeled _"Aus der Vorlesung ist bekannt, dass"_ (It is known from the lecture that):

$$\mu(T) = E_F \left[ 1 - \frac{\pi^2}{12} \left( \frac{T}{T_F} \right)^2 \right]$$

This is the **Sommerfeld Expansion**. It is a mathematical approximation that tells us how $\mu$ changes as Temperature ($T$) increases.

-   $\mu(T)$: Chemical potential at temperature $T$.
    
-   $E_F$: Fermi Energy (constant, $3\text{eV}$).
    
-   $T$: The actual temperature.
    
-   $T_F$: The "Fermi Temperature." This is just a way of writing energy in units of temperature ($E_F = k_B T_F$).
    

#### Step 2: Setting the Error Limit

The problem asks for the point where the error is **under 1%**.

This means we want the value of $\mu$ to be at least 99% of the value of $E_F$.

Mathematically, we look at the term inside the brackets $[\dots]$. If $\mu$ is 99% of $E_F$, then the stuff inside the brackets must equal $0.99$.

$$\left[ 1 - \frac{\pi^2}{12} \left( \frac{T}{T_F} \right)^2 \right] = 0.99$$

#### Step 3: Isolating the Temperature

Now, we do some algebra to find the temperature term.

Subtract $1$ from both sides (or move the terms around):

$$\frac{\pi^2}{12} \left( \frac{T}{T_F} \right)^2 = 1 - 0.99 = 0.01$$

This equation tells us that the "correction term" (the part that makes $\mu$ different from $E_F$) is now 1% (or 0.01).

Now, we solve for the ratio $\frac{T}{T_F}$:

$$\left( \frac{T}{T_F} \right)^2 = \frac{0.01 \cdot 12}{\pi^2}$$

Take the square root of both sides:

$$\frac{T}{T_F} = \sqrt{\frac{0.12}{\pi^2}}$$

#### Step 4: Converting to Kelvin

We want to find $T$ (in Kelvin). We know that $T = T_F \cdot (\text{the number we just found})$.

But wait! We weren't given $T_F$ directly. We were given $E_F = 3\text{eV}$.

We need to use the fundamental connection between energy and temperature, which involves the **Boltzmann constant ($k_B$)**:

$$E_F = k_B T_F \quad \Rightarrow \quad T_F = \frac{E_F}{k_B}$$

So, substituting this into our equation for $T$:

$$T = \frac{E_F}{k_B} \cdot \sqrt{\frac{0.12}{\pi^2}}$$

Now we plug in the numbers (this is the final line in your image):

-   $E_F = 3\text{eV}$
    
-   $k_B \approx 8.617 \times 10^{-5} \text{ eV/K}$
    
-   $\pi \approx 3.14159$
    

$$T \approx \frac{3}{8.617 \times 10^{-5}} \cdot 0.110$$

$$T \approx 34,814\text{ K} \cdot 0.110$$

$$T \approx 3830\text{ K}$$

The solution in the image rounds this to **$3800\text{ K}$**.

---

### Professor's Summary (The "So What?")

We found that you have to heat this metal up to **$3800\text{ Kelvin}$** before the error in assuming $\mu \approx E_F$ reaches even **$1\%$**.

To put that in perspective:

-   Room temperature is roughly **$300\text{ K}$**.
    
-   Iron melts at roughly **$1800\text{ K}$**.
    

**The Lesson:** For almost all solid-state physics problems involving metals on Earth, the temperature is so "low" compared to the Fermi Temperature that we can safely assume $\mu = E_F$ without worrying about errors. The electron gas is "degenerate," meaning quantum mechanics dominates over thermal energy.

**Would you like me to clarify how the Boltzmann constant works, or explain more about what the "Fermi Temperature" actually feels like physically?**