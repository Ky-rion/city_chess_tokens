

Hello! That's an excellent and fundamental question in thermodynamics. It's a classic proof that connects what we _assume_ about a gas (its equation of state) to a very powerful conclusion about its energy.

Let's break down the problem and its solution step-by-step.

### 🎯 The Goal

First, let's translate the problem from the image:

> **Given:**
> 
> 1.  The fundamental thermodynamic relation: $dE = T dS - P dV$
>     
> 2.  The Ideal Gas equation of state: $PV = N k_B T$
>     
> 
> To Prove:
> 
> The internal energy $E$ can only be a function of temperature $T$. (In other words, $E = E(T)$).

What does "E only depends on T" mean mathematically? It means that if we change other variables, like **volume** ($V$) or **pressure** ($P$), the energy $E$ **will not change** _as long as the temperature $T$ stays the same_.

The most direct way to prove this is to show that the change in energy $E$ with respect to volume $V$ _at constant temperature $T$_ is **zero**.

Our mathematical goal is to prove:

$$\left(\frac{\partial E}{\partial V}\right)_T = 0$$

If we can prove this, we've shown that $E$ doesn't depend on $V$. And since $P$, $V$, and $T$ are linked by the equation of state, if $E$ doesn't depend on $V$ at constant $T$, it can't depend on $P$ at constant $T$ either. This leaves $T$ as the _only_ variable that can change $E$.

---

### Derivation: The Step-by-Step Proof

Let's see how we can use our two given "tools" to prove this.

#### Step 1: Find an expression for $\left(\frac{\partial E}{\partial V}\right)_T$

We start with the equation we were given:

$dE = T dS - P dV$

This equation is the "total differential" of $E$ in terms of its "natural variables," $S$ and $V$. But we want to know what happens when we change $V$ while holding $T$ constant.

To do this, we can think of "dividing" the whole equation by $dV$ while holding $T$ constant. (This is a bit of a mathematical shortcut, but it's a good way to think about it.)

$$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial S}{\partial V}\right)_T - P \left(\frac{\partial V}{\partial V}\right)_T$$

The last term is just 1 (the change in $V$ with respect to $V$ is 1), so we get:

$$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial S}{\partial V}\right)_T - P$$

This important equation is sometimes called the **thermodynamic equation of state**. It's true for _any_ substance, not just an ideal gas.

#### Step 2: Deal with the tricky $\left(\frac{\partial S}{\partial V}\right)_T$ term

We have a problem. We want to show the right side is zero, but we have a term, $\left(\frac{\partial S}{\partial V}\right)_T$, that involves entropy ($S$), which we don't know much about. We need to replace it with something we _do_ know, like $P$, $V$, and $T$.

This is where a "magic" tool from thermodynamics called a **Maxwell Relation** comes in. Maxwell relations are powerful shortcuts that come from the fact that thermodynamic energies (like $E$) are "state functions."

I'll show you where this specific one comes from (it's very clever!):

1.  We start with the **Helmholtz free energy**, $F$, which is defined as $F = E - TS$.
    
2.  Let's find its total differential, $dF$:
    
    $dF = dE - d(TS) = dE - (T dS + S dT)$
    
3.  Now, substitute our starting equation $dE = T dS - P dV$:
    
    $dF = (T dS - P dV) - (T dS + S dT)$
    
    $dF = -S dT - P dV$
    
4.  From this new equation, we can see that:
    
    $\left(\frac{\partial F}{\partial T}\right)_V = -S$ and $\left(\frac{\partial F}{\partial V}\right)_T = -P$
    
5.  Because $F$ is a state function, the order of differentiation doesn't matter (Schwarz's theorem). The second derivative $\frac{\partial^2 F}{\partial T \partial V}$ must be equal to $\frac{\partial^2 F}{\partial V \partial T}$.
    
    $\frac{\partial}{\partial V} \left[ \left(\frac{\partial F}{\partial T}\right)_V \right] = \frac{\partial}{\partial T} \left[ \left(\frac{\partial F}{\partial V}\right)_T \right]$
    
    $\frac{\partial}{\partial V} [-S] = \frac{\partial}{\partial T} [-P]$
    
    $-\left(\frac{\partial S}{\partial V}\right)_T = -\left(\frac{\partial P}{\partial T}\right)_V$
    

And... voilà! We have our **Maxwell Relation**:

$$\left(\frac{\partial S}{\partial V}\right)_T = \left(\frac{\partial P}{\partial T}\right)_V$$

This is exactly what we needed! We can replace the messy entropy term with a term involving $P$ and $T$, which we know how to handle from the ideal gas law.

#### Step 3: Substitute the Maxwell Relation

Let's go back to our equation from Step 1:

$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial S}{\partial V}\right)_T - P$

Now, substitute the Maxwell Relation we just found:

$$\left(\frac{\partial E}{\partial V}\right)_T = T \left(\frac{\partial P}{\partial T}\right)_V - P$$

This is a _general_ equation, true for any system. Let's call it our **"test equation"**. We will now "test" the ideal gas with it.

#### Step 4: Use the Ideal Gas Law to finish the proof

Now we finally use the second piece of information: the ideal gas law $PV = N k_B T$.

Our "test equation" needs the term $\left(\frac{\partial P}{\partial T}\right)_V$. Let's calculate it.

First, rearrange the ideal gas law to solve for $P$:

$P = \frac{N k_B T}{V}$

Now, take the partial derivative with respect to $T$, while holding $V$ constant:

$\left(\frac{\partial P}{\partial T}\right)_V = \frac{\partial}{\partial T} \left[ \frac{N k_B T}{V} \right]$

Since $N$, $k_B$, and $V$ are all treated as constants for this derivative, we get:

$\left(\frac{\partial P}{\partial T}\right)_V = \frac{N k_B}{V}$

Now we substitute this result back into our "test equation" from Step 3:

$\left(\frac{\partial E}{\partial V}\right)_T = T \left( \frac{N k_B}{V} \right) - P$

Let's simplify that first term:

$\left(\frac{\partial E}{\partial V}\right)_T = \left( \frac{N k_B T}{V} \right) - P$

But wait... look at that term in the parentheses! From the ideal gas law, we know that $P = \frac{N k_B T}{V}$. So we can replace that whole term with $P$:

$\left(\frac{\partial E}{\partial V}\right)_T = P - P$

$$\left(\frac{\partial E}{\partial V}\right)_T = 0$$

---

### 💡 The "Big Picture" Conclusion

We have successfully proven that $\left(\frac{\partial E}{\partial V}\right)_T = 0$.

This result is called **Joule's Law** (or sometimes the "second law of Joule"). It tells us that for a gas that _obeys the ideal gas law_, its internal energy $E$ does **not** depend on its volume $V$.

**Why is this physically?**

-   An "ideal gas" is a theoretical model where we assume the gas particles are just tiny points that don't interact with each other (no attractive or repulsive forces).
    
-   The **internal energy** ($E$) of such a gas is purely the sum of the **kinetic energy** (energy of motion) of all its particles.
    
-   **Temperature** ($T$) is a measure of the _average_ kinetic energy of the particles.
    
-   Therefore, if you keep the temperature $T$ constant, the average kinetic energy of the particles is constant, and the _total_ internal energy $E$ is also constant.
    
-   It doesn't matter if you put the particles in a small box or a large box (changing $V$). As long as they have the same temperature, they have the same total energy. The energy doesn't depend on how far apart they are, because we assumed they don't interact with each other anyway!
    

So, the equation of state $PV = N k_B T$ (which models non-interacting particles) _forces_ the conclusion that the internal energy $E$ can only depend on temperature $T$.

Does that step-by-step derivation make sense? We can go over the Maxwell relations again if you'd like, as that's usually the trickiest part!