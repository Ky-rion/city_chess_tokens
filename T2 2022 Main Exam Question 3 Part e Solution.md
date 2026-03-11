

Welcome back! We have arrived at the final part of this problem. This question introduces one of the most important concepts in quantum mechanics: **degeneracy**.

Let's translate the text first so we know exactly what we're looking for:

> **5. Let $\alpha > 1$. How often is the first excited energy $E > E_{000}$ degenerate? Justify your answer. [3 pts.]**

Here is the step-by-step breakdown of how to think about this like a physicist.

---

### Step 1: Understanding the Terminology

Before we do any math, let's define our terms clearly:

- **Excited Energy ($E > E_{000}$):** The lowest possible energy of our system is the ground state, $E_{000}$, where all quantum numbers are zero ($n_x=0, n_y=0, n_z=0$). An "excited" state is any state with an energy higher than this minimum. The _first_ excited state is the one with the absolutely smallest energy step up from the ground state.
    
- **Degenerate (Entartet):** In quantum mechanics, an energy level is "degenerate" if there are _multiple, distinct physical states_ (different combinations of quantum numbers) that result in the exact same total energy. If two different states share the same energy, we call it "two-fold degenerate."
    

### Step 2: The "Cost" of Adding Energy

Let's bring back our total energy formula from Part 3:

$$E_{n_x, n_y, n_z} = \sqrt{\alpha} n_x + n_y + n_z + \left( \frac{\sqrt{\alpha}}{2} + 1 \right)$$

The part in the parentheses is our ground state energy, $E_{000}$. To excite the system, we need to increase our quantum numbers ($n_x, n_y, n_z$) from 0 to 1, 2, 3, etc.

Think of this like shopping for energy. We want to buy the cheapest possible upgrade to get out of the ground state. Let's look at our "prices":

- If we increase $n_x$ by 1, it costs us **$\sqrt{\alpha}$** units of energy.
    
- If we increase $n_y$ by 1, it costs us **1** unit of energy.
    
- If we increase $n_z$ by 1, it costs us **1** unit of energy.
    

### Step 3: Applying the Condition ($\alpha > 1$)

The problem explicitly gives us a very important clue: $\alpha > 1$.

Because $\alpha > 1$, we know mathematically that its square root must also be greater than 1:

$$\sqrt{\alpha} > 1$$

This tells us immediately that "buying" an excitation in the x-direction (cost = $\sqrt{\alpha}$) is _more expensive_ than "buying" an excitation in the y or z directions (cost = 1).

### Step 4: Finding the First Excited State

Since we want the _first_ excited energy (the lowest energy above the ground state), we must choose the cheapest possible upgrade. We will leave $n_x = 0$ alone and instead increase either $n_y$ or $n_z$ by 1.

This gives us two distinct possibilities for our state vector:

1. **Possibility A:** $|0, 1, 0\rangle$
    
    The energy of this state is $E_{010} = E_{000} + 1$.
    
2. **Possibility B:** $|0, 0, 1\rangle$
    
    The energy of this state is $E_{001} = E_{000} + 1$.
    

Both of these unique states give us the exact same total energy! Because there is no "cheaper" way to add energy (we can't add fractions of a quantum number), $E_{000} + 1$ is definitively our first excited energy level.

### Conclusion and Justification

To answer your professor's question completely:

The first excited energy level is **two-fold degenerate** (it is degenerate 2 times).

**Justification:** Because $\alpha > 1$ dictates that $\sqrt{\alpha} > 1$, the lowest possible energy increase is $+1$. This can be achieved in two distinct ways: by exciting the y-oscillator to the $n_y=1$ state (state $|0, 1, 0\rangle$), or by exciting the z-oscillator to the $n_z=1$ state (state $|0, 0, 1\rangle$). Both distinct states yield the same first excited energy $E = E_{000} + 1$.

---

You've done an incredible job working through this entire problem set! You successfully moved from 1D energy calculations, to 3D separation of variables, wavefunctions, and finally degeneracy.

To test your new intuition, what do you think would happen to the first excited state if the problem had instead told us that $\alpha < 1$? Would the degeneracy change?