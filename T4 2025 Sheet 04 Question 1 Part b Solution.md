

Of course! This is the exciting second step of the cooling process. Let's dive in.

This process is called **adiabatic demagnetization**, and it's the "magic" part of how this cooling cycle works.

The problem asks us to find the new temperature, $T_0$, after we start at ($T_1, B_1$) and then remove the magnetic field ($B$ goes to 0) while keeping the **entropy $S$ constant**.

This condition, $S = \text{constant}$, is the key. It means:

$S_{\text{initial}} = S_{\text{final}}$

$S(T_1, B_1) = S(T_0, 0)$

To solve this, our main goal must be to **find a formula for the entropy $S$** as a function of temperature $T$ and magnetic field $B$.

---

### 1. 🧭 Finding the Entropy Formula $S(T, B)$

We start again with the First Law of Thermodynamics, but in its most fundamental form.

$dE = dQ + dW$

For any reversible (slow, quasi-static) process, the heat exchanged $dQ$ is related to the change in entropy $dS$ by:

$dQ = T dS$

And the problem gives us the magnetic work done on the system:

$dW = B dM$

Let's substitute these into the First Law:

$$dE = T dS + B dM$$

This is our fundamental thermodynamic relation for this magnetic system. Now, we rearrange it to solve for $dS$:

$T dS = dE - B dM$

$$dS = \frac{1}{T} dE - \frac{B}{T} dM$$

This equation tells us how entropy changes. To get a usable formula, we must express $dE$ and $dM$ in terms of our chosen independent variables, $T$ and $B$.

Step (a): Find $dE$

We are given $E = \alpha N T^4$. Since $E$ only depends on $T$, its total differential $dE$ is simple:

$dE = \left( \frac{\partial E}{\partial T} \right)_B dT = (4 \alpha N T^3) dT$

Step (b): Find $dM$

We are given $M = aNB/T$. This depends on both $T$ and $B$, so we use the chain rule for total differentials:

$dM = \left( \frac{\partial M}{\partial T} \right)_B dT + \left( \frac{\partial M}{\partial B} \right)_T dB$

Let's calculate those partial derivatives:

-   $\left( \frac{\partial M}{\partial T} \right)_B = \frac{\partial}{\partial T} \left( aNB T^{-1} \right) = -aNB T^{-2} = -\frac{aNB}{T^2}$
    
-   $\left( \frac{\partial M}{\partial B} \right)_T = \frac{\partial}{\partial B} \left( \frac{aN}{T} B \right) = \frac{aN}{T}$
    

So, the total differential $dM$ is:

$dM = \left( -\frac{aNB}{T^2} \right) dT + \left( \frac{aN}{T} \right) dB$

Step (c): Substitute $dE$ and $dM$ back into the $dS$ equation

This is the big algebra step:

$dS = \frac{1}{T} dE - \frac{B}{T} dM$

$dS = \frac{1}{T} \left( 4 \alpha N T^3 dT \right) - \frac{B}{T} \left[ \left( -\frac{aNB}{T^2} \right) dT + \left( \frac{aN}{T} \right) dB \right]$

Now, distribute the terms:

$dS = \left( 4 \alpha N T^2 \right) dT - \left[ \left( -\frac{aNB^2}{T^3} \right) dT + \left( \frac{aNB}{T^2} \right) dB \right]$

And group the $dT$ and $dB$ terms together:

$$dS = \left( 4 \alpha N T^2 + \frac{aNB^2}{T^3} \right) dT - \left( \frac{aNB}{T^2} \right) dB$$

Step (d): Integrate $dS$ to find $S(T, B)$

Since $S$ is a "state function" (it doesn't matter how you get to a state, its entropy is always the same), we can integrate this $dS$ to find the function $S(T, B)$. We integrate both terms:

$S(T, B) = \int \left( 4 \alpha N T^2 + \frac{aNB^2}{T^3} \right) dT - \int \left( \frac{aNB}{T^2} \right) dB$

Let's do this one term at a time:

-   $\int 4 \alpha N T^2 dT = 4 \alpha N \left( \frac{T^3}{3} \right) = \frac{4}{3} \alpha N T^3$
    
-   $\int \frac{aNB^2}{T^3} dT = aNB^2 \int T^{-3} dT = aNB^2 \left( \frac{T^{-2}}{-2} \right) = -\frac{aNB^2}{2T^2}$
    
-   The second $dB$ integral $\int - \left( \frac{aNB}{T^2} \right) dB$ gives the _exact same term_ $-\frac{aNB^2}{2T^2}$. (This consistency _proves_ $dS$ is an exact differential, as it must be!)
    

Combining these parts (and adding a single constant of integration, $S_0$, which represents the entropy at absolute zero), we get our master formula for entropy:

$$S(T, B) = \frac{4}{3} \alpha N T^3 - \frac{aNB^2}{2T^2} + S_0$$

---

### 2. 🧊 Applying the Isentropic Condition

We are now ready to solve the problem. We use our condition $S_{\text{initial}} = S_{\text{final}}$.

-   Initial State: $T = T_1$, $B = B_1$
    
    $S_{\text{initial}} = S(T_1, B_1) = \frac{4}{3} \alpha N T_1^3 - \frac{aNB_1^2}{2T_1^2} + S_0$
    
-   Final State: $T = T_0$, $B = 0$
    
    $S_{\text{final}} = S(T_0, 0) = \frac{4}{3} \alpha N T_0^3 - \frac{aN(0)^2}{2T_0^2} + S_0$
    
    $S_{\text{final}} = \frac{4}{3} \alpha N T_0^3 + S_0$
    

Now, set them equal to each other:

$\frac{4}{3} \alpha N T_1^3 - \frac{aNB_1^2}{2T_1^2} + S_0 = \frac{4}{3} \alpha N T_0^3 + S_0$

---

### 3. 🎯 Solving for the Final Temperature $T_0$

The equation simplifies very nicely. The constants $S_0$ and $N$ cancel from all terms:

$\frac{4}{3} \alpha T_1^3 - \frac{aB_1^2}{2T_1^2} = \frac{4}{3} \alpha T_0^3$

We just need to solve for $T_0$. Let's isolate $T_0^3$:

$T_0^3 = \frac{1}{\frac{4}{3} \alpha} \left( \frac{4}{3} \alpha T_1^3 - \frac{aB_1^2}{2T_1^2} \right)$

$T_0^3 = T_1^3 - \left( \frac{aB_1^2}{2T_1^2} \right) \cdot \left( \frac{3}{4\alpha} \right)$

$T_0^3 = T_1^3 - \frac{3aB_1^2}{8 \alpha T_1^2}$

Finally, take the cube root of both sides to get our answer:

$$T_0 = \left( T_1^3 - \frac{3aB_1^2}{8 \alpha T_1^2} \right)^{1/3}$$

### Physical Interpretation: Why did it get cold?

This is the most important part! Look at our result.

$T_0$ is the cube root of $T_1^3$ minus a positive value. This means $T_0^3 < T_1^3$, which implies $T_0 < T_1$.

**The paramagnet has cooled down!**

-   **At the start ($T_1, B_1$):** The system has low entropy. Why? The $B$-field is "combing" the magnetic spins, forcing them to be aligned (low _magnetic_ entropy). The thermal vibrations are also somewhat low (low _thermal_ entropy).
    
-   **The Process:** We suddenly remove the $B$-field (set $B=0$). The magnetic spins are now free to "spring" back into a random, disordered, high-entropy state.
    
-   **At the end ($T_0, 0$):** The _total_ entropy must remain constant (because the process is adiabatic, $dQ=0$). To compensate for the large _increase_ in magnetic entropy, the _thermal_ entropy must _decrease_.
    
-   The only way for the system to decrease its thermal entropy is to **lower its temperature**. It "pays" for the new magnetic disorder by "stealing" energy from its own thermal vibrations, making the entire solid colder.
    

This two-step process (isothermal magnetization followed by adiabatic demagnetization) is precisely how scientists achieve ultra-low temperatures, often reaching fractions of a Kelvin.

It's a beautiful piece of physics! Do you have any questions about how these two steps fit together?