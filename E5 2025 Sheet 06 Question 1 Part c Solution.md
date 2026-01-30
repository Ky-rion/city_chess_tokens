

![[Pasted image 20260128115424.png]]

Welcome back! You are flying through these.

Now we get to do the "sanity check." In physics, whenever we derive a fancy general rule (like we did in part b), we immediately test it on a specific case where we already know the answer. If the math works out, it confirms our general rule is solid.

In this problem, we are looking at a **Gaussian** charge distribution.

### The Setup

From **part (b)**, we derived this powerful "Master Formula" relating the size of the nucleus to the slope of its form factor:

$$\left. \frac{dF}{d(q^2)} \right|_{q=0} = -\frac{\langle r^2 \rangle}{6\hbar^2}$$

For part (c), we want to find $\langle r^2 \rangle$, so let's rearrange that formula to solve for it:

$$\langle r^2 \rangle = -6\hbar^2 \left[ \frac{dF}{d(q^2)} \right]_{q=0}$$

This is our roadmap. We just need to calculate that derivative and plug it in.

---

### Step 1: Understanding the Function

We are given the form factor for a Gaussian distribution:

$$F(q) = \exp\left( - \frac{q^2}{2a^2\hbar^2} \right)$$

We need to take the derivative with respect to $q^2$.

**Student Tip:** This notation $d/d(q^2)$ can be confusing. The easiest way to handle it is to do a simple substitution.

Let's define a variable $u = q^2$.

Now, rewrite the function in terms of $u$:

$$F(u) = \exp\left( - \frac{u}{2a^2\hbar^2} \right)$$

Now, the derivative $\frac{dF}{d(q^2)}$ just becomes a standard derivative $\frac{dF}{du}$.

---

### Step 2: Taking the Derivative

We need to differentiate $F(u)$ with respect to $u$.

Recall the rule for differentiating exponentials: $\frac{d}{dx} e^{kx} = k e^{kx}$.

In our case, the constant "k" in front of our variable $u$ is:

$$k = -\frac{1}{2a^2\hbar^2}$$

So, the derivative is:

$$\frac{dF}{du} = \left( -\frac{1}{2a^2\hbar^2} \right) \cdot \exp\left( - \frac{u}{2a^2\hbar^2} \right)$$

---

### Step 3: Evaluate at $q=0$

The formula requires the value of the slope specifically at $q=0$.

If $q=0$, then our substitution variable $u = q^2 = 0$.

Let's plug $u=0$ into our derivative:

$$\left. \frac{dF}{du} \right|_{u=0} = -\frac{1}{2a^2\hbar^2} \cdot \underbrace{\exp(0)}_{1}$$

So, the slope at the origin is simply:

$$\text{Slope} = -\frac{1}{2a^2\hbar^2}$$

---

### Step 4: The Final Calculation

Now, we bring back our rearranged "Master Formula" from the very beginning and plug in our slope.

$$\langle r^2 \rangle = -6\hbar^2 \cdot (\text{Slope})$$

$$\langle r^2 \rangle = -6\hbar^2 \cdot \left( -\frac{1}{2a^2\hbar^2} \right)$$

Now, we just do the algebra clean-up:

1.  **Negatives cancel:** $(- ) \times (-) = (+)$
    
2.  **$\hbar^2$ cancels:** One in the numerator, one in the denominator.
    
3.  **Numbers simplify:** $6 / 2 = 3$.
    

$$\langle r^2 \rangle = \frac{3}{a^2}$$

---

### Professor's Concluding Remarks

We did it! We arrived at $\langle r^2 \rangle = 3/a^2$.

Why is this satisfying? The problem statement mentions: _"In the last attendance exercise we showed that [the radius] is given by $3/a^2$."_

This means our two different methods—calculating the radius directly from the charge density (exercise 5) and calculating it from the scattering form factor (this exercise)—gave the **exact same answer**.

**A quick nugget of wisdom for your future studies:**

You noticed that the charge distribution was a **Gaussian** and the resulting Form Factor $F(q)$ was _also_ a **Gaussian** (an exponential of $q^2$).

This is not a coincidence! The Form Factor is essentially the **Fourier Transform** of the charge distribution. A unique property of Gaussian functions is that their Fourier Transform is also a Gaussian. That's why the math worked out so cleanly here.

Excellent work today! You've just walked through the fundamental mathematical machinery we use to measure the size of subatomic particles.