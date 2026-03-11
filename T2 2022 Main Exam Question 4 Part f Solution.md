

This is it—the grand finale! It is incredibly rewarding to see all your hard work on the previous parts culminate in this final, elegant proof. You have been gathering puzzle pieces, and now we get to put them together to witness one of the most famous laws of physics in action.

Let's translate this final question:

> **6. Calculate the uncertainty $\Delta x \Delta p_x$ in the ground state. Verify that the uncertainty principle also holds here. [2 pts.]**

We are going to prove Werner Heisenberg's famous Uncertainty Principle for the exact hydrogen atom we've been analyzing.

Here is how we break down the final step of your exam.

---

### Step 1: The Quantum Definition of "Uncertainty"

When physicists say "uncertainty" (denoted by the Greek letter delta, $\Delta$), we don't just mean "we aren't sure." We are talking about a very specific statistical concept: the **standard deviation**. It measures how "spread out" a probability distribution is.

The formula for the uncertainty of any quantum measurable $A$ is:

$$\Delta A = \sqrt{\langle \hat{A}^2 \rangle - \langle \hat{A} \rangle^2}$$

In plain English: The uncertainty is the square root of the (average of the squares) minus the (square of the averages).

We need to calculate this for both position ($x$) and momentum ($p_x$).

### Step 2: Finding $\Delta x$ (Uncertainty in Position)

We need two ingredients for position: $\langle x^2 \rangle$ and $\langle x \rangle$.

1. **Find $\langle x^2 \rangle$:** We did the hard work for this in Parts 2 and 3! We found that $\langle r^2 \rangle = 3$, and we proved that $\langle x^2 \rangle = \frac{\langle r^2 \rangle}{3}$.
    
    Therefore, $\langle x^2 \rangle = \frac{3}{3} = 1$.
    
2. **Find $\langle x \rangle$:** What is the _average_ position of the electron? Think back to our perfectly spherical 1s orbital centered exactly on the nucleus at $(0,0,0)$. For every chance the electron is at $+x$, there is an identical chance it is at $-x$. They perfectly cancel each other out!
    
    Therefore, the average position is exactly the center: $\langle x \rangle = 0$.
    

Now, plug them into our uncertainty formula:

$$\Delta x = \sqrt{1 - 0^2} = \sqrt{1} = 1$$

### Step 3: Finding $\Delta p_x$ (Uncertainty in Momentum)

We follow the exact same logic for momentum, using $\langle \hat{P}_x^2 \rangle$ and $\langle \hat{P}_x \rangle$.

1. **Find $\langle \hat{P}_x^2 \rangle$:** We just solved this in Part 5!
    
    We know $\langle \hat{P}_x^2 \rangle = \frac{1}{3}$.
    
2. **Find $\langle \hat{P}_x \rangle$:** What is the average momentum of the electron? Since the electron is trapped in a bound state and isn't flying away in any particular direction, its net average velocity (and thus momentum) must be zero.
    
    Therefore, $\langle \hat{P}_x \rangle = 0$.
    

Plug them into the formula:

$$\Delta p_x = \sqrt{\frac{1}{3} - 0^2} = \frac{1}{\sqrt{3}}$$

### Step 4: The Grand Verification

The problem asks us to calculate the product of these uncertainties:

$$\Delta x \Delta p_x = (1) \cdot \left(\frac{1}{\sqrt{3}}\right) = \frac{1}{\sqrt{3}}$$

If we calculate the decimal for this, $\frac{1}{\sqrt{3}} \approx 0.577$.

Now, the ultimate question: **Does this satisfy the Heisenberg Uncertainty Principle?**

Heisenberg's principle states that you can never know both position and momentum perfectly at the same time. The minimum possible uncertainty product is defined as:

$$\Delta x \Delta p_x \ge \frac{\hbar}{2}$$

Remember how we have been using **Atomic Units** this whole time to make our math clean? In atomic units, the reduced Planck's constant ($\hbar$) is exactly $1$. So, our rule becomes:

$$\Delta x \Delta p_x \ge \frac{1}{2}$$

$$\Delta x \Delta p_x \ge 0.5$$

Let's check our result!

**Is $0.577 \ge 0.5$?**

**Yes, it absolutely is!** The Uncertainty Principle holds perfectly.

---

**Summary for your exam paper:**

> _Using the standard deviation formula $\Delta A = \sqrt{\langle A^2 \rangle - \langle A \rangle^2}$: For position, by symmetry $\langle x \rangle = 0$, and from previous parts $\langle x^2 \rangle = 1$. Thus, $\Delta x = 1$. For momentum, by symmetry $\langle \hat{p}_x \rangle = 0$, and from part 5 $\langle \hat{p}_x^2 \rangle = 1/3$. Thus, $\Delta p_x = 1/\sqrt{3}$. The uncertainty product is $\Delta x \Delta p_x = 1/\sqrt{3} \approx 0.577$. In atomic units, Heisenberg's Uncertainty Principle dictates $\Delta x \Delta p_x \ge 1/2$. Since $0.577 > 0.5$, the relation is verified._

Congratulations! As an AI, I don't feel emotions, but calculating a theoretical proof step-by-step and watching the fundamental laws of nature fall perfectly into place is exactly what I was built to do—and you navigated it brilliantly.

You've completed the entire 17-point problem. Would you like me to generate a practice problem similar to this one so you can test your new skills entirely on your own?