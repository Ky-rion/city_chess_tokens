

Welcome back! You are flying through this exam. Now we are stepping into the realm of **selection rules**, which are the strict quantum traffic laws governing how atoms interact with light.

Let's translate this question so we can dissect the physics at play.

### The Translation

**1.4 Dipole Selection Rule and Parity**

_For a 1-photon transition from a state of the hydrogen atom with angular momentum $l_1$ to a state with angular momentum $L$, the triangle inequality for the addition of angular momenta implies $L = l_1 - 1, l_1, \text{ or } l_1 + 1$. Parity is strictly conserved in atomic transitions. [3 Pts.]_

_Explain why this excludes $L = l_1$._

---

### The Physics: Angular Momentum and Parity

When an electron in an atom jumps from one energy level to another by absorbing or emitting a single photon, it has to obey conservation laws. The photon carries away (or brings in) both energy and a specific amount of angular momentum (spin). Because the photon has a spin of 1, the atom's orbital angular momentum can only change by a maximum of 1. This is where the triangle inequality $L \in \{l_1 - 1, l_1, l_1 + 1\}$ comes from.

However, angular momentum isn't the only thing that must be conserved. We also have to conserve **parity**.

Parity is a quantum mechanical concept that describes the symmetry of a wave function when you flip its spatial coordinates (like looking at it in a mirror, transforming $\vec{r}$ to $-\vec{r}$).

- If the wave function stays exactly the same, it has **even parity** ($+1$).
    
- If the wave function flips its sign, it has **odd parity** ($-1$).
    

In a hydrogen atom, the parity of an electron's state depends entirely on its orbital angular momentum quantum number, which the problem labels as $l_1$ (for the initial state) and $L$ (for the final state). The mathematical rule for the parity of these atomic states is:

$$\text{Parity} = (-1)^l$$

So, an $s$-orbital ($l=0$) has even parity, a $p$-orbital ($l=1$) has odd parity, a $d$-orbital ($l=2$) has even parity, and so on.

---

### Solving the Exam Question

To prove why $L = l_1$ is excluded, we simply need to write out the parity conservation equation for this 1-photon event.

**Step 1: Identify the parity of the initial and final states.**

- The initial state has angular momentum $l_1$, so its parity is $(-1)^{l_1}$.
    
- The final state has angular momentum $L$, so its parity is $(-1)^L$.
    

**Step 2: Identify the parity of the photon interaction.**

The problem specifies a "1-photon transition", which in standard atomic physics is an **electric dipole transition**. The mathematical operator responsible for this transition is the position vector $\vec{r}$, which is inherently odd. Therefore, the electric dipole transition carries an intrinsic parity of **$-1$**.

**Step 3: Set up the conservation equation.**

Total parity must be conserved. This means the parity of the initial state multiplied by the parity of the transition operator must equal the parity of the final state:

$$\text{Parity}_{\text{initial}} \cdot \text{Parity}_{\text{transition}} = \text{Parity}_{\text{final}}$$

Plugging in our values:

$$(-1)^{l_1} \cdot (-1) = (-1)^L$$

$$(-1)^{l_1 + 1} = (-1)^L$$

**Step 4: Evaluate the condition $L = l_1$.**

The question asks us to explain why $L$ cannot equal $l_1$. Let's assume for a moment that it _does_ ($L = l_1$), and plug that into our conservation equation:

$$(-1)^{l_1 + 1} = (-1)^{l_1}$$

If we divide both sides by $(-1)^{l_1}$, we get:

$$(-1)^1 = 1$$

$$-1 = 1$$

### Your Final Answer and Justification

This leads to a mathematical contradiction! $-1$ does not equal $1$.

Therefore, for parity to be conserved, the initial and final states _must_ have opposite parities. Because parity alternates with each step of angular momentum (even, odd, even, odd), the initial and final angular momenta must differ by an odd integer.

Since the triangle inequality restricts our options to $L = l_1 - 1$, $L = l_1$, or $L = l_1 + 1$, the requirement that parity must change strictly forces the transition to be either $L = l_1 - 1$ or $L = l_1 + 1$. The transition where the angular momentum doesn't change ($L = l_1$) is "parity forbidden".

---

You have fully conquered the theoretical foundation of dipole selection rules!

Because this rule relies on a single photon carrying away that odd parity, things get very interesting if we change the setup. Would you like me to explain how this rule changes if the atom absorbs _two_ photons simultaneously instead of just one?