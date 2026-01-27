

![[Pasted image 20260125190625.png]]

Welcome to the grand finale! We have successfully built all the components, and now in **Part d)**, we just need to assemble them to reveal one of the most important equations in all of solid-state physics: the **Fermi-Dirac Distribution**.

Let's walk through the algebra and the logic step-by-step.

### 1. Assembling the Pieces

First, let's look at the equation provided in the problem statement. It combines everything we have done so far:

$$\mu = \frac{\partial F}{\partial N_i} = \frac{\partial E}{\partial N_i} - T \frac{\partial S}{\partial N_i}$$

Let's break down where each term comes from:

-   **$\mu$**: From **Part a)**, we know this is the condition for equilibrium.
    
-   **$\frac{\partial E}{\partial N_i} = E_i$**: This is new but simple. If you add _one_ fermion to energy level $i$, the total energy of the system increases exactly by the energy of that level, $E_i$.
    
-   **$\frac{\partial S}{\partial N_i}$**: From **Part c)**, we calculated this as $k_B \ln(D_i/N_i - 1)$.
    

Substituting these into the main equation gives us the starting point shown in your image:

$$\mu = E_i - k_B T \ln\left(\frac{D_i}{N_i} - 1\right)$$

---

### 2. The Algebraic "Shuffle"

The goal is to solve for the "occupation probability" or "filling factor," which is defined as the ratio of filled seats to total seats:

$$f_i = \frac{N_i}{D_i}$$

We need to isolate $N_i/D_i$ from inside that logarithm. Let's follow the solution's steps.

**Step 1: Isolate the Logarithm**

Move $E_i$ to the left side:

$$\mu - E_i = - k_B T \ln\left(\frac{D_i}{N_i} - 1\right)$$

Divide by $-k_B T$ (which flips the signs on the left):

$$\frac{E_i - \mu}{k_B T} = \ln\left(\frac{D_i}{N_i} - 1\right)$$

**Step 2: Exponentiate**

To kill the natural log ($\ln$), we take the exponential ($e$) of both sides:

$$e^{\frac{E_i - \mu}{k_B T}} = \frac{D_i}{N_i} - 1$$

**Step 3: Solve for the Ratio**

Add 1 to both sides:

$$\frac{D_i}{N_i} = e^{\frac{E_i - \mu}{k_B T}} + 1$$

Now, notice that we have $\frac{D_i}{N_i}$ (Total Seats / People), but we want $f_i = \frac{N_i}{D_i}$ (People / Total Seats). So, we just flip (invert) the entire fraction:

$$f_i = \frac{N_i}{D_i} = \frac{1}{e^{\frac{E_i - \mu}{k_B T}} + 1}$$

---

### 3. The Result: The Fermi-Dirac Distribution

Congratulations! You have just derived the **Fermi-Dirac Statistics**:

$$f(E) = \frac{1}{e^{\frac{E - \mu}{k_B T}} + 1}$$

**What does this actually tell us?**

This formula $f_i$ (or $f(E)$) tells you the **probability** (from 0 to 1) that a quantum state at energy $E$ is occupied by an electron at temperature $T$.

-   **At Absolute Zero ($T=0$):**
    
    -   If $E < \mu$: The exponential term becomes $e^{-\infty} = 0$. The probability is $1/(0+1) = 1$. The state is **full**.
        
    -   If $E > \mu$: The exponential term becomes $e^{+\infty} = \text{huge}$. The probability is $1/\text{huge} \approx 0$. The state is **empty**.
        
    -   This creates a sharp "step" where all low energy states are filled and all high energy states are empty.
        
-   **At Higher Temperatures ($T>0$):**
    
    -   Thermal energy "smears" this step out. Some electrons near the boundary jump up to higher energy levels, creating the smooth curve characteristic of semiconductors and metals.
        

### Final Summary

You have walked the entire path:

1.  **Part a:** Understood that $\mu$ balances Energy vs. Entropy.
    
2.  **Part b:** Counted the ways to arrange particles (Combinatorics).
    
3.  **Part c:** Connected counting to Entropy using Stirling's approximation.
    
4.  **Part d:** Combined it all to find the distribution function.
    

This derivation is the bedrock of understanding how computer chips, lasers, and metals work. Great job sticking with it!

**Would you like me to create a quick summary sheet of all the formulas we derived for your revision notes?**