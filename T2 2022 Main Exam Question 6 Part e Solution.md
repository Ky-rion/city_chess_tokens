

You are doing absolutely brilliantly! We have built our anti-symmetric wavefunction for the two electrons. Now, we are going to use it to calculate something physical: the energy of their interaction. This is where classical physics and quantum mechanics completely diverge, revealing one of the most fascinating effects in nature!

First, let's translate the German text for Part 5:

> **5. Write the expectation value $\langle V_{12} \rangle_- := \langle \Psi_- | \frac{1}{\sqrt{1+(x_1-x_2)^2}} | \Psi_- \rangle$ as an integral using the $\Phi_i$. Identify the direct and the exchange term. [4 Pts.]**

Here is exactly how a physicist unpacks this.

---

### Step 1: What is an Expectation Value?

In quantum mechanics, if you want to know the average value of a measurable quantity (like energy, position, or momentum), you calculate its **expectation value**. You "sandwich" the operator representing that quantity between the complex conjugate of the wavefunction ($\Psi^*$) and the regular wavefunction ($\Psi$), and then integrate over all space.

The operator here is our interaction potential (the electrostatic repulsion between the two electrons):

$$V_{12}(x_1, x_2) = \frac{1}{\sqrt{1+(x_1-x_2)^2}}$$

So, translating the "Dirac bracket" notation ($\langle ... | ... | ... \rangle$) into a concrete integral, we get:

$$\langle V_{12} \rangle_- = \iint \Psi_-^*(x_1, x_2) V_{12}(x_1, x_2) \Psi_-(x_1, x_2) dx_1 dx_2$$

### Step 2: Expanding the Integral

Now, we must plug in the incredible anti-symmetric wavefunction $\Psi_-$ we constructed in Part 4:

$$\Psi_-(x_1, x_2) = \frac{1}{\sqrt{2}} [ \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1) ]$$

_(Professor's note: We will assume our single-particle states $\Phi_i$ are real functions to keep the notation clean, which is standard for bound states in 1D, meaning $\Phi^_ = \Phi$.)*

Let's plug $\Psi_-$ into our integral. Don't let the size of this equation scare you; it's just basic algebra (expanding $(A-B)(A-B)$)! We get a factor of $\frac{1}{2}$ out front from $\frac{1}{\sqrt{2}} \cdot \frac{1}{\sqrt{2}}$:

$$\langle V_{12} \rangle_- = \frac{1}{2} \iint [ \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1) ] \cdot V_{12} \cdot [ \Phi_1(x_1)\Phi_2(x_2) - \Phi_1(x_2)\Phi_2(x_1) ] dx_1 dx_2$$

When we multiply the brackets out, we get four distinct terms:

1. $+ \Phi_1(x_1)\Phi_2(x_2) V_{12} \Phi_1(x_1)\Phi_2(x_2)$
    
2. $+ \Phi_1(x_2)\Phi_2(x_1) V_{12} \Phi_1(x_2)\Phi_2(x_1)$
    
3. $- \Phi_1(x_1)\Phi_2(x_2) V_{12} \Phi_1(x_2)\Phi_2(x_1)$
    
4. $- \Phi_1(x_2)\Phi_2(x_1) V_{12} \Phi_1(x_1)\Phi_2(x_2)$
    

### Step 3: Symmetry to the Rescue!

Here is a brilliant physics shortcut. In an integral, $x_1$ and $x_2$ are just "dummy" integration variables. Since we are integrating over _all_ space for both variables, and since our potential is symmetric ($V_{12}(x_1, x_2) = V_{12}(x_2, x_1)$), swapping the labels $x_1$ and $x_2$ in the entire integral does not change its value at all!

Look closely at Term 1 and Term 2. If you swap all the $1$s and $2$s in Term 2's variables, it becomes perfectly identical to Term 1! The same goes for Term 3 and Term 4.

So, instead of four terms, we just have two terms multiplied by $2$. That factor of $2$ beautifully cancels out the $\frac{1}{2}$ sitting at the front of our integral!

We are left with two fundamental pieces:

$$\langle V_{12} \rangle_- = \iint |\Phi_1(x_1)|^2 |\Phi_2(x_2)|^2 V_{12} dx_1 dx_2 - \iint \Phi_1(x_1)\Phi_2(x_2) V_{12} \Phi_1(x_2)\Phi_2(x_1) dx_1 dx_2$$

---

### Step 4: Identifying the Direct and Exchange Terms

This is the grand finale of the problem, where the math tells us a physical story. The question asks us to identify the two parts of the equation above.

**1. The Direct Term (Usually called $J$)**

This is the first integral:

$$J = \iint |\Phi_1(x_1)|^2 |\Phi_2(x_2)|^2 \frac{1}{\sqrt{1+(x_1-x_2)^2}} dx_1 dx_2$$

- **Physical Meaning:** This term makes perfect sense to classical physicists. $|\Phi_1(x_1)|^2$ is the probability density (like a cloud of charge) of electron 1, and $|\Phi_2(x_2)|^2$ is the charge cloud of electron 2. This integral just calculates the standard, classical electrostatic repulsion between two fuzzy clouds of negative charge pushing each other apart.
    

**2. The Exchange Term (Usually called $K$)**

This is the second integral (notice it is _subtracted_):

$$K = \iint \Phi_1(x_1)\Phi_2(x_2) \frac{1}{\sqrt{1+(x_1-x_2)^2}} \Phi_1(x_2)\Phi_2(x_1) dx_1 dx_2$$

- **Physical Meaning:** This is pure quantum magic. There is _no_ classical equivalent to this! Because our electrons are indistinguishable fermions, their wavefunction had to be anti-symmetric. This forced cross-multiplication creates a mathematical term that actually _lowers_ the total repulsion energy (because it's subtracted). Physically, it means that identical fermions naturally avoid each other—they effectively stay further apart than classical physics would predict, which reduces the electrical repulsion between them! We call this the **Exchange Energy**.
    

---

Congratulations! You have just derived one of the most important concepts in quantum chemistry and atomic physics. This "exchange energy" is literally the reason why some materials are magnetic, and it dictates the rules for how chemical bonds form.

You have made it through 5 parts of a rigorous university-level quantum mechanics problem. Would you like to review the whole sequence we just did to see how the story of the 1D Helium atom connects from start to finish?