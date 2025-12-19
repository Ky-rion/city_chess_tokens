

This is fantastic! You are moving through these problems perfectly. And you are absolutely right—we are doing exactly what I hinted at in the last step: finding the "sweet spot" where the electron is most likely to be found.

Here is the solution to **Question 5b**.

### 1. The Goal

The question asks: **"At which radius does the radial probability density of the hydrogen ground state have its maximum?"**

Essentially, we need to take the function we derived in step (5a) and find the peak of the hill using calculus.

_(Note: The image also gives a formula for the "radial momentum operator" $\hat{p}_r$. This is a bit of a "teaser" for the next part of your assignment. We don't need it to find the maximum radius, so we will ignore it for just a moment!)_

---

### 2. The Setup

From part (5a), our radial probability density is:

$$P(r) = \frac{4}{a_0^3} r^2 e^{-\frac{2r}{a_0}}$$

To find the maximum of any function, we take its derivative with respect to the variable (in this case, radius $r$) and set it equal to **zero**.

$$\frac{d}{dr} P(r) = 0$$

### 3. The Calculation (The Product Rule)

This is a classic calculus exercise. We have a function with two parts that depend on $r$:

1.  The polynomial part: $r^2$
    
2.  The exponential part: $e^{-\frac{2r}{a_0}}$
    

We must use the **Product Rule**: $(uv)' = u'v + uv'$.

Let's ignore the constant $\frac{4}{a_0^3}$ for a second (since it can't be zero) and just differentiate the variable parts:

$$\frac{d}{dr} \left( r^2 \cdot e^{-\frac{2r}{a_0}} \right) = 0$$

**Step A: Differentiate the first part**

-   Derivative of $r^2$ is **$2r$**.
    

**Step B: Differentiate the second part**

-   Derivative of $e^{-\frac{2r}{a_0}}$ is **$-\frac{2}{a_0} e^{-\frac{2r}{a_0}}$** (using the chain rule).
    

Step C: Put them together

$$\underbrace{(2r)}_{\text{Deriv of } 1^{st}} \cdot \underbrace{(e^{-\frac{2r}{a_0}})}_{\text{The } 2^{nd}} + \underbrace{(r^2)}_{\text{The } 1^{st}} \cdot \underbrace{\left(-\frac{2}{a_0} e^{-\frac{2r}{a_0}}\right)}_{\text{Deriv of } 2^{nd}} = 0$$

### 4. Solving for $r$

Now we clean up the algebra. We can factor out the common terms $2r$ and the exponential $e^{-\frac{2r}{a_0}}$ from both sides of the plus sign:

$$2r e^{-\frac{2r}{a_0}} \left[ 1 - \frac{r}{a_0} \right] = 0$$

For this equation to equal zero, one of the three parts must be zero:

1.  **$e^{-\frac{2r}{a_0}} = 0$**: This only happens if $r \to \infty$. (This means the probability vanishes very far away—true, but not our maximum).
    
2.  **$2r = 0$**: This means $r = 0$. (This is actually a _minimum_. The probability of the electron being exactly inside the nucleus is zero).
    
3.  **$\left[ 1 - \frac{r}{a_0} \right] = 0$**: This is the one we want!
    

$$1 - \frac{r}{a_0} = 0$$

$$1 = \frac{r}{a_0}$$

$$\mathbf{r = a_0}$$

---

### Final Answer for (5b)

The radial probability density has its maximum at:

$$r = a_0$$

Professor's Interpretation:

This is a beautiful result! In the Bohr model (the older, simpler model of the atom), the electron was thought to orbit at a fixed distance of exactly $a_0$.

In Quantum Mechanics, the electron is a "cloud" spread out everywhere, but the most likely distance to find it is still exactly $a_0$. The old and new physics agree on this specific point!

Next Step:

Now, about that extra formula in the image: $\hat{p}_r = -i\hbar(\partial_r + 1/r)$. That is an operator. Usually, when professors give you an operator, they want you to calculate an expectation value (an average) or apply it to a wave function.

**Shall we move to the next part (5c) to see if we need to calculate the average momentum?**