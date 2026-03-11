

This is a fantastic next question! We are moving from single-particle systems to multi-particle systems. This topic is called the "addition of angular momentum," and it is absolutely crucial for understanding real-world quantum mechanics, like how electrons behave in complex atoms.

First, let's translate the German text from your assignment:

- **"Ein System bestehe aus Teilchen 1 und 2 in Drehimpulseigenzuständen $(l_1, m_1)$ und $(l_2, m_2)$."** translates to **"A system consists of particles 1 and 2 in angular momentum eigenstates $(l_1, m_1)$ and $(l_2, m_2)$."**
    
- **"Ist das System aus beiden Teilchen ein Eigenzustand des Gesamtdrehimpulsquadrats $J^2$? Ist es ein Eigenzustand von $J_z$? Begründen Sie jeweils Ihre Antwort."** translates to **"Is the system composed of both particles an eigenstate of the total angular momentum squared $J^2$? Is it an eigenstate of $J_z$? Justify your answers in each case."**
    

Let's break this down. In quantum mechanics, when we combine two systems, the total state of the system is the "tensor product" of the individual states. We can write our combined state as:

$$| \psi \rangle = | l_1, m_1 \rangle \otimes | l_2, m_2 \rangle$$

For simplicity, we often just write this as a combined ket: $| l_1, m_1; l_2, m_2 \rangle$. This is known as the **uncoupled basis** because we are treating the two particles as independent, separate entities.

Now, let's test this state against our total angular momentum operators.

### 1. Is it an eigenstate of $\hat{J}_z$?

The total z-component of angular momentum, $\hat{J}_z$, is simply the sum of the z-components of the individual particles:

$$\hat{J}_z = \hat{L}_{1z} + \hat{L}_{2z}$$

Remember that an operator for particle 1 only acts on the state of particle 1, and the same goes for particle 2. Let's apply $\hat{J}_z$ to our combined state:

$$\hat{J}_z | l_1, m_1; l_2, m_2 \rangle = (\hat{L}_{1z} + \hat{L}_{2z}) | l_1, m_1; l_2, m_2 \rangle$$

Distributing the operator gives:

$$= (\hat{L}_{1z} | l_1, m_1 \rangle) \otimes | l_2, m_2 \rangle + | l_1, m_1 \rangle \otimes (\hat{L}_{2z} | l_2, m_2 \rangle)$$

Since we know $| l_1, m_1 \rangle$ is an eigenstate of $\hat{L}_{1z}$ with eigenvalue $m_1$ (assuming $\hbar = 1$ like in the previous problem), and similarly for particle 2, we get:

$$= (m_1 | l_1, m_1 \rangle) \otimes | l_2, m_2 \rangle + | l_1, m_1 \rangle \otimes (m_2 | l_2, m_2 \rangle)$$

$$= (m_1 + m_2) | l_1, m_1; l_2, m_2 \rangle$$

**Conclusion for $\hat{J}_z$:** **Yes**, the system is an eigenstate of $\hat{J}_z$. We applied the operator and got the exact same state back, multiplied by a constant scalar eigenvalue of $(m_1 + m_2)$.

---

### 2. Is it an eigenstate of $\hat{J}^2$?

This is where it gets tricky, and where the ladder operators from the previous question come in handy!

The total angular momentum squared operator is:

$$\hat{J}^2 = (\hat{\vec{L}}_1 + \hat{\vec{L}}_2) \cdot (\hat{\vec{L}}_1 + \hat{\vec{L}}_2)$$

If we expand this dot product, we get:

$$\hat{J}^2 = \hat{L}_1^2 + \hat{L}_2^2 + 2(\hat{\vec{L}}_1 \cdot \hat{\vec{L}}_2)$$

Let's expand that middle dot-product term into its $x, y$, and $z$ components:

$$\hat{J}^2 = \hat{L}_1^2 + \hat{L}_2^2 + 2(\hat{L}_{1z}\hat{L}_{2z} + \hat{L}_{1x}\hat{L}_{2x} + \hat{L}_{1y}\hat{L}_{2y})$$

Now, let's think about applying this massive operator to our uncoupled state $| l_1, m_1; l_2, m_2 \rangle$:

- **The "Good" Terms:** Our state is perfectly happy being acted on by $\hat{L}_1^2$, $\hat{L}_2^2$, and $\hat{L}_{1z}\hat{L}_{2z}$. These will all just spit out constant eigenvalues ($l_1(l_1+1)$, $l_2(l_2+1)$, and $m_1m_2$ respectively) and leave the state unchanged.
    
- **The "Problem" Terms:** The issue lies entirely with the $\hat{L}_{1x}\hat{L}_{2x} + \hat{L}_{1y}\hat{L}_{2y}$ piece.
    

In quantum mechanics, states with a definite $z$-component (definite $m$) do _not_ have a definite $x$ or $y$ component. If you recall the ladder operators we just discussed ($\hat{L}_\pm = \hat{L}_x \pm i\hat{L}_y$), we can rewrite those problem terms as:

$$\hat{L}_{1x}\hat{L}_{2x} + \hat{L}_{1y}\hat{L}_{2y} = \frac{1}{2}(\hat{L}_{1+}\hat{L}_{2-} + \hat{L}_{1-}\hat{L}_{2+})$$

Look at what happens when this acts on our state!

- The $\hat{L}_{1+}\hat{L}_{2-}$ term raises particle 1's $m$-value and lowers particle 2's $m$-value. It creates a _new_ state: proportional to $| l_1, m_1+1; l_2, m_2-1 \rangle$.
    
- The $\hat{L}_{1-}\hat{L}_{2+}$ term does the opposite, creating another _new_ state: proportional to $| l_1, m_1-1; l_2, m_2+1 \rangle$.
    

Because applying $\hat{J}^2$ changes the $m$ values and creates a superposition of different states, it does not return the original state multiplied by a constant.

**Conclusion for $\hat{J}^2$:**

**No**, in general, the uncoupled product state is _not_ an eigenstate of $\hat{J}^2$. (There is a small exception if you are at the absolute maximum or minimum possible values for $m_1$ and $m_2$ where the ladder operators annihilate the state, but generally speaking, the answer is no).

---

To find the true eigenstates of $\hat{J}^2$, we have to mathematically mix these uncoupled states together into what we call the "coupled basis."

Would you like me to briefly explain how we use Clebsch-Gordan coefficients to build those coupled eigenstates?