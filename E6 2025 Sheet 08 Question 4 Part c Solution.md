

![[Pasted image 20260125190612.png]]

Welcome back to the third act of our derivation! This is where the magic happens. We are going to connect the "counting games" we played in Part (b) to real Thermodynamics.

This part is often the most mathematically dense, so let's walk through it slowly.

---

### The Goal of Part c)

> **German:** "Verwenden Sie nun die Stirlingformel... um $\frac{\partial S}{\partial N_i}$ zu berechnen."
> 
> **English:** "Now use Stirling's formula... to calculate $\frac{\partial S}{\partial N_i}$."

We want to find how the **Entropy ($S$)** changes when we add one particle ($N_i$).

We start with **Boltzmann's Tombstone Equation**:

$$S = k_B \ln(\Omega)$$

Since our total system is made of many independent energy levels, the total number of states is the product of the states of each level ($\Omega = \Omega_1 \cdot \Omega_2 \cdot \dots$).

Because of the logarithm rules ($\ln(A \cdot B) = \ln A + \ln B$), the total entropy is the sum:

$$S = k_B \sum_j \ln(\Omega_j)$$

---

### Step 1: Breaking down the Logarithms

From Part (b), we know:

$$\Omega_i = \frac{D_i!}{N_i! (D_i - N_i)!}$$

Let's take the natural log ($\ln$) of this. Remember that division inside a log becomes subtraction:

$$\ln(\Omega_i) = \ln(D_i!) - \ln(N_i!) - \ln((D_i - N_i)!)$$

This looks messy because of the factorials. This is where **Stirling's Approximation** comes to the rescue.

---

### Step 2: Stirling's Approximation

Stirling's formula is a cheat code for dealing with factorials of huge numbers (like the number of atoms in a solid):

$$\ln(x!) \approx x \ln(x) - x$$

Let's apply this cheat code to all three terms in our equation.

1.  **Term 1:** $\ln(D_i!) \approx D_i \ln(D_i) - D_i$
    
2.  **Term 2:** $\ln(N_i!) \approx N_i \ln(N_i) - N_i$
    
3.  **Term 3:** $\ln((D_i - N_i)!) \approx (D_i - N_i) \ln(D_i - N_i) - (D_i - N_i)$
    

Now, substitute these back into our big equation:

$$\ln(\Omega_i) \approx [D_i \ln(D_i) - D_i] - [N_i \ln(N_i) - N_i] - [(D_i - N_i) \ln(D_i - N_i) - (D_i - N_i)]$$

**The Great Cancellation:**

Look at the linear terms (the ones without "ln").

We have: $- D_i - (-N_i) - (-(D_i - N_i))$

$= - D_i + N_i + D_i - N_i = 0$

They all cancel out! We are left with just the logarithmic terms, exactly as shown in your solution image:

$$\ln(\Omega_i) \approx D_i \ln(D_i) - N_i \ln(N_i) - (D_i - N_i) \ln(D_i - N_i)$$

---

### Step 3: Taking the Derivative

Now we need to take the derivative with respect to $N_i$:

$$\frac{\partial}{\partial N_i} \ln(\Omega_i)$$

Let's look at the three terms again:

1.  $D_i \ln(D_i)$: This has no $N_i$ in it. **Derivative is 0.**
    
2.  $- N_i \ln(N_i)$: We use the product rule $(fg)' = f'g + fg'$.
    
    -   Derivative is: $- [1 \cdot \ln(N_i) + N_i \cdot \frac{1}{N_i}] = - \ln(N_i) - 1$
        
3.  $- (D_i - N_i) \ln(D_i - N_i)$: This requires the chain rule (notice the minus signs!).
    
    -   Derivative is: $- [(-1) \cdot \ln(D_i - N_i) + (D_i - N_i) \cdot \frac{1}{D_i - N_i} \cdot (-1)]$
        
    -   Simplifies to: $+ \ln(D_i - N_i) + 1$
        

**Combine them:**

$$\frac{\partial \ln(\Omega_i)}{\partial N_i} = (- \ln(N_i) - 1) + (\ln(D_i - N_i) + 1)$$

The $-1$ and $+1$ cancel out!

We are left with:

$$\ln(D_i - N_i) - \ln(N_i)$$

Using log rules ($\ln A - \ln B = \ln(A/B)$), we get:

$$\ln\left(\frac{D_i - N_i}{N_i}\right) = \ln\left(\frac{D_i}{N_i} - 1\right)$$

---

### Step 4: The Final Entropy Derivative

The question asks for $\frac{\partial S}{\partial N_i}$.

Remember $S = k_B \sum_j \ln(\Omega_j)$.

When we differentiate a sum $\sum_j$ with respect to a specific variable $N_i$, all the terms where $j \neq i$ are constants (they don't depend on $N_i$), so their derivatives are zero. We only care about the term where $j=i$.

So:

$$\frac{\partial S}{\partial N_i} = k_B \frac{\partial \ln(\Omega_i)}{\partial N_i}$$

Substitute our result from Step 3:

$$\frac{\partial S}{\partial N_i} = k_B \ln\left(\frac{D_i}{N_i} - 1\right)$$

---

**Summary of Part c):**

We used Stirling's approximation to simplify the factorials, took the derivative carefully, and found that the change in entropy depends simply on the ratio of available seats ($D_i$) to people ($N_i$).

We now have all the puzzle pieces!

-   **Part a:** gave us the equilibrium condition $\mu = \frac{\partial F}{\partial N_i}$.
    
-   **Part b:** gave us the counting formula.
    
-   **Part c:** gave us the entropy change.
    

**Are you ready for the final step where we combine them to discover the famous Fermi-Dirac distribution?**