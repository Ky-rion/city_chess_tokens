

Excellent! You are doing great. This next question introduces one of the most famous and profound concepts in quantum mechanics: the **Commutator**.

We are solving **Problem 5c**, which asks two things:

1.  **Calculate** the commutator $[\hat{r}, \hat{p}_r]$.
    
2.  **Explain** what this result means for measurements.
    

Let’s break this down into our manageable questions again.

---

### Question 1: What is a "Commutator"?

In normal math (like $2 \times 3$ or $x \cdot y$), the order of multiplication doesn't matter. $A \times B$ is usually the same as $B \times A$.

In Quantum Mechanics, our variables are **operators** (instructions to do something to a function), and the order **does** matter. The commutator measures the difference between doing things in one order versus the other. It is defined as:

$$[\hat{A}, \hat{B}] = \hat{A}\hat{B} - \hat{B}\hat{A}$$

**Professor's Tip:** When calculating a commutator involving derivatives, **always** apply it to an imaginary "test function" or wave function, let's call it $f(r)$. If you don't use a test function, you will likely make a mistake with the derivatives!

### Question 2: Who are the players?

We have two operators:

1.  **$\hat{r}$ (Position Operator):** This simply means "multiply by $r$".
    
2.  $\hat{p}_r$ (Radial Momentum Operator): This is given in the image from (5b) as:
    
    $$\hat{p}_r = -i\hbar \left( \frac{\partial}{\partial r} + \frac{1}{r} \right)$$
    

### Question 3: How do we calculate $[\hat{r}, \hat{p}_r]$?

Let's apply the definition $[\hat{r}, \hat{p}_r] = \hat{r}\hat{p}_r - \hat{p}_r\hat{r}$ to our test function $f(r)$.

Step A: Calculate the first term $\hat{r}\hat{p}_r f(r)$

This means "Apply momentum first, then multiply by position."

$$\hat{r} \left( \hat{p}_r f \right) = r \cdot \left[ -i\hbar \left( \frac{\partial f}{\partial r} + \frac{1}{r}f \right) \right]$$

Distribute the $r$ inside:

$$= -i\hbar \left( r \frac{\partial f}{\partial r} + r \cdot \frac{1}{r}f \right)$$

$$= -i\hbar \left( r \frac{\partial f}{\partial r} + f \right) \quad \dots \text{(Result A)}$$

Step B: Calculate the second term $\hat{p}_r\hat{r} f(r)$

This means "Multiply by position first, then apply momentum." This is the tricky one! We have to take the derivative of the product $(r \cdot f)$.

$$\hat{p}_r (r f) = -i\hbar \left( \frac{\partial}{\partial r}(rf) + \frac{1}{r}(rf) \right)$$

Use the **Product Rule** for the derivative $\frac{\partial}{\partial r}(rf) = 1 \cdot f + r \cdot \frac{\partial f}{\partial r}$:

$$= -i\hbar \left( \left[ f + r\frac{\partial f}{\partial r} \right] + \frac{1}{r}(rf) \right)$$

Simplify the last part ($\frac{1}{r} \cdot r = 1$):

$$= -i\hbar \left( f + r\frac{\partial f}{\partial r} + f \right)$$

$$= -i\hbar \left( r\frac{\partial f}{\partial r} + 2f \right) \quad \dots \text{(Result B)}$$

### Question 4: What is the difference (A - B)?

Now we subtract Result B from Result A.

$$[\hat{r}, \hat{p}_r] f = (\text{Result A}) - (\text{Result B})$$

$$= \left[ -i\hbar \left( r f' + f \right) \right] - \left[ -i\hbar \left( r f' + 2f \right) \right]$$

Factor out the $-i\hbar$:

$$= -i\hbar \left[ (r f' + f) - (r f' + 2f) \right]$$

The $r f'$ terms cancel out (this is good!):

$$= -i\hbar [ f - 2f ]$$

$$= -i\hbar [ -f ]$$

$$= i\hbar f$$

Since this is true for _any_ function $f$, we can drop the $f$ and write the operator equation:

$$[\hat{r}, \hat{p}_r] = i\hbar$$

---

### Question 5: What does this mean for measurements?

The second part of the question asks for the physical meaning.

In Quantum Mechanics, if the commutator of two observables is **zero**, it means you can measure both precisely at the same time. They are "compatible."

If the commutator is **non-zero** (like our result $i\hbar$), the observables are **incompatible**. This leads directly to a **Heisenberg Uncertainty Principle**.

The Answer to write down:

Since $[\hat{r}, \hat{p}_r] = i\hbar \neq 0$, the quantities $r$ (radial position) and $p_r$ (radial momentum) cannot be measured simultaneously with arbitrary precision.

Mathematically, they must satisfy the uncertainty inequality:

$$\Delta r \cdot \Delta p_r \ge \frac{\hbar}{2}$$

This means the more precisely you know how far the electron is from the nucleus ($\Delta r$ is small), the less you know about how fast it is moving away from the nucleus ($\Delta p_r$ becomes large), and vice versa.

Professor's Next Step:

You have now conquered the commutators! Usually, after commutators, we start looking at expectation values (averages). For example, "What is the average radius $\langle r \rangle$ of this electron?"

Would you like to try calculating the average radius next? (It usually involves a fun integral!)