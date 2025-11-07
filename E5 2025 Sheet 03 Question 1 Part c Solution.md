

This is the perfect conclusion to our problem! We will once again use the law of radioactive decay, but in a very direct and elegant way.

Let's get started.

---

### 1. The Core Physical Principle

Here is the key insight:

-   The **electric power** ($P_{\text{electric}}$) we get is just the **thermal power** ($P_{\text{thermal}}$) multiplied by a constant efficiency ($\eta = 0.05$).
    
-   The **thermal power** ($P_{\text{thermal}}$) is just the **activity** ($A$) multiplied by the constant energy-per-decay ($E_{\text{decay}}$).
    

So, we can write:

$P_{\text{electric}} = \eta \times P_{\text{thermal}} = \eta \times (A \times E_{\text{decay}})$

Since $\eta$ and $E_{\text{decay}}$ are both constants, the **electric power ($P_{\text{electric}}$) is directly proportional to the activity ($A$)**.

What does this mean? It means that the **electric power itself must decay over time, following the exact same radioactive decay law as the plutonium atoms!**

The formula for decay is: $N(t) = N_0 e^{-\lambda t}$

For activity, it's: $A(t) = A_0 e^{-\lambda t}$

And therefore, for power, it is: $P(t) = P_0 e^{-\lambda t}$

---

### 2. The Strategy: A "Point-to-Point" Calculation

We could calculate the initial power at launch ($P_0$) and then use the 4387-day travel time to Neptune ($t_N$) to find the final power.

But there is a much more direct (and clever) way:

1.  We **know** the exact power when Voyager 2 reached Saturn ($P_S = 400 \text{ W}$).
    
2.  We **know** the time it took to get to Saturn ($t_S = 1467 \text{ days}$).
    
3.  We **know** the time it took to get to Neptune ($t_N = 4387 \text{ days}$).
    

We can simply calculate how much the power _decayed_ during the journey **between** Saturn and Neptune.

---

### 3. Step 1: Find the Time Elapsed Between Planets

Let's find the time $\Delta t$ (delta-t, or "change in time") for the probe to fly from Saturn to Neptune.

-   $\Delta t = t_N - t_S$
    
-   $\Delta t = 4387 \text{ days} - 1467 \text{ days}$
    
-   **$\Delta t = 2920 \text{ days}$**
    

So, the generator was running (and decaying) for 2920 days between these two encounters.

---

### 4. Step 2: Use the Radioactive Decay Law for Power

We will use the decay law, starting from Saturn:

$P_N = P_S \cdot e^{-\lambda (\Delta t)}$

Where:

-   $P_N$ is the power at Neptune (what we want to find).
    
-   $P_S$ is the power at Saturn (400 W).
    
-   $\lambda$ is the decay constant (which we already know from part b).
    
-   $\Delta t$ is the time elapsed between Saturn and Neptune (2920 days).
    

First, let's get our units consistent. We need $\lambda$ and $\Delta t$ in the same units. We used $\text{s}^{-1}$ for $\lambda$ before, so let's convert $\Delta t$ to seconds.

-   $\lambda = 2.495 \times 10^{-10} \text{ s}^{-1}$ (from part b)
    
-   $\Delta t \text{ (in s)} = 2920 \text{ days} \times \frac{24 \text{ h}}{1 \text{ day}} \times \frac{3600 \text{ s}}{1 \text{ h}}$
    
-   **$\Delta t \approx 2.523 \times 10^8 \text{ s}$**
    

---

### 5. Step 3: Calculate the Final Power

Now, we just plug everything into our power-decay formula:

-   $P_N = (400 \text{ W}) \times e^{-(2.495 \times 10^{-10} \text{ s}^{-1}) \times (2.523 \times 10^8 \text{ s})}$
    
-   Let's calculate that exponent first: $-(2.495 \times 10^{-10}) \times (2.523 \times 10^8) \approx -0.06295$
    
-   $P_N = 400 \text{ W} \times e^{-0.06295}$
    
-   $P_N = 400 \text{ W} \times 0.93898$
    
-   **$P_N \approx 375.59 \text{ W}$**
    

### Final Answer

When Voyager 2 reached Neptune after 4387 days, the generators were delivering **375.6 W** of power.

This calculation shows how incredibly stable and predictable these radioisotope generators are. Scientists could predict _exactly_ how much power the probe would have at each stage of its decades-long journey. This is why, even today (as of 2024), Voyager 2 is _still_ transmitting data from interstellar space, all thanks to the steady decay of its ${}^{238}\text{Pu}$ power source.

This completes our three-part problem! We've gone from a single decay's energy all the way to predicting the power of a deep-space probe.

Would you like to try another problem, perhaps on a different topic like radioactive dating or nuclear reactions?