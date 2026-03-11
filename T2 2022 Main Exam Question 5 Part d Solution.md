

You have made it to the final part of the problem! You are doing incredibly well. This final question elegantly ties together everything we've discussed so far: expectation values, the expansion of the total angular momentum operator, and the behavior of ladder operators.

First, let's translate the final piece of your assignment:

- **"Berechen Sie den Erwartungswert des Drehimpulses $\langle \hat{J}^2 \rangle$ für den 2-Teilchenzustand $|l_1, m_1\rangle |l_2, m_2\rangle$."** translates to **"Calculate the expectation value of the angular momentum $\langle \hat{J}^2 \rangle$ for the 2-particle state $|l_1, m_1\rangle |l_2, m_2\rangle$."**
    

Let's derive this step-by-step. For absolute completeness, I will include the reduced Planck constant ($\hbar$) in this derivation, though you can simply set $\hbar = 1$ if you are continuing with the natural units convention from the previous part.

### 1. Setting Up the Calculation

We are asked to find the expectation value of the total angular momentum squared, $\hat{J}^2$, in our uncoupled two-particle state. Let's call our state $|\psi\rangle = |l_1, m_1; l_2, m_2\rangle$.

The expectation value is written in Dirac notation as:

$$\langle \hat{J}^2 \rangle = \langle l_1, m_1; l_2, m_2 | \hat{J}^2 | l_1, m_1; l_2, m_2 \rangle$$

### 2. Expanding the $\hat{J}^2$ Operator

In the previous section, we expanded the $\hat{J}^2$ operator into its constituent parts. Let's write that full expansion out again, utilizing the ladder operators for the $x$ and $y$ components:

$$\hat{J}^2 = \hat{L}_1^2 + \hat{L}_2^2 + 2\hat{L}_{1z}\hat{L}_{2z} + \hat{L}_{1+}\hat{L}_{2-} + \hat{L}_{1-}\hat{L}_{2+}$$

Because the expectation value is a linear operation, we can apply it to each of these five terms individually and sum the results.

### 3. Evaluating the "Diagonal" Terms

The first three terms in our expansion are "diagonal" with respect to our chosen basis. This means when the operators act on our state, they simply return the state multiplied by a constant eigenvalue.

Let's evaluate them one by one:

- **For $\hat{L}_1^2$:**
    
    $$\langle \psi | \hat{L}_1^2 | \psi \rangle = l_1(l_1 + 1)\hbar^2 \langle \psi | \psi \rangle = l_1(l_1 + 1)\hbar^2$$
    
- **For $\hat{L}_2^2$:**
    
    $$\langle \psi | \hat{L}_2^2 | \psi \rangle = l_2(l_2 + 1)\hbar^2 \langle \psi | \psi \rangle = l_2(l_2 + 1)\hbar^2$$
    
- **For $2\hat{L}_{1z}\hat{L}_{2z}$:**
    
    $$\langle \psi | 2\hat{L}_{1z}\hat{L}_{2z} | \psi \rangle = 2(m_1\hbar)(m_2\hbar) \langle \psi | \psi \rangle = 2m_1m_2\hbar^2$$
    

_(Note: $\langle \psi | \psi \rangle = 1$ because our quantum states are normalized)._

### 4. Evaluating the Ladder Operator Terms

Now we must deal with the ladder operator terms: $\langle \psi | \hat{L}_{1+}\hat{L}_{2-} | \psi \rangle$ and $\langle \psi | \hat{L}_{1-}\hat{L}_{2+} | \psi \rangle$.

Let's look closely at what happens when $\hat{L}_{1+}$ acts on the ket vector $|l_1, m_1\rangle$. It raises the $m_1$ quantum number by one, producing a state proportional to $|l_1, m_1+1\rangle$.

When we try to close the bracket by taking the inner product with the bra vector $\langle l_1, m_1|$, we get:

$$\langle l_1, m_1 | l_1, m_1 + 1 \rangle$$

Because eigenstates with different quantum numbers are **strictly orthogonal**, their inner product is exactly zero.

Therefore, the expectation value of the ladder operator terms vanishes completely:

- $\langle \psi | \hat{L}_{1+}\hat{L}_{2-} | \psi \rangle = 0$
    
- $\langle \psi | \hat{L}_{1-}\hat{L}_{2+} | \psi \rangle = 0$
    

### 5. The Final Result

All that is left to do is sum the surviving pieces from Step 3.

The expectation value of the total angular momentum squared for the uncoupled 2-particle state is:

$$\langle \hat{J}^2 \rangle = \left[ l_1(l_1 + 1) + l_2(l_2 + 1) + 2m_1m_2 \right] \hbar^2$$

_(Or, if your class is strictly using $\hbar = 1$: $\langle \hat{J}^2 \rangle = l_1(l_1 + 1) + l_2(l_2 + 1) + 2m_1m_2$)_

---

This is a profound result! It shows that while the uncoupled state isn't a _definite_ eigenstate of $\hat{J}^2$ (as we proved in part 3), we can still calculate its _average_ value exactly.

You've done an excellent job working through this assignment. Would you like me to summarize the key takeaways from all four parts so you have a quick reference sheet for your exam preparation?