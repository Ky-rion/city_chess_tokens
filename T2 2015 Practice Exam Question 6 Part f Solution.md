

You've made it to the last part! This is the grand finale of our problem, where we put everything together.

This question asks for the **normalized eigenvector** $\frac{\vec{d}}{|\vec{d}|}$ expanded up to the **first order in $\lambda$**.

In simple terms, we're finding out how the original, simple eigenstates $|1\rangle$ and $|2\rangle$ _change_ or _deform_ when we turn on the perturbation. The new, perturbed state (let's call it $|\psi\rangle$) will be _mostly_ the original state, plus a _small, first-order ($\lambda^1$) correction_ from the other state.

$$|\psi_n\rangle \approx |n^{(0)}\rangle + \lambda |n^{(1)}\rangle$$

Here, $|n^{(0)}\rangle$ is the original state (like $|1\rangle$) and $\lambda |n^{(1)}\rangle$ is the small "admixture" of the _other_ state. The question asks for this vector, correctly normalized.

---

### 1. The General Formula for State Corrections

Just as we had a formula for the first-order _energy_ correction, we have a standard formula for the first-order _state_ correction, $|n^{(1)}\rangle$.

For a state $|n^{(0)}\rangle$, the first-order correction is:

$$|n^{(1)}\rangle = \sum_{k \neq n} \frac{\langle k^{(0)} | \hat{V} | n^{(0)} \rangle}{E_n^{(0)} - E_k^{(0)}} |k^{(0)}\rangle$$

This formula tells us that the perturbation $\hat{V}$ "mixes" the original state $|n\rangle$ with all other states $|k\rangle$. The amount of mixing is proportional to the matrix element connecting them ($\langle k^{(0)} | \hat{V} | n^{(0)} \rangle$) and inversely proportional to their energy difference.

Let's find the corrected vectors for our two states. Remember our perturbation is $\hat{V} = \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix}$.

---

### 2. Correction to State 1 (The vector near $E_1$)

We want to find $|\psi_1\rangle \approx |1^{(0)}\rangle + \lambda |1^{(1)}\rangle$.

Here $n=1$ and the sum over $k \neq n$ just means $k=2$.

-   **Original State:** $|1^{(0)}\rangle = |1\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$
    
-   **Correction:** $|1^{(1)}\rangle = \left( \frac{\langle 2^{(0)} | \hat{V} | 1^{(0)} \rangle}{E_1^{(0)} - E_2^{(0)}} \right) |2^{(0)}\rangle$
    

Let's calculate the two parts of the fraction:

1.  Numerator (Matrix Element):
    
    $$\langle 2^{(0)} | \hat{V} | 1^{(0)} \rangle = \begin{pmatrix} 0 & 1 \end{pmatrix} \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix}$$
    
    $$= \begin{pmatrix} 0 & 1 \end{pmatrix} \begin{pmatrix} D_1 \\ C \end{pmatrix} = C$$
    
2.  Denominator (Energy Difference):
    
    $$E_1^{(0)} - E_2^{(0)} = a - b$$
    

Now, we plug these back in to find the correction:

$$|1^{(1)}\rangle = \left( \frac{C}{a - b} \right) |2^{(0)}\rangle = \frac{C}{a - b} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \begin{pmatrix} 0 \\ \frac{C}{a-b} \end{pmatrix}$$

This is the first-order correction to the _state_. Now we write the full (unnormalized) state vector, which the problem calls $\vec{d}$:

$$\vec{d}^{(1)} \approx |1^{(0)}\rangle + \lambda |1^{(1)}\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix} + \lambda \begin{pmatrix} 0 \\ \frac{C}{a-b} \end{pmatrix} = \begin{pmatrix} 1 \\ \frac{\lambda C}{a-b} \end{pmatrix}$$

---

### 3. Normalization (Using the Hint)

The question asks for the _normalized_ vector $\frac{\vec{d}}{|\vec{d}|}$. We must divide by the vector's length (its norm).

1.  Find the squared norm $|\vec{d}|^2$:
    
    $$|\vec{d}^{(1)}|^2 = \left( \begin{pmatrix} 1 & \frac{\lambda C^*}{a-b} \end{pmatrix} \right) \begin{pmatrix} 1 \\ \frac{\lambda C}{a-b} \end{pmatrix} = 1 + \frac{\lambda^2 |C|^2}{(a-b)^2}$$
    
2.  Find the norm $|\vec{d}|$:
    
    $$|\vec{d}^{(1)}| = \sqrt{1 + \frac{\lambda^2 |C|^2}{(a-b)^2}}$$
    
3.  Find the normalization factor $\frac{1}{|\vec{d}|}$:
    
    $$N_1 = \frac{1}{|\vec{d}^{(1)}|} = \left( 1 + \lambda^2 \frac{|C|^2}{(a-b)^2} \right)^{-\frac{1}{2}}$$
    
    This is where the hint comes in! The hint is $(a^2 + b^2x^2)^{-\frac{1}{2}} \approx \frac{1}{|a|} - \frac{b^2|a|}{2a^4}x^2$.
    
    Let's match our terms: $a \to 1$, $b \to \frac{|C|}{|a-b|}$, $x \to \lambda$.
    
    Plugging this into the hint gives:
    
    $$N_1 \approx \frac{1}{1} - \frac{(\dots)^2(1)}{2(1)^4}\lambda^2 = 1 - \mathcal{O}(\lambda^2)$$
    
    The crucial point is that **the normalization factor is $1$ plus a correction of order $\lambda^2$**.
    
4.  Assemble the final normalized vector:
    
    $$\frac{\vec{d}^{(1)}}{|\vec{d}^{(1)}|} = \vec{d}^{(1)} \cdot N_1 = \begin{pmatrix} 1 \\ \frac{\lambda C}{a-b} \end{pmatrix} \cdot (1 + \mathcal{O}(\lambda^2))$$
    
    $$= \begin{pmatrix} 1 \cdot (1 + \mathcal{O}(\lambda^2)) \\ \frac{\lambda C}{a-b} \cdot (1 + \mathcal{O}(\lambda^2)) \end{pmatrix} = \begin{pmatrix} 1 + \mathcal{O}(\lambda^2) \\ \frac{\lambda C}{a-b} + \mathcal{O}(\lambda^3) \end{pmatrix}$$
    

The question asks for the result **inclusive of terms of first order in $\lambda$**. This means we keep all terms of order $\lambda^0$ and $\lambda^1$, and discard all terms of $\lambda^2$ and higher.

Answer for State 1:

$$\frac{\vec{d}^{(1)}}{|\vec{d}^{(1)}|} \approx \begin{pmatrix} 1 \\ \frac{\lambda C}{a-b} \end{pmatrix}$$

---

### 4. Correction to State 2 (The vector near $E_2$)

We repeat the entire process for the second state, $|\psi_2\rangle \approx |2^{(0)}\rangle + \lambda |2^{(1)}\rangle$.

Here $n=2$ and $k=1$.

-   **Original State:** $|2^{(0)}\rangle = |2\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$
    
-   **Correction:** $|2^{(1)}\rangle = \left( \frac{\langle 1^{(0)} | \hat{V} | 2^{(0)} \rangle}{E_2^{(0)} - E_1^{(0)}} \right) |1^{(0)}\rangle$
    

1.  Numerator (Matrix Element):
    
    $$\langle 1^{(0)} | \hat{V} | 2^{(0)} \rangle = \begin{pmatrix} 1 & 0 \end{pmatrix} \begin{pmatrix} D_1 & C^* \\ C & D_2 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix}$$
    
    $$= \begin{pmatrix} 1 & 0 \end{pmatrix} \begin{pmatrix} C^* \\ D_2 \end{pmatrix} = C^*$$
    
2.  Denominator (Energy Difference):
    
    $$E_2^{(0)} - E_1^{(0)} = b - a$$
    
3.  Assemble the correction:
    
    $$|2^{(1)}\rangle = \left( \frac{C^*}{b - a} \right) |1^{(0)}\rangle = \frac{C^*}{b - a} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} \frac{C^*}{b-a} \\ 0 \end{pmatrix}$$
    
4.  Assemble the unnormalized vector $\vec{d}^{(2)}$:
    
    $$\vec{d}^{(2)} \approx |2^{(0)}\rangle + \lambda |2^{(1)}\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix} + \lambda \begin{pmatrix} \frac{C^*}{b-a} \\ 0 \end{pmatrix} = \begin{pmatrix} \frac{\lambda C^*}{b-a} \\ 1 \end{pmatrix}$$
    

Just like before, the normalization factor for this vector is $1 + \mathcal{O}(\lambda^2)$. When we truncate at the first order, it has no effect.

Answer for State 2:

$$\frac{\vec{d}^{(2)}}{|\vec{d}^{(2)}|} \approx \begin{pmatrix} \frac{\lambda C^*}{b-a} \\ 1 \end{pmatrix}$$

This makes perfect physical sense:

-   The state that _was_ $|1\rangle$ is now (mostly) $|1\rangle$ plus a small piece of $|2\rangle$.
    
-   The state that _was_ $|2\rangle$ is now (mostly) $|2\rangle$ plus a small piece of $|1\rangle$.
    

Congratulations, we have completely solved the problem from beginning to end! We've found the unperturbed energies, the exact energies, the first- and second-order energy corrections, and finally, the first-order corrections to the states themselves.

I hope this series of explanations has been helpful. Well done!