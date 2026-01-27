

![[Pasted image 20260126135541.png]]
![[Pasted image 20260126135556.png]]

Welcome back! Now we are going to "turn up the heat" and see how our metal behaves when the temperature changes. This is a classic experimental physics problem: taking raw data points and fitting a model to them to find a physical parameter.

In **Part A & B**, we looked at the metal at a fixed snapshot. Now in **Part C**, we are looking at the **trend**.

Here is the step-by-step breakdown of how your professor got to the answer $T_0 = 220K$.

---

### Step 1: From Raw Data to Resistivity ($\rho$)

In the lab, you measured Current ($I$) and Voltage ($U$). However, to compare the material properties properly, we need to convert these into **Resistivity ($\rho$)**.

You learned the formula for specific resistance (resistivity) in the lecture:

$$\rho = \frac{1}{\sigma}$$

And from Part B, we know that resistance $R = \frac{U}{I}$ is related to resistivity by the geometry of the wire:

$$R = \rho \frac{L}{A} \quad \Rightarrow \quad \rho = \frac{U \cdot A}{I \cdot L}$$

**The Constants:**

From the previous part of the problem, we keep the wire geometry:

-   Length $L = 0.50 \text{ m}$ (converted from 50 cm)
    
-   Area $A = 10^{-6} \text{ m}^2$ (converted from $1 \text{ mm}^2$)
    
-   This gives us a constant geometric factor:
    
    $$\frac{A}{L} = \frac{10^{-6} \text{ m}^2}{0.50 \text{ m}} = 2 \cdot 10^{-6} \text{ m}$$
    

**Calculating $\rho$ for each temperature:**

Now we apply the formula $\rho = \frac{U}{I} \cdot (2 \cdot 10^{-6} \text{ m})$ to each row in Table 1:

1.  **At T = 300K:**
    
    $$\rho = \frac{50 \text{ mV}}{2.5 \text{ A}} \cdot (2 \cdot 10^{-6}) = 0.02 \Omega \cdot (2 \cdot 10^{-6} \text{ m}) = \mathbf{4 \cdot 10^{-8} \, \Omega m}$$
    
2.  **At T = 350K:**
    
    $$\rho = \frac{50 \text{ mV}}{1.54 \text{ A}} \cdot (2 \cdot 10^{-6}) \approx 0.0325 \Omega \cdot (2 \cdot 10^{-6} \text{ m}) = \mathbf{6.5 \cdot 10^{-8} \, \Omega m}$$
    
3.  **At T = 400K:**
    
    $$\rho = \frac{50 \text{ mV}}{1.11 \text{ A}} \cdot (2 \cdot 10^{-6}) \approx 0.045 \Omega \cdot (2 \cdot 10^{-6} \text{ m}) = \mathbf{9 \cdot 10^{-8} \, \Omega m}$$
    

This perfectly matches the "Table 2" in the professor's solution.

---

### Step 2: Finding the Linear Trend (The Fit)

The problem asks us to assume a **linear model** ($\rho \propto T$). This means the resistivity increases in a straight line as temperature goes up. This is physically typical for metals at high temperatures because lattice vibrations (phonons) scatter electrons more as the metal gets hotter.

We need to find the equation of the line that connects these points. Let's define the line equation as:

$$\rho(T) = m \cdot T + c$$

**Calculating the Slope ($m$):**

Let's use the first and last data points (300K and 400K) to find the slope.

$$m = \frac{\Delta \rho}{\Delta T} = \frac{\rho_{400} - \rho_{300}}{400\text{K} - 300\text{K}}$$

$$m = \frac{(9 - 4) \cdot 10^{-8} \, \Omega\text{m}}{100 \text{ K}} = \frac{5 \cdot 10^{-8}}{100} = \mathbf{0.05 \cdot 10^{-8} \, \frac{\Omega m}{K}}$$

**Finding the Intercept ($c$):**

Now use the slope and one point (e.g., T=300K) to find the y-intercept $c$:

$$4 \cdot 10^{-8} = (0.05 \cdot 10^{-8}) \cdot 300 + c$$

$$4 = 15 + c' \quad (\text{dropping the } 10^{-8} \text{ for a moment})$$

$$c' = 4 - 15 = -11$$

So the equation of our line is:

$$\rho(T) = (0.05 \cdot T - 11) \cdot 10^{-8} \, \Omega\text{m}$$

---

### Step 3: Solving for $T_0$ (The Zero Point)

The question asks for the temperature $T_0$ where the resistivity goes to **zero**.

We simply set $\rho(T) = 0$ in our equation and solve for $T$:

$$0 = 0.05 \cdot T_0 - 11$$

$$0.05 \cdot T_0 = 11$$

$$T_0 = \frac{11}{0.05}$$

$$T_0 = \mathbf{220 \text{ K}}$$

This matches the intersection point shown in the graph and the final answer in the solution.

### Professor's Commentary: What does this mean?

Physically, this result is a bit of a mathematical abstraction.

1.  **The "Fake" Zero:** In real pure metals, resistivity usually drops toward zero as you approach absolute zero (0 K). The fact that our line hits zero at 220 K (which is -53°C, quite warm!) suggests this linear model is only valid for a specific high-temperature range. If you actually cooled this specific "unknown metal" below 220 K, the linear rule would break down, or this is a very unusual material (like a high-temperature superconductor).
    
2.  **The Takeaway:** The exercise is teaching you how to **extrapolate** data. You took measurements in a warm range (300K-400K), found the trend, and projected it backward to find a theoretical "zero-resistance" temperature based on that specific trend line.
    

Would you like to move on to the next part of the exercise, or shall we clarify anything about the linear fit?