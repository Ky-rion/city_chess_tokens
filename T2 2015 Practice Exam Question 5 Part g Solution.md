

It has been a pleasure working through this entire problem with you. This final part, (g), is the capstone that brings all our previous results together to demonstrate a profound physical principle.

## 🧠 The Goal: Verify the Heisenberg Uncertainty Principle

This problem asks us to do two things:

1.  **Explicitly verify** that the Heisenberg Uncertainty Relation is satisfied for all energy states $|n\rangle$.
    
2.  Find the specific state $n$ for which the uncertainty is **minimal**.
    

Let's start by stating the principle itself.

---

### 1. What is the Heisenberg Uncertainty Principle?

The uncertainty principle, in its general form, states that for any two observables (operators) $\hat{A}$ and $\hat{B}$, the product of their uncertainties ($\Delta A$ and $\Delta B$) in any given state must be greater than or equal to a minimum value, which is determined by their commutator:

$(\Delta A) (\Delta B) \ge \frac{1}{2} | \langle [\hat{A}, \hat{B}] \rangle |$

For our problem, we are interested in $\hat{A} = \hat{x}$ (position) and $\hat{B} = \hat{p}$ (momentum). So, we must verify that:

**$(\Delta x) (\Delta p) \ge \frac{1}{2} | \langle [\hat{x}, \hat{p}] \rangle |$**

Let's calculate all the pieces of this inequality using our results from parts (d), (e), and (f).

---

### 2. Step-by-Step Verification

#### Step 1: Calculate the Uncertainties $\Delta x$ and $\Delta p$

The uncertainty $(\Delta O)$ of an operator $\hat{O}$ is the standard deviation, defined by the formula:

$(\Delta O)^2 = \langle \hat{O}^2 \rangle - \langle \hat{O} \rangle^2$

-   Position Uncertainty $(\Delta x)$:
    
    From part (e), we found the average position $\langle \hat{x} \rangle = 0$.
    
    From part (f), we found $\langle \hat{x}^2 \rangle = n + \frac{1}{2}$.
    
    $(\Delta x)^2 = \langle \hat{x}^2 \rangle - \langle \hat{x} \rangle^2 = \left( n + \frac{1}{2} \right) - (0)^2 = n + \frac{1}{2}$
    
    Therefore, $\Delta x = \sqrt{n + \frac{1}{2}}$.
    
-   Momentum Uncertainty $(\Delta p)$:
    
    From part (e), we found the average momentum $\langle \hat{p} \rangle = 0$.
    
    From part (f), we found $\langle \hat{p}^2 \rangle = n + \frac{1}{2}$.
    
    $(\Delta p)^2 = \langle \hat{p}^2 \rangle - \langle \hat{p} \rangle^2 = \left( n + \frac{1}{2} \right) - (0)^2 = n + \frac{1}{2}$
    
    Therefore, $\Delta p = \sqrt{n + \frac{1}{2}}$.
    

#### Step 2: Calculate the Uncertainty Product

Now, let's multiply the two uncertainties together:

$(\Delta x) (\Delta p) = \left( \sqrt{n + \frac{1}{2}} \right) \left( \sqrt{n + \frac{1}{2}} \right)$

$(\Delta x) (\Delta p) = n + \frac{1}{2}$

This is the "left-hand side" of our inequality.

#### Step 3: Calculate the "Right-Hand Side"

The right side of the inequality is $\frac{1}{2} | \langle [\hat{x}, \hat{p}] \rangle |$.

From part (d), we calculated the commutator:

$[\hat{x}, \hat{p}] = i$

Since $i$ is just a number (not an operator), its expectation value is just itself:

$\langle [\hat{x}, \hat{p}] \rangle = \langle n | i | n \rangle = i \langle n | n \rangle = i(1) = i$

Now, we take the absolute value (or magnitude) of this complex number:

$|i| = 1$

So, the entire right-hand side of the HUP inequality is:

$\frac{1}{2} | \langle [\hat{x}, \hat{p}] \rangle | = \frac{1}{2} (1) = \frac{1}{2}$

#### Step 4: Compare Both Sides

Let's plug our results back into the main inequality:

$(\Delta x) (\Delta p) \ge \frac{1}{2} | \langle [\hat{x}, \hat{p}] \rangle |$

$n + \frac{1}{2} \ge \frac{1}{2}$

The energy level $n$ can be any integer $n = 0, 1, 2, 3, \dots$.

-   If $n = 0$, the relation is $\frac{1}{2} \ge \frac{1}{2}$, which is **true**.
    
-   If $n = 1$, the relation is $1 + \frac{1}{2} \ge \frac{1}{2}$, which is **true**.
    
-   If $n = 2$, the relation is $2 + \frac{1}{2} \ge \frac{1}{2}$, which is **true**.
    

Since $n$ is always positive or zero, the quantity $n + \frac{1}{2}$ will always be greater than or equal to $\frac{1}{2}$.

We have therefore explicitly verified that the Heisenberg Uncertainty Relation is satisfied for all $n$.

---

### 3. For Which $n$ is the Uncertainty Minimal?

Now we answer the second part of the question. We want to find the value of $n$ that makes the uncertainty product $(\Delta x) (\Delta p) = n + \frac{1}{2}$ as small as possible.

Since $n \ge 0$, the smallest possible value for $n$ is **$n=0$**.

**The uncertainty is minimal for the $n=0$ state (the ground state).**

When $n=0$, the uncertainty product is:

$(\Delta x) (\Delta p) = 0 + \frac{1}{2} = \frac{1}{2}$

This is a beautiful result! The ground state of the quantum harmonic oscillator is a "minimum uncertainty state." It is as "localized" in both position and momentum as quantum mechanics will possibly allow, perfectly satisfying the lower bound of the Heisenberg Uncertainty Principle.

Congratulations on completing this entire problem set! This is a cornerstone of quantum mechanics, and you've now worked through all the essential parts.

Do you have any questions about what we've done, or would you like to discuss the physical meaning of any of these results?