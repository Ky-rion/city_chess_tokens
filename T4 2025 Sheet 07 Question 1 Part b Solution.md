

Hello again! It is wonderful to see you continuing with this problem. We are now moving to the **grand finale** of the Third Law of Thermodynamics: proving that absolute zero is physically unreachable.

You have asked for the explanation of **Part (1.b)** (labeled as 2.b in the solution sheet). This question asks us to prove that the rate of temperature change with respect to pressure drops to zero as $T \to 0$, and to discuss what this implies for reaching absolute zero.

Here is the step-by-step breakdown of the professor's solution.

---

### Part (b): The Proof of Unattainability

The Goal

We want to evaluate the quantity $\left(\frac{\partial T}{\partial P}\right)_S$ as $T \rightarrow 0$.

This derivative describes adiabatic cooling. It answers the question: "If I insulate my system (keeping Entropy $S$ constant) and change the pressure ($P$), how much does the Temperature ($T$) change?"

Step 1: The Total Differential of Entropy

Just like in the previous part, we start with the total differential of entropy. Entropy $S$ is a function of Pressure ($P$) and Temperature ($T$), so a small change $dS$ is given by:

$$dS = \left(\frac{\partial S}{\partial P}\right)_T dP + \left(\frac{\partial S}{\partial T}\right)_P dT$$

Step 2: Substituting Known Physical Quantities

We need to replace those abstract partial derivatives with measurable quantities ($C_P$, $V$, $\beta$).

1.  **The First Term:** From the Maxwell relation we used in Part (a), we know that $\left(\frac{\partial S}{\partial P}\right)_T = -V\beta$.
    
2.  **The Second Term:** By the definition of heat capacity, we know that $\left(\frac{\partial S}{\partial T}\right)_P = \frac{C_P}{T}$.
    

Substituting these into our equation for $dS$, we get:

$$dS = -V\beta dP + \frac{C_P}{T} dT$$

Step 3: Applying the Adiabatic Condition ($dS = 0$)

The derivative we want to find is $\left(\frac{\partial T}{\partial P}\right)_S$. The subscript $S$ means Entropy is constant (an adiabatic process).

Therefore, we set $dS = 0$ and solve for the ratio $\frac{dT}{dP}$:

$$0 = -V\beta dP + \frac{C_P}{T} dT$$

Rearranging the terms:

$$\frac{C_P}{T} dT = V\beta dP$$

$$\left(\frac{\partial T}{\partial P}\right)_S = T \cdot \frac{V\beta}{C_P}$$

Step 4: Taking the Limit as $T \to 0$

Now we check what happens as we approach absolute zero. We have two parts in our expression:

1.  The factor **$T$**: This obviously goes to $0$.
    
2.  The factor **$\frac{V\beta}{C_P}$**: In Part (a), we proved that this ratio approaches a **finite constant** (specifically $-\frac{1}{x} \frac{\partial \ln a}{\partial P}$).
    

Since we are multiplying "zero" by a "finite number," the result is zero:

$$\lim_{T \to 0} \left(\frac{\partial T}{\partial P}\right)_S = 0 \cdot (\text{finite constant}) = 0$$

---

### Discussion: Why is Absolute Zero Unattainable?

The question asks you to "discuss the attainability of absolute zero".

The Physics of Cooling

To cool a substance to very low temperatures, we typically use a cycle of two steps:

1.  **Isothermal Compression:** We squeeze the gas while letting heat escape (reducing entropy).
    
2.  **Adiabatic Expansion:** We isolate the gas and expand it. This usually causes the temperature to drop significantly.
    

The Consequence of our Proof

Our result $\lim_{T \to 0} \left(\frac{\partial T}{\partial P}\right)_S = 0$ tells us that as we get closer to absolute zero, the "cooling power" of the adiabatic step vanishes.

-   At high temperatures, changing pressure ($dP$) causes a large drop in temperature ($dT$).
    
-   At temperatures near zero, changing pressure ($dP$) causes almost **no** drop in temperature ($dT$).
    

Because the temperature drop per step becomes infinitesimally small, you would need an **infinite number of steps** to actually reach $T=0$. Since we cannot perform an infinite number of operations in finite time, **absolute zero is unattainable**.

This is often stated as the alternative formulation of the Third Law of Thermodynamics: _"It is impossible to reach absolute zero using a finite number of processes."_

---

### Summary for your notes

-   **The Math:** We set $dS=0$ and rearranged the total differential to find the slope of the adiabatic process ($\frac{dT}{dP}$).
    
-   **The Result:** The slope vanishes ($\rightarrow 0$) because of the factor $T$ in the heat capacity relation.
    
-   **The Meaning:** You cannot cool down any further using pressure changes once you get close to zero. The "handle" you use to control temperature simply stops working.
    

**Would you like to move on to Problem 2, where we leave the abstract world and apply this to a "Real Gas" equation of state?**