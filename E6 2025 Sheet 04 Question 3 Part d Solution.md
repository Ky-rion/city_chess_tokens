

![[Pasted image 20260125184027.png]]
![[Pasted image 20260125184034.png]]

We are now at the finish line! This is the part where all that setup pays off and we get the famous "Arrhenius Equation" for defects.

This step is pure algebra, but there is a **huge trap** in the professor's solution slide (Image 5) that might confuse you. I will point it out so you don't get stuck.

Let's derive the final answer step-by-step.

---

### The Goal

We want to find the **equilibrium concentration of defects** ($n/N$).

Basically: "If I heat this crystal to 500 Kelvin, what percentage of atoms will be missing?"

### The Derivation

#### Step 1: Set up the Gibbs Free Energy Equation

From Part (b), we know:

$$G(n) = H(n) - T \cdot S(n)$$

-   **Enthalpy:** $H(n) = n \cdot \Delta H_S$ (Total energy cost for $n$ defects).
    
-   **Entropy:** From Part (c), $S(n) = k_B \cdot \ln \left( \binom{N}{n}^2 \right) = 2 k_B \cdot \ln \binom{N}{n}$.
    
    _(Note: We brought the power of 2 down to the front using log rules: $\ln(x^2) = 2\ln x$)_.
    

So, our full equation is:

$$G(n) = n \cdot \Delta H_S - 2 k_B T \cdot \ln \binom{N}{n}$$

#### Step 2: Minimize the Energy (The Derivative)

Nature is lazy. It wants to be at the bottom of the energy valley. To find the minimum, we take the derivative with respect to $n$ and set it to zero:

$$\frac{dG}{dn} = 0$$

Let's differentiate our $G(n)$ equation term by term:

1.  **First term:** The derivative of $n \cdot \Delta H_S$ is just **$\Delta H_S$**.
    
2.  **Second term:** We need the derivative of that messy log term. Luckily, the problem statement (Image 4, Equation 3) gives us a cheat code:
    
    $$\frac{d}{dn} \ln \binom{N}{n} \approx \ln\left(\frac{N}{n}\right)$$
    

So, plugging that "cheat code" into our derivative:

$$\frac{dG}{dn} = \Delta H_S - 2 k_B T \cdot \ln\left(\frac{N}{n}\right) = 0$$

> **⚠️ WARNING: TYPO ALERT ⚠️**
> 
> Look at the professor's solution in **Image 5 (Equation 20 & 21)**.
> 
> Do you see how the **$T$ (Temperature)** is missing? And the signs are weird?
> 
> -   **Professor's Eq 21:** $\Delta H_S + 2k_B \cdot \ln(\frac{N}{n}) \approx 0$
>     
> 
> This line in the image is dimensionally incorrect (Energy + Energy/Kelvin $\neq$ 0). The Temperature $T$ mysteriously vanished in the middle steps, only to magically reappear in the final answer (Equation 22). **Ignore the missing $T$ in the intermediate steps of the image; it is a typo.** The derivation I am showing you here is the correct physical path.

#### Step 3: Solve for n

Now we just use algebra to isolate $n$.

Start with our corrected derivative equation:

$$\Delta H_S - 2 k_B T \cdot \ln\left(\frac{N}{n}\right) = 0$$

Move the log term to the other side:

$$\Delta H_S = 2 k_B T \cdot \ln\left(\frac{N}{n}\right)$$

Divide by $2 k_B T$:

$$\frac{\Delta H_S}{2 k_B T} = \ln\left(\frac{N}{n}\right)$$

To get rid of the natural log ($\ln$), we take the exponent ($e$) of both sides:

$$\exp\left( \frac{\Delta H_S}{2 k_B T} \right) = \frac{N}{n}$$

Finally, flip the fraction upside down (invert both sides) to get $n/N$:

$$\frac{n}{N} = \exp\left( -\frac{\Delta H_S}{2 k_B T} \right)$$

---

### Understanding the Final Result

The final equation is beautiful because it tells a story:

$$n/N \approx e^{-\frac{\Delta H_S}{2 k_B T}}$$

1.  **The "2" in the denominator:** This is the signature of a **Schottky Defect**. Because we created **two** holes (cation + anion), the entropy gain was doubled, which ends up putting a factor of 2 in the bottom. If this were a Frenkel defect (only 1 hole + 1 moved atom), that 2 generally wouldn't be there in the same way.
    
2.  **The Temperature ($T$):** Since $T$ is in the denominator of a negative exponent, as Temperature goes **UP**, the number of defects goes **UP** exponentially.
    
3.  **The Energy Cost ($\Delta H_S$):** Since $\Delta H$ is in the numerator, the harder it is to break the bonds (higher $\Delta H$), the fewer defects you get.
    

**Would you like me to create a quick practice problem? For example, we could calculate the actual number of defects in a grain of salt at 500°C?**