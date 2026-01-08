

Hello there! I am delighted to welcome you to the world of low-temperature thermodynamics. It is a fascinating place where intuition often has to be rebuilt, but the mathematics is incredibly elegant.

You have asked about **Problem 1: Absolute Zero**. This problem essentially asks us to prove a consequence of the Third Law of Thermodynamics: that you cannot actually reach absolute zero temperature ($T=0$) through a finite number of physical processes.

Let's break down the professor's solution step-by-step. Don't worry about the wall of calculus; we will decode it together.

---

### Part (a): The Ratio of Expansion to Heat Capacity

The Goal:

We want to look at the ratio $\frac{V\beta}{C_P}$ as temperature approaches zero.

-   $C_P$ is the heat capacity (how much energy it takes to raise the temperature).
    
-   $\beta$ is the thermal expansion coefficient (how much the volume changes when you heat it).
    

Step 1: Connecting Volume and Entropy (Maxwell Relations)

The first hurdle is that $\beta$ involves volume ($V$), but $C_P$ involves entropy ($S$). We need a bridge between them.

The professor uses the Gibbs Free Energy ($G$) to build this bridge.

$$dG = -SdT + VdP$$

Because $dG$ is an exact differential, the mixed partial derivatives must be equal. This gives us a famous Maxwell Relation:

$$\left(\frac{\partial V}{\partial T}\right)_P = -\left(\frac{\partial S}{\partial P}\right)_T$$

This is a powerful trick! It allows us to calculate how volume changes with temperature (left side) by looking at how entropy changes with pressure (right side).

Step 2: Calculating Entropy from Heat Capacity

We don't know $S$ directly, but we do know $C_P$. The definition of heat capacity is related to the change in entropy:

$$C_P = T \left(\frac{\partial S}{\partial T}\right)_P$$

We can rearrange this to solve for entropy by integrating:

$$S(T) = \int_0^T \frac{C_P(T')}{T'} dT'$$

Note: We assume the Third Law holds, so $S(0) = 0$.

Step 3: The Mathematical Approximation

The problem gives us an approximation for $C_P$ near absolute zero:

$$C_P \approx T^x (a + bT + cT^2)$$

where $a, b, c$ depend on pressure $P$.

When we integrate $\frac{C_P}{T}$, we treat $P$ as a constant. The leading term (the biggest one near zero) is the $T^x$ term.

$$\int_0^T \frac{a (T')^x}{T'} dT' = \int_0^T a (T')^{x-1} dT' = \frac{a}{x} T^x$$

The solution writes out the full integral for all terms, but the $T^x$ term is the "dominant" one we care about for the limit.

Step 4: Differentiating with respect to Pressure

Now, remember our Maxwell relation from Step 1? We need $-\left(\frac{\partial S}{\partial P}\right)_T$.

Since the coefficients $a, b, c$ depend on pressure ($P$), we have to take the derivative of our integral result with respect to $P$:

$$\left(\frac{\partial S}{\partial P}\right)_T = \frac{1}{x} (\partial_P a) T^x + \dots (\text{higher order terms})$$

So, the term $V\beta$, which equals $-\left(\frac{\partial S}{\partial P}\right)_T$, is roughly:

$$V\beta \approx -\frac{1}{x} (\partial_P a) T^x$$

Step 5: Taking the Limit

Finally, we look at the fraction the question asked for:

$$\frac{V\beta}{C_P} \approx \frac{-\frac{1}{x} (\partial_P a) T^x}{a T^x}$$

Notice that $T^x$ cancels out! We are left with:

$$\lim_{T \to 0} \frac{V\beta}{C_P} = -\frac{1}{x a} (\frac{\partial a}{\partial P}) = -\frac{1}{x} \frac{\partial \ln a}{\partial P}$$

This result is just a number (a finite constant). We have successfully proven Part (a).

---

### Part (b): Can We Reach Absolute Zero?

The Goal:

We want to calculate $\lim_{T \to 0} \left(\frac{\partial T}{\partial P}\right)_S$.

This derivative represents adiabatic cooling. It asks: "If I change the pressure ($P$) while keeping the system insulated (constant entropy $S$), how much does the temperature ($T$) change?"

Step 1: The Total Differential of Entropy

We start by writing the total change in entropy $dS$ as a function of $P$ and $T$:

$$dS = \left(\frac{\partial S}{\partial P}\right)_T dP + \left(\frac{\partial S}{\partial T}\right)_P dT$$

Step 2: Substituting Physical Quantities

We replace the partial derivatives with the physical quantities we know:

1.  From Maxwell (Part a): $\left(\frac{\partial S}{\partial P}\right)_T = -V\beta$.
    
2.  From definition of heat capacity: $\left(\frac{\partial S}{\partial T}\right)_P = \frac{C_P}{T}$.
    

So the equation becomes:

$$dS = -V\beta dP + \frac{C_P}{T} dT$$

Step 3: Setting $dS = 0$ (Adiabatic Process)

We want to see what happens in an isentropic (adiabatic) process, so we set $dS = 0$ and solve for the slope $\frac{dT}{dP}$:

$$0 = -V\beta dP + \frac{C_P}{T} dT$$

$$\frac{C_P}{T} dT = V\beta dP$$

$$\left(\frac{\partial T}{\partial P}\right)_S = T \cdot \frac{V\beta}{C_P}$$

Step 4: The Final Conclusion

Now we take the limit as $T \to 0$.

Look at the terms on the right side:

1.  We have the factor $T$, which obviously goes to $0$.
    
2.  We have the fraction $\frac{V\beta}{C_P}$. In Part (a), we proved this fraction goes to a **finite constant**.
    

Therefore:

$$\lim_{T \to 0} \left(\frac{\partial T}{\partial P}\right)_S = 0 \cdot (\text{constant}) = 0$$

What does this mean physically?

This is the "Unattainability Principle."

Imagine a graph with Pressure on the x-axis and Temperature on the y-axis. You are trying to cool the gas by changing pressure.

-   Usually, changing pressure changes temperature (the slope is non-zero).
    
-   However, as you get closer and closer to $T=0$, the "cooling power" of changing pressure vanishes (the slope becomes flat/zero).
    

Because the slope flattens out, you would need an infinite number of pressure changes to actually reach $T=0$. Thus, **absolute zero is unattainable.**

---

### Summary for your notes

-   **Part (a)** used a Maxwell relation to link volume expansion to the pressure dependence of entropy. It showed that $\beta$ and $C_P$ scale similarly near zero.
    
-   **Part (b)** used those results to show that the efficiency of cooling by pressure change drops to zero as $T \to 0$.
    

**Would you like me to explain the next problem (Problem 2), where we apply these concepts to a "Real Gas"?**