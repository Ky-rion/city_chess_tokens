

![[Pasted image 20260209163602.png]]

That is the spirit! Let's continue our journey into the subatomic world.

In **Part (a)**, we smashed an electron and a positron together to create a heavy particle called the **$\Upsilon(4S)$ meson** (pronounced "Upsilon 4-S"). We found that the "available energy" or "Center-of-Mass energy" ($\sqrt{s}$) was **10.583 GeV**.

Now, in **Part (b)**, we are looking at what happens immediately after that collision. The $\Upsilon(4S)$ is unstable and decays almost instantly into two other particles: a **$B$-meson** and an **anti-$B$-meson** ($\bar{B}$).

We need to find out how fast these new $B$-mesons are moving.

---

### 1. The Physics Picture: Two-Body Decay

Imagine the $\Upsilon(4S)$ as a heavy ball sitting perfectly still in the center of our frame (because we are in the Center-of-Mass system). It suddenly splits into two equal pieces ($B$ and $\bar{B}$).

Because momentum must be conserved:

- Before the split, the momentum was zero (the $\Upsilon(4S)$ was at rest).
    
- After the split, the total momentum must still be zero.
    

This implies the two new particles must fly apart back-to-back with **equal and opposite momentum**. This is why the solution starts with:

$$\vec{p}_B = -\vec{p}_{\bar{B}}$$

We just call the magnitude of this momentum $|\vec{p}|$.

### 2. Conservation of Energy

Now we use the **Conservation of Energy**. The energy of the parent particle ($\sqrt{s}$) must equal the sum of the energies of the two daughter particles.

$$E_{parent} = E_B + E_{\bar{B}}$$

Since the $B$ and $\bar{B}$ have the same mass ($m_B$) and the same momentum magnitude ($|\vec{p}|$), they must have exactly the same energy. So we can just say:

$$\sqrt{s} = 2 \times E_B$$

Recall the relativistic energy formula ($E = \sqrt{m^2 + p^2}$). Substituting that in gives us the equation shown in the solution:

$$\sqrt{s} = 2 \sqrt{m_B^2 + \vec{p}^2}$$

### 3. Solving for Momentum ($|\vec{p}|$)

Now we just need to do some algebra to isolate $|\vec{p}|$.

1. **Divide by 2:**
    
    $$\frac{\sqrt{s}}{2} = \sqrt{m_B^2 + \vec{p}^2}$$
    
2. **Square both sides:**
    
    $$\frac{s}{4} = m_B^2 + \vec{p}^2$$
    
3. **Subtract the mass squared ($m_B^2$):**
    
    $$\vec{p}^2 = \frac{s}{4} - m_B^2$$
    
4. **Take the square root:**
    
    $$|\vec{p}| = \sqrt{\frac{s}{4} - m_B^2}$$
    

**Plugging in the numbers:**

- From Part (a), $\sqrt{s} = 10.583 \text{ GeV}$ (so $s \approx 112$).
    
- From the text in Part (a), the mass of a $B$-meson is $m_B = 5.28 \text{ GeV}/c^2$.
    

$$|\vec{p}| = \sqrt{\left(\frac{10.583}{2}\right)^2 - (5.28)^2}$$

$$|\vec{p}| = \sqrt{(5.2915)^2 - (5.28)^2}$$

Notice how close these two numbers are! $5.29$ vs $5.28$. The total available energy is _barely_ enough to create these two particles. There is very little "leftover" energy to turn into speed.

$$|\vec{p}| \approx 0.349 \text{ GeV}/c$$

This matches the solution exactly.

---

### 4. The Speed Factor ($\beta\gamma$)

The second half of the question asks us to calculate $\beta\gamma$ (beta-gamma) and show it is much less than 1 ($\ll 1$).

**What is $\beta\gamma$?**

In relativity:

- $\beta = v/c$ (How fast you are going as a fraction of light speed).
    
- $\gamma = \frac{1}{\sqrt{1-\beta^2}}$ (The Lorentz factor).
    

A handy identity in particle physics is:

$$\beta\gamma = \frac{\text{Momentum}}{\text{Mass}} = \frac{p}{m}$$

**The Calculation:**

Using our momentum result ($0.349$) and the mass ($5.28$):

$$\beta\gamma = \frac{0.349}{5.28} \approx \mathbf{0.066}$$

**The Interpretation:**

Since $0.066$ is much smaller than $1$, this proves that the $B$-mesons are moving **very slowly** (non-relativistically) in the Center-of-Mass frame.

**Why do we care?**

The question states: _"Based on this... it will be assumed that the B-mesons are at rest."_

Because they are moving so slowly, for the next parts of the calculation, we can simplify our lives by pretending they are just sitting still. This is a very common approximation in physics: if a number is small enough, treat it as zero!

Ready for the next part? I suspect we might have to deal with that magnetic field mentioned in the first text soon!