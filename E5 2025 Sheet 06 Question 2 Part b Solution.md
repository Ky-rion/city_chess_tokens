

![[Pasted image 20260128115728.png]]

Welcome back to class! You have done the hard work of setting up the vectors. Now, we are going to use them to predict reality.

In this section, we are going to do three things:

1.  **Derive** a famous formula that tells us how much energy the electron keeps after hitting the proton.
    
2.  **Calculate** the "hardness" of the collision (the momentum transfer, $Q^2$).
    
3.  **Understand** the Bjorken variable $x$—a concept that will become crucial later when we start breaking protons apart!
    

Let's look at the solution provided in your image and break it down step-by-step.

---

### 1. Deriving the Scattered Energy $E'$

The goal is to find $E'$ (the outgoing electron energy) using only the things we know: the incoming energy $E$, the scattering angle $\theta$, and the proton mass $M$.

**The Physics Principle:** Conservation of Four-Momentum.

$$p + P = p' + P'$$

_(Incoming Electron + Resting Proton = Outgoing Electron + Recoiling Proton)_

**The "Professor's Trick" (Derivation):**

The standard way to solve these problems is to isolate the variable we _don't_ know and _don't_ care about—which is the recoiling proton $P'$—and square it to get rid of it.

1.  Rearrange the conservation equation to isolate $P'$:
    
    $$P + p - p' = P'$$
    
2.  Square both sides (take the dot product with themselves):
    
    $$(P + p - p')^2 = (P')^2$$
    
3.  Recall that the square of any four-momentum is the particle's mass squared ($P^2 = M^2c^2$).
    
    $$(P + p - p')^2 = M^2c^2$$
    

Now, expand the left side. Remember that $2AB$ in four-vectors means $2(E_A E_B - \vec{A}\cdot\vec{B})$.

$$P^2 + p^2 + p'^2 + 2(p \cdot P) - 2(p \cdot p') - 2(P \cdot p') = M^2c^2$$

We can simplify this significantly using our knowns:

-   $P^2 = M^2c^2$ and $p^2 \approx 0$ (electron is massless).
    
-   $p'^2 \approx 0$ (outgoing electron is massless).
    
-   The $M^2c^2$ on the right cancels with the $P^2$ on the left.
    

We are left with:

$$2(p \cdot P) - 2(p \cdot p') - 2(P \cdot p') = 0$$

Divide by 2 and rearrange:

$$(p \cdot P) - (p' \cdot P) = (p \cdot p')$$

$$P \cdot (p - p') = p \cdot p'$$

Now, let's plug in the actual vector components we defined in Part (a):

-   **Left Side ($P \cdot (p - p')$):**
    
    Since the proton is at rest, $P = (Mc, 0, 0, 0)$. It only has an energy component.
    
    $P \cdot (p - p') = Mc \times (\frac{E}{c} - \frac{E'}{c}) = M(E - E')$.
    
-   **Right Side ($p \cdot p'$):**
    
    $p \cdot p' = \frac{E}{c}\frac{E'}{c} - \vec{k} \cdot \vec{p}'$.
    
    Using the dot product formula $\vec{A}\cdot\vec{B} = |A||B|\cos\theta$:
    
    $p \cdot p' = \frac{EE'}{c^2} - \frac{EE'}{c^2}\cos\theta = \frac{EE'}{c^2}(1 - \cos\theta)$.
    

Set them equal:

$$M(E - E') = \frac{EE'}{c^2}(1 - \cos\theta)$$

Now, just algebra to solve for $E'$:

$$ME - ME' = \frac{E E'}{c^2}(1 - \cos\theta)$$

$$ME = ME' + E' \left[ \frac{E}{c^2}(1 - \cos\theta) \right]$$

$$ME = E' \left[ M + \frac{E}{c^2}(1 - \cos\theta) \right]$$

Divide by the bracket term:

$$E' = \frac{ME}{M + \frac{E}{c^2}(1 - \cos\theta)}$$

Finally, divide the top and bottom by $M$ to match the formula in your image:

$$E' = \frac{E}{1 + \frac{E}{Mc^2}(1 - \cos\theta)}$$

---

### 2. Calculating the Values

Now we plug in our numbers.

-   $E = 25 \text{ GeV}$
    
-   $\theta = 10^\circ$
    
-   $m_p c^2 = 0.938 \text{ GeV}$ (Note: Keep units consistent! $938 \text{ MeV}$ is $0.938 \text{ GeV}$)
    

**Step A: Calculate the denominator term**

$$\cos(10^\circ) \approx 0.9848$$

$$1 - \cos(10^\circ) = 0.0152$$

$$\frac{E}{m_p c^2} = \frac{25}{0.938} = 26.65$$

$$Term = 26.65 \times 0.0152 \approx 0.405$$

**Step B: Calculate Energy $E'$**

$$E' = \frac{25}{1 + 0.405} = \frac{25}{1.405} \approx 17.79 \text{ GeV}$$

The solution provided lists **17.8 GeV**. We have a match!

---

### 3. The Momentum Transfer $Q^2$

**What is it?**

$Q^2$ is the "squared four-momentum transfer." It tells us how hard the electron hit the proton. A higher $Q^2$ means the electron probed deeper into the proton (seeing smaller details).

**The Formula:**

We defined $Q^2 = -q^2 = -(p - p')^2$.

From our earlier derivation, we found that $(p - p')^2 = -2(p \cdot p')$.

So:

$$Q^2 = 2(p \cdot p') = 2 \frac{E E'}{c^2} (1 - \cos\theta)$$

**The Calculation:**

$$Q^2 = 2 \times 25 \times 17.8 \times (1 - 0.9848)$$

$$Q^2 = 890 \times 0.0152 \approx 13.5 \text{ GeV}^2$$

The solution matches: **13.5 GeV$^2/c^2$**.

---

### 4. The Bjorken Scaling Variable $x$

This is the sneaky part of the question.

**The Answer:**

$$x = 1$$

**The Explanation:**

The variable $x$ is defined as:

$$x = \frac{Q^2}{2 P \cdot q}$$

It is a measure of "inelasticity."

-   If $x=1$, the scattering is **Elastic**. The proton stays a proton. It bounces whole.
    
-   If $x < 1$, the scattering is **Inelastic**. The proton breaks apart (into quarks/gluons).
    

**Why is it 1 here?**

Look at the target. We started with a proton ($P^2 = M^2$). We ended with a proton ($P'^2 = M^2$).

From conservation: $P + q = P'$.

Square it: $(P+q)^2 = P'^2$.

$$P^2 + 2P \cdot q + q^2 = M^2$$

$$M^2 + 2P \cdot q - Q^2 = M^2$$

Subtract $M^2$ from both sides:

$$2P \cdot q - Q^2 = 0 \implies Q^2 = 2P \cdot q$$

Since the numerator equals the denominator, **$x$ must be 1.**

**Summary for your notes:**

-   **$E'$**: Decreased to 17.8 GeV because the electron pushed the proton.
    
-   **$Q^2$**: 13.5 GeV$^2$. This is the "resolution" of our microscope.
    
-   **$x$**: Equals 1, because the proton did not shatter.
    

Ready for the next part? I suspect we might start looking at what happens if $x \neq 1$!