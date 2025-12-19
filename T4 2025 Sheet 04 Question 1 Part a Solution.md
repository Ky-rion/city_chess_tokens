

Hello! This is a fantastic problem and a cornerstone of understanding low-temperature physics. Let's break it down step-by-step, just as we would in a lecture.

The goal is to find the "magnetization heat" ($Q$) for a specific process.

---

## 🏛️ 1. The Core Concept: The First Law of Thermodynamics

Whenever we are asked about heat ($Q$), work ($W$), and energy ($E$), our starting point is always the **First Law of Thermodynamics**. It's the universe's energy conservation rule.

In its differential form, it states:

$$dE = dQ + dW$$

Where:

-   $dE$ is the tiny change in the **internal energy** of our system (the paramagnet).
    
-   $dQ$ is the tiny amount of **heat** added _to_ the system.
    
-   $dW$ is the tiny amount of **work** done _on_ the system.
    

To find the total heat $Q$ for the whole process, we would integrate this equation:

$\Delta E = Q + W$

This means **$Q = \Delta E - W$**. So, our plan is simple:

1.  Find the total change in internal energy, $\Delta E$.
    
2.  Find the total work done, $W$.
    
3.  Subtract $W$ from $\Delta E$ to find $Q$.
    

---

## ✏️ 2. Step 1: The Change in Internal Energy ($\Delta E$)

This is the most important (and simplest!) part of this question.

-   The problem _gives_ us the formula for internal energy: $E = \alpha N T^4$.
    
-   Notice that this formula depends **only on temperature ($T$)**. It does _not_ depend on the magnetic field ($B$).
    
-   The problem _tells_ us the process is **isothermal**, meaning the temperature is held constant at $T = T_1$.
    

So, let's look at the energy at the start and end of the process:

-   **Initial State:** $B = 0$, $T = T_1 \implies E_{\text{initial}} = \alpha N T_1^4$
    
-   **Final State:** $B = B_1$, $T = T_1 \implies E_{\text{final}} = \alpha N T_1^4$
    

The change in internal energy $\Delta E$ is $E_{\text{final}} - E_{\text{initial}}$:

$\Delta E = (\alpha N T_1^4) - (\alpha N T_1^4) = 0$

**This is a huge simplification!** Because the process is isothermal and the energy only depends on temperature, the internal energy does _not change at all_.

---

## ⚙️ 3. Step 2: Simplifying and Finding the Work ($W$)

Now we go back to our First Law equation:

$\Delta E = Q + W$

Since we just proved that $\Delta E = 0$, our equation becomes:

$0 = Q + W$

...which means:

$Q = -W$

This tells us something very important physically: the "magnetization heat" we're looking for is simply the **negative** of the magnetic work done on the system. To keep the temperature from rising, any work you do _on_ the magnet must be immediately removed _as_ heat.

Now, we just need to calculate the total work, $W$.

-   The problem gives us the differential work term: $dW = B dM$.
    
-   To find the total work $W$, we must integrate this from the initial state to the final state:
    
    $W = \int dW = \int_{\text{start}}^{\text{end}} B dM$
    

This integral is a bit tricky, as it has both $B$ and $dM$. We need to express everything in terms of one variable. The easiest variable to use is the magnetic field, $B$, since it just goes from $0$ to $B_1$.

We need to find out what $dM$ is in terms of $dB$.

1.  We are given the formula for magnetization:
    
    $M = a \frac{NB}{T}$
    
2.  During our process, $T$ is held constant at $T_1$. So, for this specific path, the formula is:
    
    $M = \frac{aN}{T_1} B$
    
3.  Now, let's find the differential $dM$ by differentiating this expression. Since $a$, $N$, and $T_1$ are all constants:
    
    $dM = d \left( \frac{aN}{T_1} B \right) = \left( \frac{aN}{T_1} \right) dB$
    

Now we can substitute this expression for $dM$ back into our work integral:

$W = \int_{B=0}^{B=B_1} B \cdot \left( \frac{aN}{T_1} dB \right)$

We can pull all the constants ($a, N, T_1$) out of the integral:

$W = \frac{aN}{T_1} \int_0^{B_1} B dB$

This is now a very simple integral:

-   $\int B dB = \frac{1}{2} B^2$
    

Let's evaluate this at our limits (from $0$ to $B_1$):

$W = \frac{aN}{T_1} \left[ \frac{1}{2} B^2 \right]_0^{B_1}$

$W = \frac{aN}{T_1} \left( \left( \frac{1}{2} B_1^2 \right) - \left( \frac{1}{2} (0)^2 \right) \right)$

$W = \frac{aN B_1^2}{2T_1}$

This is the total work done _on_ the system.

---

## 💡 4. The Final Answer: The Magnetization Heat ($Q$)

In Step 2, we found that $Q = -W$.

We just calculated $W$, so we can now find our final answer for the heat $Q$:

$$Q = - \frac{aN B_1^2}{2T_1}$$

### What does this mean?

The **negative sign** is the most important physical result. It means that $Q$ is **negative**, which tells us that heat is **flowing _out of_** the paramagnet.

Think about it intuitively:

1.  You apply an external magnetic field ($B$).
    
2.  This field does work ($W$) on the tiny magnetic dipoles in the solid, forcing them to align. This is like "combing" tangled hair—you are doing work to create order.
    
3.  This work (this "combing") adds energy to the system.
    
4.  If you did nothing else, this added energy would make the solid heat up (its temperature would rise).
    
5.  But the problem demands that the temperature **stay constant** ($T=T_1$). The only way for the system to stay at $T_1$ while you are adding work-energy is for it to "dump" an equivalent amount of energy into its surroundings as **heat ($Q$)**.
    

So, work $W = \frac{aN B_1^2}{2T_1}$ flows _in_, and heat $Q = - \frac{aN B_1^2}{2T_1}$ flows _out_, keeping the total internal energy change $\Delta E$ at zero.

This process is the first step in "paramagnetic cooling," as the problem title suggests.

I hope that detailed explanation helps! This is a beautiful example of the First Law in action. Would you like to discuss what happens in the _next_ step of the cooling cycle, which is called adiabatic demagnetization?