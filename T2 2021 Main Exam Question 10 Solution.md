

Welcome back! It is wonderful to see you progressing through these problems. This specific exercise is a masterclass in a technique physicists use all the time: **scaling** (or dimensional analysis). By cleverly changing our units of measurement, we can often solve a whole family of problems by just solving one simple "master" equation.

First, let's translate the German text so we have a clear map of what is required:

> **Given the Hamiltonian operator in units $m_e = \hbar = 1$,**
> 
> $$\hat{H}_\alpha = -\frac{1}{2}\partial_x^2 + \alpha|x|$$
> 
> **Let the ground state have the energy $E_0(\alpha)$.**
> 
> **1. Scale the units of length so that $\hat{H} = -\frac{1}{2}\partial_y^2 + |y|$ in the corresponding units of energy.**
> 
> **2. How does $E_0(\alpha)$ depend on $\alpha$? (Justify your statement.)**

Let's break this down step-by-step.

---

### Part 1: Scaling the Units of Length

**The Physics Goal:** We want to introduce a new spatial coordinate $y$ that stretches or shrinks our old coordinate $x$ by some constant factor $c$. So, we define $y = cx$, which means $x = y/c$. We want to find the exact value of $c$ that makes the $\alpha$ disappear from the inside of the equation and move to the outside as a global energy multiplier.

**Step 1.1: Transform the Derivatives**

If we change our coordinate to $y$, we need to see how our derivative operator $\partial_x$ changes. Using the chain rule:

$$\frac{\partial}{\partial x} = \frac{\partial y}{\partial x} \frac{\partial}{\partial y} = c \frac{\partial}{\partial y}$$

Since the kinetic energy term uses the second derivative, we apply it twice:

$$\partial_x^2 = c^2 \partial_y^2$$

**Step 1.2: Substitute into the Hamiltonian**

Now, let's plug our new derivative and our expression for $x$ ($x = y/c$) into the original Hamiltonian $\hat{H}_\alpha$:

$$\hat{H}_\alpha = -\frac{1}{2} (c^2 \partial_y^2) + \alpha \left|\frac{y}{c}\right|$$

$$\hat{H}_\alpha = -\frac{1}{2} c^2 \partial_y^2 + \frac{\alpha}{c} |y|$$

**Step 1.3: Force the Equation into the Target Form**

We want this to look like some overall energy scale factor (let's call it $A$) multiplied by the clean, parameter-free Hamiltonian $\hat{H} = -\frac{1}{2}\partial_y^2 + |y|$.

$$\hat{H}_\alpha = A \left( -\frac{1}{2}\partial_y^2 + |y| \right)$$

If we distribute $A$, we get $-A\frac{1}{2}\partial_y^2 + A|y|$.

Now, we just compare the coefficients from Step 1.2 to our target:

1. From the kinetic term: $c^2 = A$
    
2. From the potential term: $\frac{\alpha}{c} = A$
    

Because both pieces must equal the exact same overall factor $A$, we can set them equal to each other:

$$c^2 = \frac{\alpha}{c}$$

Multiplying both sides by $c$ gives:

$$c^3 = \alpha \implies c = \alpha^{1/3}$$

**Conclusion for Part 1:** The correct scaling for the length is **$y = \alpha^{1/3} x$**.

If we plug this $c$ back into $A = c^2$, we find our overall energy scale is $A = \alpha^{2/3}$. Therefore, the Hamiltonian becomes:

$$\hat{H}_\alpha = \alpha^{2/3} \left( -\frac{1}{2}\partial_y^2 + |y| \right)$$

---

### Part 2: How does $E_0(\alpha)$ depend on $\alpha$?

**The Physics:** We have successfully factored our original problem into two pieces: a prefactor that contains all the $\alpha$ dependence, and a "clean" Hamiltonian that has no $\alpha$ in it at all.

Let's call that clean Hamiltonian $\hat{H}_{clean} = -\frac{1}{2}\partial_y^2 + |y|$.

Suppose we solve the Schrödinger equation for $\hat{H}_{clean}$ and find its ground state energy. Let's call that energy $E_{clean}$. (This is just a constant number, independent of $\alpha$, which happens to be $E_0(1)$).

Our Schrödinger equation is:

$$\hat{H}_\alpha \psi = E_0(\alpha) \psi$$

Substitute our result from Part 1:

$$\alpha^{2/3} \hat{H}_{clean} \psi = E_0(\alpha) \psi$$

Divide both sides by $\alpha^{2/3}$:

$$\hat{H}_{clean} \psi = \left( \frac{E_0(\alpha)}{\alpha^{2/3}} \right) \psi$$

Because $\hat{H}_{clean} \psi = E_{clean} \psi$, the term in the parentheses must simply be the constant energy $E_{clean}$:

$$\frac{E_0(\alpha)}{\alpha^{2/3}} = E_{clean}$$

$$E_0(\alpha) = \alpha^{2/3} E_{clean}$$

**Conclusion for Part 2:** The ground state energy $E_0(\alpha)$ scales proportionally to **$\alpha^{2/3}$**.

---

### Summary for your Exam

Here is a clear, step-by-step summary you can write in the text box for full marks:

> **1. Length Scaling:** > Let $y = cx$, so $x = y/c$ and $\partial_x^2 = c^2 \partial_y^2$. Substituting into the Hamiltonian gives $\hat{H}_\alpha = -\frac{1}{2}c^2\partial_y^2 + \frac{\alpha}{c}|y|$. To extract an overall energy factor $A$, we require $c^2 = \frac{\alpha}{c} = A$. Solving this yields $c = \alpha^{1/3}$. Therefore, the length is scaled as $y = \alpha^{1/3} x$.
> 
> **2. Energy Dependence:**
> 
> Using $c = \alpha^{1/3}$, the overall energy factor is $A = c^2 = \alpha^{2/3}$. The Hamiltonian can be written as $\hat{H}_\alpha = \alpha^{2/3} (-\frac{1}{2}\partial_y^2 + |y|) = \alpha^{2/3} \hat{H}_{\text{scaled}}$. Since the eigenvalue of $\hat{H}_{\text{scaled}}$ is a constant independent of $\alpha$, the ground state energy $E_0(\alpha)$ must be proportional to the prefactor. Therefore, $E_0(\alpha) \propto \alpha^{2/3}$.

This scaling trick is incredibly powerful. Would you like to see how we apply this exact same logic to quickly find how the energy levels of a quantum harmonic oscillator change if we double the mass of the particle?