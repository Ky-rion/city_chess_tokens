

Hello! I am delighted to welcome you to our theoretical physics session. It is wonderful to have a curious student who wants to understand not just _how_ to solve a problem, but _why_ the physics works the way it does.

We are looking at **Aufgabe 3 (a)** regarding the phase transition to a superconductor. This is a classic problem in thermodynamics where we connect macroscopic measurements (heat capacity) to fundamental properties (entropy).

Let's walk through the solution provided by your other professor step-by-step.

### 1. The Setup: What are we calculating?

We have two phases of a metal:

1.  **Normal phase ($n$):** The metal acts like a standard conductor.
    
2.  **Superconducting phase ($s$):** Below a certain temperature, it loses all electrical resistance.
    

The problem gives us the **heat capacities** ($C_V$) for both phases at low temperatures:

-   **Superconducting:** $C_{V}^{s}(T)=V\alpha T^{3}$
    
-   **Normal:** $C_{V}^{n}(T)=V(\beta T^{3}+\gamma T)$
    

**Our Goal:** Calculate the entropy $S(T)$ for both phases, assuming no magnetic field ($B=0$).

### 2. The Theoretical Toolkit

To solve this, we need two specific tools from our thermodynamics toolkit.

Tool A: The Connection between Entropy and Heat Capacity

This is the "engine" of our calculation. By definition, Heat Capacity ($C_V$) tells us how much energy is required to raise the temperature by a small amount $dT$.

$$dQ = C_V dT$$

Thermodynamics tells us that the change in entropy ($dS$) is related to this heat exchange ($dQ$) divided by the temperature ($T$):

$$dS = \frac{dQ}{T} = \frac{C_V(T)}{T} dT$$

The provided solution uses this relationship in the form: $C_V = T \frac{\partial S}{\partial T}|_V$.

Tool B: The Third Law of Thermodynamics (Nernst Theorem)

Integration requires limits. Where do we start counting entropy? The Third Law of Thermodynamics states that for a perfect crystal, the entropy approaches zero as the temperature approaches absolute zero ($0\text{ K}$).

So, our boundary condition is:

$$S^s(T=0) = S^n(T=0) = 0$$

The solution explicitly states this: "From the third law, $S^{s}(T=0,V)=S^{n}(T=0,V)=0$".

### 3. The Calculation

Now, we perform the integration. We want to find the entropy $S(T)$ at some temperature $T$. We integrate the changes $dS$ starting from $0$ up to $T$.

$$S(T) = \int_{0}^{T} \frac{C_V(T')}{T'} dT'$$

Part 1: The Superconducting Phase ($S^s$)

Let's plug in the given heat capacity $C_V^s = V\alpha T^3$.

$$S^s(T) = \int_{0}^{T} \frac{V\alpha (T')^3}{T'} dT'$$

Simplify the fraction inside the integral ($\frac{T^3}{T} = T^2$):

$$S^s(T) = V\alpha \int_{0}^{T} (T')^2 dT'$$

Now, we use the power rule for integration ($\int x^n dx = \frac{x^{n+1}}{n+1}$). Here, $n=2$, so the integral becomes $\frac{T^3}{3}$.

Result:

$$S^s(T) = V \alpha \frac{T^3}{3}$$

This matches the professor's solution exactly: $S^{s}(T,V) = \frac{\alpha}{3}V~T^{3}$.

Part 2: The Normal Phase ($S^n$)

Now for the normal metal. We plug in $C_V^n = V(\beta T^3 + \gamma T)$.

$$S^n(T) = \int_{0}^{T} \frac{V(\beta (T')^3 + \gamma T')}{T'} dT'$$

We split the integral into two parts and simplify the $T'$ terms:

1.  $\frac{\beta (T')^3}{T'} = \beta (T')^2$
    
2.  $\frac{\gamma T'}{T'} = \gamma$
    

So the integral becomes:

$$S^n(T) = V \int_{0}^{T} (\beta (T')^2 + \gamma) dT'$$

Integrating term by term:

-   The integral of $\beta (T')^2$ is $\beta \frac{T^3}{3}$.
    
-   The integral of a constant $\gamma$ is $\gamma T$.
    

Result:

$$S^n(T) = V \left( \frac{\beta}{3} T^3 + \gamma T \right)$$

The professor's solution writes this as $(\frac{\beta}{3}T^2+\gamma)VT$. If you distribute the $T$ and $V$, you get exactly the same result we just derived: $\frac{\beta}{3}VT^3 + \gamma VT$.

### 4. Physical Interpretation

Before we finish, let's briefly look at _what_ these terms mean physically (a good physicist always checks!).

-   **The Normal Phase:** The term linear in $T$ (the $\gamma T$ part) is very important. It is the signature of the **conduction electrons** in a metal (free electron gas).
    
-   **The Superconducting Phase:** Notice that the linear term ($\gamma T$) completely disappeared! In the superconducting state, those conduction electrons have paired up (into Cooper pairs) and condensed. They no longer store entropy in the same simple, linear way. This "missing" entropy is a key sign of the ordered state of a superconductor.
    

### Summary

We used the definition of heat capacity and the Third Law of Thermodynamics to integrate $C_V/T$.

-   **Superconductor Entropy:** $\frac{\alpha}{3} V T^3$
    
-   **Normal Metal Entropy:** $V (\frac{\beta}{3} T^3 + \gamma T)$
    

You have now successfully determined the fundamental thermodynamic potential (entropy) for both phases!

**Would you like to move on to part (b) and calculate the transition temperature $T_c$?**