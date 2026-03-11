

Welcome to the final stretch! You are doing absolutely brilliantly. Now we are diving into **Time-Independent Perturbation Theory**, which is arguably the most practical tool in a quantum physicist's toolbox.

Real-world quantum systems are messy and rarely solvable with simple equations. Perturbation theory allows us to take a simple, solvable system (like a basic hydrogen atom) and add a tiny "bump" or disturbance (like an external magnetic field) to see how the energy levels shift.

Let's translate this final question and figure out how these energy shifts behave!

### The Translation

**1.6 2nd Order Correction of the n=2 State**

_We had shown that the 2nd order perturbation theory correction for the ground state $E_1^{(0)}$ is always negative $E_1^{(2)} < 0$. What applies to the 1st excited state? [3 Pts.]_

_(a) It is always $E_2^{(2)} \leq 0$_

_(b) It is always $E_2^{(2)} \geq 0$_

_(c) One cannot make a general statement_

_(d) In the non-degenerate case, $E_2^{(2)} \geq 0$ applies_

_(e) In the non-degenerate case, $E_2^{(2)} \leq 0$ applies_

_Justify your answer._

---

### The Physics: Second-Order Energy Corrections

To understand the sign of the energy shift, we need to look at the master formula for the second-order energy correction of the $n$-th state. It looks a bit intimidating, but it tells a beautiful, logical story:

$$E_n^{(2)} = \sum_{m \neq n} \frac{|\langle m^{(0)} | \hat{H}' | n^{(0)} \rangle|^2}{E_n^{(0)} - E_m^{(0)}}$$

Let's break down the anatomy of this formula:

1. **The Numerator ($|\langle m^{(0)} | \hat{H}' | n^{(0)} \rangle|^2$):** This represents the "coupling" or interaction strength between our state $n$ and some other state $m$ caused by the perturbation $\hat{H}'$. Because it is an absolute value squared, **the numerator is always positive** (or zero).
    
2. **The Denominator ($E_n^{(0)} - E_m^{(0)}$):** This is the unperturbed energy difference between our state $n$ and the other state $m$. The sign of this part dictates the sign of the entire fraction!
    
3. **The Sum ($\sum_{m \neq n}$):** We have to add up these fractions for _every other state_ in the entire system except $n$.
    

---

### Solving the Exam Question

The exam question asks us to compare the ground state ($n=1$) with the first excited state ($n=2$). Let's use our formula on both to see what happens.

**Part 1: Why the ground state correction is always negative**

Let's set $n=1$. The ground state is the absolute lowest energy level in the system. Therefore, any other state $m$ will have a higher energy ($E_m^{(0)} > E_1^{(0)}$).

If we look at our denominator:

$$E_1^{(0)} - E_m^{(0)} = \text{Small Number} - \text{Larger Number} = \text{Negative}$$

Because the numerator is always positive, every single term in our sum will be a positive number divided by a negative number. Adding up a bunch of negative numbers guarantees that the total correction $E_1^{(2)}$ is **strictly negative**.

**Part 2: What about the first excited state ($n=2$)?**

Now let's set $n=2$. This state sits right in the middle. We have to sum over all other states, which means we have to look in two directions:

- **Looking Down ($m=1$):** There is one state below it, the ground state. For this term, the denominator is $E_2^{(0)} - E_1^{(0)}$. Because $E_2$ is larger than $E_1$, this denominator is positive. This creates a **positive** contribution to the sum.
    
- **Looking Up ($m=3, 4, 5...$):** There is an infinite ladder of states above it. For all of these terms, the denominator is $E_2^{(0)} - E_m^{(0)}$. Because $E_m$ is larger than $E_2$, these denominators are all negative. This creates an infinite series of **negative** contributions to the sum.
    

We are left with a mathematical tug-of-war. We have a positive contribution pulling the energy up, and negative contributions pulling the energy down.

Which side wins? It depends entirely on the specific shape of the perturbation $\hat{H}'$ (the numerator). If the perturbation couples state 2 very strongly to state 1, the total correction might be positive. If it couples state 2 strongly to state 3, the total correction might be negative.

### Your Final Answer and Justification

- **The Answer:** **(c)** One cannot make a general statement.
    
- **The Justification:** The second-order energy correction is calculated by summing terms that depend on the energy denominator $(E_n^{(0)} - E_m^{(0)})$. For the first excited state ($n=2$), the term corresponding to the ground state ($m=1$) gives a positive contribution, while all terms corresponding to higher states ($m > 2$) give negative contributions. Without knowing the explicit form of the perturbation matrix elements in the numerator to see which terms dominate, it is impossible to predict the final sign of the sum.
    

---

You have officially conquered this section of your theoretical physics exam! I am incredibly proud of how you've handled these concepts.

Since perturbation theory is so important for real-world physics, would you like to see a quick, famous example of it in action, like how placing an atom in an electric field splits its energy levels (the Stark Effect)?