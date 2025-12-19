

That is the spirit of a true theoretical physicist! When our math contradicts physical reality, we don't ignore it—we find the missing piece of the puzzle.

To fix the **Gibbs Paradox**, we have to fundamentally change how we count "states" in nature.

### 1. The Diagnosis: What went wrong?

In our previous derivation (Part a), we implicitly assumed the particles were **distinguishable**. Imagine we had two particles, Alice and Bob.

-   **State A:** Alice is in the left corner, Bob is in the right corner.
    
-   **State B:** Bob is in the left corner, Alice is in the right corner.
    

In classical mechanics, State A and State B are different. We counted them as two separate possibilities.

But for atoms (like Helium), "Alice" and "Bob" don't exist. There is just "an atom" and "an atom." If you swap them, the universe looks exactly the same.

-   **Quantum Reality:** State A and State B are the **same** physical state.
    

**The Error:** We overcounted the number of possible states! For $N$ particles, there are $N!$ (N factorial) ways to swap labels (permutations). We counted all of them, but we should have only counted one.

---

### 2. The Cure: The Indistinguishability Factor

To fix the entropy, we need to divide the number of microstates ($\Omega$) by $N!$.

Since Entropy is $S = k_B \ln(\Omega)$, dividing $\Omega$ by $N!$ corresponds to subtracting a logarithm:

$$S_{\text{corrected}} = S_{\text{original}} - k_B \ln(N!)$$

#### The Stirling Approximation

For typical gas quantities (like $10^{23}$ particles), $N$ is huge. We can use Stirling's Approximation:

$$\ln(N!) \approx N \ln(N) - N$$

Let's apply this "patch" to our result from **(2.a)**.

Original (Flawed) Entropy:

$$S \approx N k_B \ln(V) + \text{Terms}(T)$$

Corrected Entropy:

$$S_{new} = \left[ N k_B \ln(V) + \text{Terms}(T) \right] - k_B (N \ln N - N)$$

Let's group the terms with logarithms together:

$$S_{new} = N k_B \left( \ln(V) - \ln(N) \right) + \text{Terms}(T) + N k_B$$

Using log rules ($\ln A - \ln B = \ln(A/B)$), we get the magic fix:

> $$S_{new} = N k_B \ln\left( \frac{V}{N} \right) + \dots$$

Why is this brilliant?

Instead of depending on Volume ($V$), the entropy now depends on the Specific Volume ($V/N$, or the volume per particle).

-   If you double the size of the box ($2V$) and the number of particles ($2N$), the ratio $\frac{2V}{2N}$ stays the same. The term inside the log doesn't change! This makes Entropy properly **extensive** (additive).
    

---

### 3. Re-Solving Part (2.b) with the Fix

Now, let's re-calculate the mixing of two identical gases using our new formula.

**Recall the Setup:**

-   Gas 1: $N_1, V_1$
    
-   Gas 2: $N_2, V_2$
    
-   We assume equal pressure and temperature, so the density is uniform: $\frac{V_1}{N_1} = \frac{V_2}{N_2} = \frac{V_{total}}{N_{total}} = v$ (constant specific volume).
    

#### Step 1: Initial Entropy ($S_{anf}$)

$$S_{anf} = S_1 + S_2$$

$$S_{anf} = \left[ N_1 k_B \ln\left(\frac{V_1}{N_1}\right) + \dots \right] + \left[ N_2 k_B \ln\left(\frac{V_2}{N_2}\right) + \dots \right]$$

Since $\frac{V_1}{N_1} = v$ and $\frac{V_2}{N_2} = v$, this simplifies nicely:

$$S_{anf} = (N_1 + N_2) k_B \ln(v) + \dots$$

#### Step 2: Final Entropy ($S_{end}$)

Now they are mixed. Total $N = N_1+N_2$, Total $V = V_1+V_2$.

$$S_{end} = (N_1+N_2) k_B \ln\left(\frac{V_1+V_2}{N_1+N_2}\right) + \dots$$

Notice that $\frac{V_1+V_2}{N_1+N_2}$ is also just equal to $v$!

$$S_{end} = (N_1+N_2) k_B \ln(v) + \dots$$

#### Step 3: The Difference

$$\Delta S = S_{end} - S_{anf} = 0$$

Victory!

For identical gases, the entropy of mixing is exactly zero. By treating the particles as indistinguishable (adding the $1/N!$ factor), we have resolved the Gibbs Paradox.

### Summary for your notes

This corrected equation (when fully written out with all constants) is known as the **Sackur-Tetrode Equation**. It is one of the most beautiful results in statistical mechanics because it uses Quantum Mechanics (indistinguishability) to fix a problem in Classical Thermodynamics.

**Would you like to try a specific example, like mixing different gases (e.g., Argon and Neon), to see how the entropy behaves then?**